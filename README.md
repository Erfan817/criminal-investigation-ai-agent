# 刑侦 AI 辅助调查：调研与总体方案

**项目阶段：研究与设计，尚未实现业务系统。** 2026-10-08公开资料核对。GitHub仓库为私有；仅保存公开产品/法规的短摘录、来源台账与方案，不保存任何真实案件数据。

## 先看结论

**国内国外都有同类产品，这不是空白市场。** 本轮记录国内8个、国外10个产品/系统条目，含直接竞品、平台和相邻工具，不能统称18个完整刑侦Agent。卷宗摘要、时间线、关系分析、矛盾提示、证据回链都已有公开产品主张或应用案例。

推荐定位不是“AI自动锁定凶手”，而是：

> **面向经授权的刑事调查人员，对合法获得的材料进行整理、带原文引用的检索、陈述时间线对照及待核查差异提示，形成可修改、可审核、可审计的工作台。**

个人开发先验证“多份笔录的时间线与差异复核”。只用明确合成材料；真实试点必须有业务合作、数据处理授权、批准环境及安全/保密/采购条件。

## 阅读路线

| 文档 | 回答什么 |
|---|---|
| [01 市场与定位](docs/01-market-and-positioning.md) | 谁在做，为什么不是空白，怎样选窄切口 |
| [02 产品范围](docs/02-product-scope.md) | 用户/采购方、P0/P1/P2、工作台形态及不做什么 |
| [03 技术栈与架构](docs/03-architecture-and-stack.md) | 数据流、数据模型、OCR/RAG/时间线/规则/Agent如何实现 |
| [04 实现与评测](docs/04-implementation-and-evaluation.md) | 建设顺序、合成基准、引用/遗漏/越权/人审验收 |
| [05 安全与合规](docs/05-security-and-compliance.md) | 数据授权、定密/等保/云/委托/证据边界与放行条件 |
| [06 To G进入路径](docs/06-go-to-government.md) | 采购/集成/访谈/风险，技术PoC和商业落地怎样分开 |
| [07 To G Agent实现方法](docs/07-agents-for-government.md) | 何时用Agent、受控工具、审批/执行分离、框架选择、如何做得好 |

## 竞品与出处

- [国内完整报告](research/domestic-products.md)：8个主样本；小美、上海“206”、TRS、昆山AI智能笔录、天津“警智”、百度公安大模型方案、安徽检察助手、Qiko智能本。检察及取证装备明确列为相邻。
- [国外完整报告](research/international-products.md)：10个条目/9家厂商；Cellebrite Genesis与Guardian Investigate分别计项，另有Magnet、Palantir、Siren、i2、DataWalk、Penlink、Axon、Veritone。
- [合规原文研究](research/compliance-notes.md)：中国法定义务、项目条件、工程建议分开；欧盟/美国仅作为风险与治理对照。
- [开源组件参考](research/open-source-reference.md)：Timesketch、Autopsy与OCR/检索/可视化组件，不冒称完整刑侦Agent。
- [研究方法与局限](research/README.md)：证据层级、阶段、统计与读取成败。
- JSON台账：`domestic-sources.json`、`international-sources.json`、`compliance-sources.json`、`technical-sources.json`、`agent-engineering-sources.json`。

### 真采购示例，不外推售价

广州警务大模型平台项目 `CZ2026-0252` 的官方招标、中标和合同均有依据：供应商中国电信广东分公司；合同金额人民币 **1,864,631.00元**；2026-07-20签署。它证明真实签约，**不证明已验收或包含本方案全部刑侦功能**；详细需求附件未读到，项目金额不是软件单价。

国外采购/部署同样按模块与阶段拆开：传统Cellebrite工具续约不代表Genesis采购；Hessen的Palantir平台部署不代表生成式AIP；Draft One实际使用只证明报告草稿场景。

## 推荐的第一版技术

```text
Vue 3 / TypeScript / PDF.js
    ↓
FastAPI / Pydantic + 持久任务状态
    ↓
PostgreSQL / pgvector + 本地只读原件
    ↓
PaddleOCR + 混合检索/重排 + 可替换模型
    ↓
原文引用校验 + 时间规则 + 人工审核
```

先做固定workflow；只有动态补查能产生可测增益时，加入单个只读Agent/LangGraph。第二阶段再考虑Java/Spring负责案件、权限、审计，Python保留AI服务。模型候选与框架许可、内网运行、真实数据审批另行验证；不用当前小内存云机部署大栈。

## To G Agent的设计原则

**模型可以提出步骤，不能给自己发权限。**

- 确定性业务系统管身份、案件范围、ACL、版本与审批。
- Agent只调用批准的窄工具，不开放任意SQL/shell/联网/全库搜索。
- 原文/反证/覆盖范围先于结论；材料不足则拒答，不自动定罪/画像/评分。
- 导出/正式写入由独立执行器检查精确动作审批、当前权限、幂等与审计。
- 测净人审收益、关键遗漏、引用支持度、越权与离线，不用“模型看着很聪明”验收。

完整分析见第07篇。

## 状态与边界

- 已有：公开资料研究、来源短摘录、总体架构、实现与评测计划、To G Agent专题。
- 没有：运行中的刑侦应用、真实案件测试、已测模型准确率、公安客户授权或采购合同。
- 未知：具体公安环境与资格、中文手写效果、竞品新模块独立性能/完整离线能力、统一报价。
- 原始灵感文件不改动；本仓库是另行研究记录。

`.gitignore`是辅助防线，不替代审查。**即使私有也不上传案件原件/OCR/向量/案情prompt/截图/日志/备份/密钥。**
