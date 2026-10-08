# 国外刑侦 AI 调查助手与数字取证/情报分析竞品：证据型清单

- **调研日期：2026-10-08。** 比较依法取得的案件材料整理、检索与研判辅助；不提供身份识别、跟踪或预测警务操作教程。
- **收录：10个条目、9家厂商；52个已读正文来源，其中6个政府/执法机关原始来源。** Cellebrite 的 Genesis 与 Guardian Investigate 按不同工作流计两项；配套工具只解释角色。
- 这是公开证据调研，不是产品实测。文末登记来源URL、日期依据、摘录与阅读范围；结构化文件为 `international-sources.json`。

## 主要结论

1. **案件材料问答、摘要/时间线/关系与源证据回链已存在直接竞品，不能按市场空白立项。** Genesis 官网明确 contradictions 和来源回链；Guardian Investigate 明确文档摘要、不一致提示与案件工作台；Magnet Intelligent Insights 明确引用验证、关系/时间线及多分析 agentic workflow。[CEL01][CEL04][MAG02]
2. **新发布、早期访问、一般可用与真实部署要分开。** Genesis 2026-03-16首发为early access，另一官方文章写2026-06 GA且有具名客户证言；Magnet当前Review产品页仍写Intelligent Insights早期访问且限美国/英国。不能统称“早已全球规模落地”。[CEL06][CEL05][MAG04]
3. **平台与开箱即用刑侦助手不同。** Palantir、Siren、DataWalk、i2在数据整合、图谱、协作和治理上是上位或相邻竞品。Siren正式文档已有K9插件与本地模型接口；i2当前属Harris，传统图谱/时间分析成熟，但本轮未核实“i2 Copilot”正式产品。[PAL06][SIR06][SIR09][I203][I205]
4. **传统产品采购不能证明新生成式模块在用。** Leicestershire已签合同只确认Inseyets等取证产品；Hessen政府证明Palantir平台本地部署，不证明AIP生成式能力；Arvada政府确认Draft One使用，但它是报告草稿工具，非完整破案Agent。[GOV11][PAL05][AXO04]
5. **必须降级的落地主张**：Penlink匿名real-world examples无机构/案号；Veritone的Beverly Hills引文是would benefit，不是已部署；Tradewinds的Awardable是可采购状态，不是订单。[PEN04][VER05][VER04]
6. **适合差异化的方向是可审计、可复核的中文案件材料工作台**：内网/离线可用、中文卷宗处理、断言级证据定位、可解释矛盾核查和版本留痕。这是建议验收项，不是已证明的市场空白。AI输出不自动成为新证据或鉴定结论，更不能作为自动定罪依据。

## 证据分级

|代码|含义|不能推导的结论|
|---|---|---|
|A|政府/警局原始合同、会议/政策或自有部署说明|试点、拟采购、被阻采购虽有A级来源，仍不等于已签/已上线|
|B|厂商具名客户或合同案例|不等于政府独立核验或原始授标合同|
|C|厂商匿名案例|不等于具名真实客户或可复现破案效果|
|D|官方产品、技术文档、新品发布/demo|证明描述/存在，不证明客户实际采用|
|K|Framework、GSA/BPA/vehicle、marketplace、Awardable|可买/入围不等于已买，框架上限不是单家收入|

“明确”仅表示官方正文明确描述；“部分”是邻接功能，未实测同一工作流；“未见”指本轮证据不足，不等于功能不存在。

## 快速对比

|编号|产品/系统|类型|摘要|时间线|关系图|矛盾检查|引用|客户/采购证据|
|---|---|---|---|---|---|---|---|---|
|P01|Cellebrite Genesis|直接调查助手|明确|明确|明确|明确主张|明确回链|B具名实际案工作；新模块政府合同未得|
|P02|Guardian Investigate；Inseyets/Pathfinder配套|直接工作台|明确|明确|明确|明确主张|部分|D Investigate；A合同只证配套Inseyets|
|P03|Magnet AI / Review Intelligent Insights|直接引用型分析|明确|明确|关系分析明确，图UI未证|未证|明确|D新AI早期开放；B历史AI/Automate|
|P04|Gotham / Europa + AIP|可定制上位平台|可构建，警方案例未证|具体功能未证|平台关联证据|未证|血缘/审计，非逐句引文|A Hessen部署；英国拟采购受阻|
|P05|Siren Investigate / K9|图谱AI助手|图谱报告|传统时间分析|明确|未证|records/图数据，逐答引用未证|C匿名sheriff实施；K9具名客户未证|
|P06|i2 Analyst’s Notebook / iBase / Hub|相邻成熟平台|情报产品，LLM全卷未证|明确|明确|未证|源数据/人工核查|B Vancouver/BC；Copilot未核实|
|P07|DataWalk Graph + AI|图谱与调查平台|明确|部分/形式未证|明确|异常不等于证言矛盾|血缘，逐句引文未证|B Anderson/DOJ厂商稿；C匿名GenAI；K渠道|
|P08|Penlink CoAnalyst / PLX|直接嵌入助手|明确|明确文字主张|可视化/匿名图案例|异常不等于证言矛盾|审计/源分离，精确回链未证|C匿名故事+D发布|
|P09|Axon Draft One|相邻报告草稿|场景草稿非全卷|叙事非分析器|未见|未见|源录音/转写可核对|A Arvada政府确认使用|
|P10|Veritone Investigate / iDEMS|相邻多模态证据平台|全卷界面未证|专属功能未证|专属功能未证|未见|索引/管理，逐答引文未证|K Awardable；具名上线未证|

不按营销关键词对准确率排名，不把厂商“快若干倍”、聚合客户数、破案率当独立效果证据。

## 名称与角色核对

- **Genesis**：独立云端、单案件多源AI助手；多设备可放同案。官方把跨案件连接归于**Pathfinder**，不能混为Genesis已有全域跨案推理。[CEL01]
- **Guardian**：云原生证据管理、保管链与共享套件；**Guardian Investigate**是案情管理/AI工作台；**Inseyets（UFED、Physical Analyzer）**是提取/解析输入链。Inseyets独立产品页未读到可用正文，但Guardian集成说明与政府合同支持名称/角色。[CEL03][GOV11]
- **Pathfinder**：多设备AI分析、Timeline与Link Analysis；有本地VM/服务器和AWS VPC证据，不可移植为Genesis/Investigate离线证明。[CEL02]
- **Magnet AI**是2026生态intelligence engine；**Review Intelligent Insights**是直接分析功能；历史**Magnet.AI**图像预标注与**AUTOMATE**取证编排不能混写为同一代生成式Agent。[MAG02][MAG03][MAG07]
- **Gotham / AIP**分别是情报平台与可构建AI工作流/Agent的平台能力；警方用了Palantir不足以确定用了AIP。[PAL05][PAL06]
- **Siren**官方技术导航已有Platform16.0、AI plugin2.1，**K9 Companion**有文档；营销页仍展示Siren14，不把它当最新版本。[SIR10][SIR06]
- **i2**当前属Harris/Constellation而非IBM；“Copilot”正式名称与上市状态本轮未核实。[I205][I204]
- **CoAnalyst**的2025 Agentic迭代与2026 PLX集成正文已读；2024-05-15首发只有检索线索、正文失败，不升格为正文证实日期。[PEN02][PEN03]
- **Draft One**是报告草稿；**Investigate/iDEMS**是证据hub/套件，不是已证明的完整自动破案Agent。[AXO04][VER04]

## 逐项竞品与证据

### P01｜Cellebrite Genesis

- **厂商/地区**：Cellebrite；以色列；在美国设业务实体（发布稿署名 Petah Tikva / Tysons Corner）。
- **定位**：直接竞品：面向单案件的生成式/Agentic AI 调查助手。
- **核心功能**：
  - 自然语言跨证据问答；支持 UFDR、文档、音视频、CDR 等多种证据格式。
  - 摘要、时间线、关系与跨文件连接、矛盾线索提示。
  - 答案回链原始材料，人工验证；单案件内可放多设备，不等于跨案件分析。
- **目标工作流重合**：
  - **卷宗摘要**：明确：可问答和摘要，但中文纸质卷宗/OCR质量未验证。
  - **时间线**：明确：timeline 可视化。
  - **关系图**：明确：relationships / mind maps；不是已验证的身份认定。
  - **矛盾检查**：明确：页面写 contradictions；没有检出率/误报率证据。
  - **证据引用**：明确：每个回答链接来源材料；页码/音视频时码粒度未实测。
- **部署/可用性**：官方 FAQ 明确 cloud-based，可独立于其他 Cellebrite 工具使用。2026-03-16 发布稿为 early access；另一官方文章写 2026-06 已 generally available。未找到 Genesis 专属本地/完全离线部署证明；不能用厂商全组合的 on-prem/hybrid 描述替代。
- **客户/采购证据与阶段**：
  - **B：厂商具名客户案例**：官方 Genesis 文章引用 Ocean County Prosecutor’s Office 实验室主任 Jim Hill 与 Calcasieu Parish Sheriff’s Office 数字取证单位 Jerod K. Abshire，描述真实案工作与人工验证。只有厂商载体，未取到这些单位自己的发布或 Genesis 采购合同。 [CEL05]
  - **C：厂商匿名早期客户**：首发稿引用匿名澳大利亚警方反恐侦探的早期体验；不当作具名规模化落地。 [CEL06]
- **未核实**：中文/中文手写卷宗支持；源引用到页码/段落/时码的粒度；独立准确率与幻觉/矛盾检出率；具名客户自有发布、采购金额、离线部署。
- **正文读取**：是：官方产品 FAQ、官方案例文章与发布稿正文；不是产品实测。
- **来源链接**：[CEL01](https://cellebrite.com/en/products/cellebrite-genesis/)；[CEL05](https://cellebrite.com/en/blog/the-new-age-of-investigations-cellebrites-journey-to-genesis/)；[CEL06](https://cellebrite.com/en/resources/press-releases/cellebrite-launches-genesis-agentic-ai-for-digital-investigations-cellebrite/)。

### P02｜Cellebrite Guardian Investigate（Guardian 套件；旁列 Inseyets / Pathfinder）

- **厂商/地区**：Cellebrite；以色列/美国。
- **定位**：直接竞品：案件工作台与调查管理；含相邻数字取证/证据管理组合。
- **核心功能**：
  - 把案件证据、文档、调查任务集中在同一工作台；自然语言问答与结构化报告。
  - 摘要文档、发现不一致、构建案件时间线、可视化关系。
  - Guardian 本体承担证据管理/共享与保管链；Inseyets 负责提取/解析，Pathfinder 负责多设备与跨案件分析，不能混称同一个 Agent。
- **目标工作流重合**：
  - **卷宗摘要**：明确：summarize documents。
  - **时间线**：明确：Build Timelines。
  - **关系图**：明确：可视化 relationships；Pathfinder 的 link analysis 另有官方证明。
  - **矛盾检查**：明确：spot inconsistencies；尚无正式评测。
  - **证据引用**：部分：Guardian 保管链、案内源数据与权限控制明确；Investigate 逐条生成断言的精确引用粒度未核实。
- **部署/可用性**：Guardian / Guardian Investigate 官方均为 cloud-native / cloud-based，Investigate 写 Powered by AWS。Guardian Collaborate 的 FedRAMP High 是特定联邦环境描述，不可扩张到 Genesis 或所有 Investigate 功能。Pathfinder 单独明确支持 on-prem VM/实体服务器或 AWS VPC。
- **客户/采购证据与阶段**：
  - **D：产品页及厂商汇总**：Guardian 产品页自称部署于全球执法机构，并列聚合机构数；没有读到能确定 Guardian Investigate AI 模块已被哪家警方采购的具名文件。 [CEL03] [CEL04]
  - **A：政府已签合同，但只覆盖相邻 Inseyets 等取证产品**：英国 Leicestershire PCC 的 2025/S 000-016210 为已签 Digital Forensics Software Renewal，供应商 CELLEBRITE UK LIMITED，列表含 Inseyets On-Prem Pro / Online Pro / PA Stand Alone。2025-03-31 签署，合同期 2025-04-01—2026-03-31。可证明取证产品真实采购与替换成本；不能证明 Genesis、Guardian Investigate 或 Pathfinder 在此采购内。 [GOV11]
- **未核实**：Guardian Investigate 专属客户/合同；生成报告的断言级引用与版本留痕；FedRAMP/CJIS 主张对应的确切产品、区域与功能边界；Pathfinder 的本轮具名采购证据。
- **正文读取**：是：Guardian、Investigate、Pathfinder 与政府合同正文。Inseyets 独立产品页未读到可用正文，角色由 Guardian 集成说明和政府合同交叉确认。
- **来源链接**：[CEL03](https://cellebrite.com/en/products/guardian/)；[CEL04](https://cellebrite.com/en/products/guardian/guardian-investigate/)；[CEL02](https://cellebrite.com/en/products/pathfinder/)；[GOV11](https://find-tender.service.gov.uk/Notice/016210-2025)；[CEL01](https://cellebrite.com/en/products/cellebrite-genesis/)。

### P03｜Magnet AI / Magnet Review Intelligent Insights（区别于历史 Magnet.AI）

- **厂商/地区**：Magnet Forensics；加拿大（官方 Nashville 稿的检索正文署名 Waterloo, Ontario；当前新AI稿在美国 Nashville 发布）；早期区域为美国/英国。
- **定位**：直接竞品：证据检索、引用型摘要与多分析 Agent 工作流；取证生态相邻。
- **核心功能**：
  - Magnet AI 是生态中的 AI intelligence engine，不是所有老产品统一改名。
  - Review 的 Intelligent Insights 提供自然语言结构化调查摘要、关键发现和后续分析建议。
  - 基于 LLM 与 agentic workflow 分析关系、时间线和模式；Citation Verification；产生线索而非结论。
- **目标工作流重合**：
  - **卷宗摘要**：明确：structured investigative summaries。
  - **时间线**：明确：Intelligent Insights 分析 timelines；Review 有 Timeline 视图。
  - **关系图**：部分：关系分析明确；本轮页面没有充分证实 Insights 原生关系图编辑器。
  - **矛盾检查**：未见明确专属能力；模式分析不等于证言矛盾检查。
  - **证据引用**：明确：verifiable citations linked directly to source evidence / Citation Verification。
- **部署/可用性**：2026-04-21 官方发布 Magnet AI / Intelligent Insights。当前 Review 产品页明确“Intelligent Insights early access is available in the U.S. and UK regions”，不能把发布稿的 available 写成全球全面正式开放。本轮未确认 Review 新 AI 的私有化/完全离线部署与模型数据驻留。
- **客户/采购证据与阶段**：
  - **B：历史 AI 具名客户**：Greensboro Police Department 的官方案例 PDF 中，Matthew Kraft 说明使用 AXIOM 内历史 Magnet.AI 预标注图像。不能当作 2026 年 Review Intelligent Insights 已落地的证据。 [MAG03]
  - **B：相邻自动化产品具名客户**：2023-02-27 官方发布 Metro Nashville PD 使用 Magnet AUTOMATE 消除设备积压；这是取证任务编排，不是生成式 Agent 已完成自动破案。 [MAG07]
  - **D：新 AI 能力发布/早期开放**：本轮未拿到具名警局自己的 Intelligent Insights 上线公告或采购合同。 [MAG02] [MAG04]
- **未核实**：Intelligent Insights 实际客户、采购与长期生产规模；云/内网/离线部署和中文支持；引用粒度及外部独立测试。
- **正文读取**：是：官方产品/发布正文与历史案例 PDF 提取文本；部分页面抽取省略，未看视频、未实测。
- **来源链接**：[MAG01](https://www.magnetforensics.com/magnet-ai/)；[MAG02](https://www.magnetforensics.com/news/magnet-forensics-unveils-magnet-ai-advancing-the-next-era-of-digital-investigative-intelligence/)；[MAG04](https://www.magnetforensics.com/products/magnet-review/)；[MAG03](https://www.magnetforensics.com/wp-content/uploads/2022/08/MF_AXIOM_DVR-E_Greensboro_CaseStudy_8.5x11.pdf)；[MAG07](https://www.magnetforensics.com/news/metro-nashville-police-department-uses-magnet-automate-to-eliminate-months-long-device-backlog-in-days-accelerating-the-pursuit-of-justice/)。

### P04｜Palantir Gotham / Gotham Europa + AIP（不是单一开箱即用刑侦助手）

- **厂商/地区**：Palantir Technologies；美国；警方部署证据来自德国、采购争议证据来自英国。
- **定位**：平台型直接/上位竞品：数据整合、调查情报与可定制 AI 工作流。
- **核心功能**：
  - Gotham / Europa 提供调查情报与多源数据、第三方 AI/ML 集成；当前 Gotham 首页也强调国防场景，不能直接当成刑侦功能说明书。
  - AIP 提供 Ontology 上的 AI workflows、agents、AIP Logic、Chatbot Studio 与 Evals。
  - AIP 的治理、审计、权限与 lineage 是平台能力；每家警方使用了哪些 AIP 功能需另证。
- **目标工作流重合**：
  - **卷宗摘要**：部分/平台可构建：本轮未确认警方已用的具体卷宗摘要模板。
  - **时间线**：待验证：不能仅从 Gotham 品牌推断具体警局已启用 AI 时间线。
  - **关系图**：部分：政府证明多库数据关联，平台定位相符；本轮已读页面不足以确认警方具体图谱界面和自动关系认定。
  - **矛盾检查**：未见明确警方产品证据。
  - **证据引用**：部分：AIP 有 historical lineage / audit trails，不等同刑事证据断言级引用。
- **部署/可用性**：Europa 官网明确 hybrid hosting / 可选本地 AI 厂商。德国 Hessen 内政部 2025-09-11 正文说明 HessenData 服务器与分析数据在州数据中心，警方掌握数据，访问按角色并记录。它证明该本地部署真实存在，不证明其他国家的所有 AIP AI 能力都能离线。
- **客户/采购证据与阶段**：
  - **A：政府自述真实部署**：Hessen 内政部说明警方自 2017 年使用 HessenData，并提及 Palantir 的选型及其他德国州授标。该来源是政府对自身采购/部署的说明，不是本轮读到的原始授标合同；也未证实其使用生成式 AIP。 [PAL05]
  - **A：政府会议证明试点与被阻采购，非成功落地**：伦敦议会 2026-06-17 逐字稿第 5 页明确，拟采购系统并未处于使用中，另有 separate pilot；MOPAC 因流程/竞争性/性价比问题阻止拟议 UOA 采购。不能把拟议 Palantir 合同写成签约上线，也未明确该试点产品是 Gotham 还是 AIP。 [GOV12] [GOV13]
- **未核实**：具名警方的 Gotham/AIP 产品版本与 AI 功能映射；警方卷宗摘要、时间线、矛盾检查、逐条证据引用的实测；HessenData 与 Gotham 商用版本的本轮政府文件映射；英国拟议采购后续是否重新完成。
- **正文读取**：是：Gotham/Europa 官方页、AIP 文档、德国政府全文及英国会议 PDF；产品页部分抽取较短。
- **来源链接**：[PAL01](https://www.palantir.com/platforms/gotham/europa/)；[PAL03](https://www.palantir.com/platforms/gotham/)；[PAL06](https://www.palantir.com/docs/foundry/aip/overview/)；[PAL05](https://innen.hessen.de/presse/innenminister-zur-plenardebatte-ueber-die-plattform-hessendata)；[GOV12](https://www.london.gov.uk/about-us/londonassembly/meetings/documents/b31762/Minutes%20-%20Appendix%201%20-%20Transcript%20-%20QA%20with%20MOPAC%20Wednesday%2017-Jun-2026%2010.00%20Police%20and%20Crime%20Co.pdf?T=9)；[GOV13](https://london.gov.uk/who-we-are/what-london-assembly-does/london-assembly-work/london-assembly-publications/police-and-crime-committee-letter-tough-choices)。

### P05｜Siren Investigate / Siren AI plugin / K9 Companion

- **厂商/地区**：Siren；爱尔兰；本轮案例为匿名美国县级警长部门。
- **定位**：直接竞品：检索与知识图谱调查平台 + 图谱型 AI 助手。
- **核心功能**：
  - Investigate 前端 + Federate/Elasticsearch 后端，多数据集联结检索、关系图、Geo/Temporal 分析。
  - Siren AI plugin 接入多个 LLM；K9 Companion 对话、检索数据、解释与操作图谱，生成图谱报告。
  - 公开文档导航已有 Platform 16.0 / AI plugin 2.1；产品营销页面仍展示 Siren 14，不把营销文案当当前版本号。
- **目标工作流重合**：
  - **卷宗摘要**：部分：生成基于用户图谱的报告；对完整卷宗材料的逐份摘要需实测。
  - **时间线**：明确：Investigate 有 Geo/Temporal / time analysis；K9 自动生成案情时间线未单独验证。
  - **关系图**：明确：graph browser / link analysis；K9 可理解并操作图谱。
  - **矛盾检查**：未见明示；图模式异常不等于证言矛盾核查。
  - **证据引用**：部分：连接原始 records / record-as-relation 数据；K9 每条回答的精确来源引文未确认。
- **部署/可用性**：官方安装文档支持在 Investigate 实例安装插件；LLM 文档明确 OpenAI、Azure OpenAI、AWS Bedrock、OpenAI-compatible，并列 locally-hosted provider 示例。本地模型集成有公开证据，但不等于警方已验收全离线方案。K9 文档明确图谱节点/边数据会发送给配置的 LLM，私有模型/数据出域控制必须核对。
- **客户/采购证据与阶段**：
  - **C：厂商匿名实施案例**：Siren 详述一个美国县级 sheriff 部门把 16 个系统与 UFED 取证数据汇聚成单一检索入口；写 Since implementing，但没有机构名称、合同或案号。 [SIR02]
  - **D：K9 产品与技术文档**：技术文档证明 K9 是实际存在的插件能力，不证明上述匿名客户已采购 K9/生成式功能。未找到本轮政府采购文件。 [SIR06] [SIR07]
- **未核实**：K9 具名执法生产客户及采购；逐断言证据引用和矛盾检测；本地化部署、模型出口控制的客户验收证据。
- **正文读取**：是：产品、匿名案例与当前 AI/平台技术文档；旧营销链接 14.0 文档返回 404，改读文档实际导航中的 16.0/2.1。
- **来源链接**：[SIR01](https://siren.io/siren-investigate/)；[SIR02](https://siren.io/case-studies/disconnected-data-in-criminal-investigations/)；[SIR03](https://siren.io/law-enforcement-and-intelligence/)；[SIR06](https://docs.siren.io/siren-ai/2.1/siren-ai/c_introduction.html)；[SIR07](https://docs.siren.io/siren-ai/2.1/siren-ai/t_k9_chat_companion.html)；[SIR08](https://docs.siren.io/siren-ai/2.1/siren-ai/t_installing.html)；[SIR09](https://docs.siren.io/siren-ai/2.1/siren-ai/t_configuring_openai_compat.html)；[SIR10](https://docs.siren.io/siren-platform-user-guide/16.0/index.html)。

### P06｜i2 Analyst’s Notebook / iBase / Analysis Hub（未核实“i2 Copilot”正式产品）

- **厂商/地区**：i2 Group / Harris Computer；英国业务；2022 年进入加拿大 Harris / Constellation 集团；本轮案例加拿大。
- **定位**：相邻成熟竞品：情报关系图、时间分析、共享数据库；AI 化处于扩展。
- **核心功能**：
  - Analyst’s Notebook 对结构化/非结构化数据进行可视分析，实体、链接、事件、时间线、属性。
  - iBase / Analysis Hub 支持共享调查情报环境；案件图谱、汇报与跨团队协作。
  - 官网 Responsible AI 写 machine learning / natural language capabilities 与人工主导；未读到正式名为 Copilot 的已上线刑侦 Agent 证据。
- **目标工作流重合**：
  - **卷宗摘要**：部分：图表/情报产品与非结构化数据处理；LLM 全卷宗自动摘要未确认。
  - **时间线**：明确：timelines / temporal analysis。
  - **关系图**：明确：entities、links、network analysis。
  - **矛盾检查**：未确认自动化语义矛盾检查。
  - **证据引用**：部分：承载数据与图表，可人工核查；生成式答案逐条引文未确认。
- **部署/可用性**：Analyst’s Notebook 官网明确 desktop；具名客户案例写 iBase / Analysis Hub 通过 secure virtual desktops 访问自有基础设施，客户可自主部署。AI 页面说 wherever possible 在客户控制环境运行，是原则，非所有 AI 功能离线可用证明。
- **客户/采购证据与阶段**：
  - **B：厂商具名客户故事**：Ryan Prox 的官方故事明确 Vancouver Police Department 使用 Analyst’s Notebook / iBase，随后构建 British Columbia 共享 CRIME 数据仓库；是实际客户叙述，不是本轮政府合同。 [I202]
  - **D：AI 原则及产品说明**：未见具名警方采购“Copilot”或新生成式 Agent 的来源。i2 的传统部署不能等同最新 LLM 能力已被部署。 [I203] [I204]
- **未核实**：正式 Copilot 名称、GA/版本、客户证据；LLM 摘要/矛盾检查/引用粒度；本轮原始警方授标文件。
- **正文读取**：是：官方产品、所有权历史、AI原则和客户全文；未依赖旧“IBM i2”名称作为当前归属。
- **来源链接**：[I201](https://i2group.com/)；[I202](https://i2group.com/articles/transforming-intelligence-with-i2-ryans-story)；[I203](https://i2group.com/solutions/i2-analysts-notebook)；[I204](https://i2group.com/trust/responsible-ai)；[I205](https://i2group.com/about-i2)。

### P07｜DataWalk Graph + AI Investigations Platform

- **厂商/地区**：DataWalk S.A. / DataWalk Inc.；波兰/美国（公司页列 Wroclaw 与 Redwood City）。
- **定位**：直接/平台竞品：知识图谱、财务/刑事情报调查与 AI 摘要。
- **核心功能**：
  - 合并结构化/非结构化证据、知识图谱、本体、多跳/可视查询、关系图、资金流、报告与案件管理。
  - 执法页明确 LLM-generated summaries；匿名联邦警方案例写 GenAI 提取文本实体、转写音频、生成摘要。
  - 数据血缘、权限、可审计协作；不是自动定罪或可直接采信的 AI 证据。
- **目标工作流重合**：
  - **卷宗摘要**：明确：LLM summaries / transcription summary。
  - **时间线**：部分：事件/时空与关联分析平台有支撑；本轮没有足够正文锁定自动案情时间线输出形式。
  - **关系图**：明确：knowledge graph / link charts / flows。
  - **矛盾检查**：部分：anomalies / hypothesis testing；不等同证人陈述矛盾检查。
  - **证据引用**：部分：lineage / audit / reproducibility 明确；LLM 句句引用到原始页码/时码未确认。
- **部署/可用性**：官方强调客户对系统与数据的 full ownership/control，可自扩展；本轮未读到适用于警方新 AI 的完整云/本地/离线 SKU 清单。可购买 COTS 与支持服务。不能把公司国防页的 air-gapped 描述扩大到每项执法 AI。
- **客户/采购证据与阶段**：
  - **B：具名选择客户，但为厂商稿**：2019-10-16 厂商公告 Anderson（South Carolina）Police Department 选择 DataWalk；正文当时使用将来时 will use，不能证明当前仍在用或已启用生成式 AI。 [DAT07]
  - **B：厂商称真实 DOJ 延续合同**：2026-02-04 官方稿写 RII 获多年延续合同，DataWalk 自 2019 年为 DOJ MNF 的 SIFT 环境组件。本轮未找到对应政府授标原件，不升级为 A。 [DAT08]
  - **C：匿名欧洲联邦警方案例**：10-week project 写使用生成式 AI 做文本实体提取、音频转写/摘要；机构不具名，无法独立核实。 [DAT02]
  - **K：采购渠道，非客户已采购**：官网列 RII GSA、DOJ BPA、NASA SEWP、SLSA 等 vehicle。FBI/DEA/ATF 等“can utilize”只代表可能采购，不能写已全部使用；$500m 为更大 BPA 背景/上限，不是 DataWalk 订单价。 [DAT06]
- **未核实**：DOJ 延续授标原件与 DataWalk 金额份额；最新具名警方生成式 AI 生产部署；离线能力与断言级证据引用。
- **正文读取**：是：产品、执法页、公司地址、具名发布稿与匿名案例/vehicle 正文。
- **来源链接**：[DAT01](https://datawalk.com/industries/law-enforcement/)；[DAT02](https://datawalk.com/case-study-federal-police-agency/)；[DAT04](https://datawalk.com/company/)；[DAT06](https://datawalk.com/contract-vehicles/)；[DAT07](https://datawalk.com/anderson-police-department-selects-datawalk/)；[DAT08](https://datawalk.com/datawalk-retained-by-the-u-s-department-of-justice-to-power-landmark-financial-crime-investigations/)；[DAT09](https://datawalk.com/product/)。

### P08｜Penlink CoAnalyst / CoAnalyst for PLX

- **厂商/地区**：Penlink；美国（官方发布说明 headquartered in the U.S.）。
- **定位**：直接竞品：调查数据内嵌生成式/Agentic AI 助手。
- **核心功能**：
  - 语义搜索、自然语言查询、摘要、可视化、关系/模式和异常提示。
  - 2025-02-11 官方公布 Agentic AI 迭代；2026-04-30 文章写已嵌入 PLX 并 available now。
  - 强调 analyst-in-the-loop，AI 输出区别于源数据、透明与审计；不以泛用聊天工具替代刑侦判断。
- **目标工作流重合**：
  - **卷宗摘要**：明确：summarizations / detailed summaries。
  - **时间线**：明确文字主张：PLX CoAnalyst 可呈现 relationships、timelines、key details；可视化粒度未实测。
  - **关系图**：部分/明确主张：数据可视化、匿名案例 network diagrams；PLX UI 未实测。
  - **矛盾检查**：部分：anomaly detection；没有专门证言矛盾能力证据。
  - **证据引用**：部分：输出/源数据区分、auditability；逐答案 citation 回链尚未确认。
- **部署/可用性**：CoAnalyst for PLX 官方写 available now；本轮没有拿到 CoAnalyst 专属云/本地/完全离线部署文档，不能从 PLX 或其他 Penlink 产品的部署形态继承。2024-05-15 首发时间只有搜索线索，相关发布页访问受限，不作为已读正文的确认日期。
- **客户/采购证据与阶段**：
  - **C：无法独立核验的匿名案例**：2025-06-18 官网称三个 real-world examples，涵盖刑事调查，但没有机构、案号、执法机关自身发布或合同。只能按匿名厂商主张收录，不能据此宣称已在具名警局规模部署或可复现破案效果。 [PEN04]
  - **D：官方发布与产品可用性**：2025 Agentic 发布与 2026 PLX 集成是产品存在/可获得证据，不是政府客户采购证明。 [PEN02] [PEN03]
- **未核实**：具名机构 CoAnalyst 使用/采购；部署与数据驻留/中文能力；证据引用与矛盾分析的实际输出；2024 首发稿正文。
- **正文读取**：是：CoAnalyst 产品、2025 发布、2026 PLX 文章及匿名例子全文；2024 首发页未成功读正文。
- **来源链接**：[PEN01](https://www.penlink.com/platform/coanalyst/)；[PEN02](https://www.penlink.com/press-release/agentic-ai-for-digital-investigations/)；[PEN03](https://www.penlink.com/blog/coanalyst-plx-digital-evidence/)；[PEN04](https://www.penlink.com/blog/coanalyst-in-action/)。

### P09｜Axon Draft One

- **厂商/地区**：Axon；美国；本轮客户自述来自 Colorado 的 Arvada。
- **定位**：相邻产品：警情/现场报告写作助手，不是完整破案 Agent。
- **核心功能**：
  - 基于执法记录仪音频转写及警员补充上下文生成叙事报告草稿。
  - 人必须审阅、补填、签名，主管审批；可按事件/指控级别限制使用。
  - 并排核对原始视频/转写、AI 参与披露和使用事件审计。
- **目标工作流重合**：
  - **卷宗摘要**：部分：单次/多次现场记录的草稿，不等于全案卷宗摘要。
  - **时间线**：部分：叙事报告可描述先后顺序；未证明跨证据案情时间线分析器。
  - **关系图**：未见。
  - **矛盾检查**：未见。
  - **证据引用**：部分：源录音/转写可并排审阅与审计；不等于每条报告断言的证据引用。
- **部署/可用性**：产品与客户流程依赖 Axon 网络/证据系统，正文明确 audio 自动上传并转写；未见私有化/完全离线 Draft One。来源对原始 AI 草稿留存存在版本差异：产品页写不保存草稿本身的 event history，责任页写美国可选保留，须以实际地区/租户配置与合同核实，不能写“永不保存”或“全部默认保存”。
- **客户/采购证据与阶段**：
  - **A：政府客户自己说明使用**：Arvada 市政府官网明确警局 utilizes Draft One，并说自 2025-09 起所有警员可选使用，必须培训、审核签名；这是实际部署自述，不是本轮购买合同/金额。 [AXO04]
  - **B：厂商具名客户**：Lafayette PD 案例说明日常采用 Draft One 且警员审核编辑；时间节省为厂商案例陈述，不当作独立准确率/统一 ROI。 [AXO03]
  - **A：政府部门介绍与政策边界**：DOJ COPS Office 2025-01 文章介绍 Draft One 的音频驱动流程；它是政府出版资料，但不是合同。文中当时明确不解析视频视觉内容，不能据此假设新版本功能完全未变。 [AXO05]
- **未核实**：采购文件、实际费用与合同区域；草稿保留开关/时间及检方披露政策；中文、离线、多证据案情研判能力。
- **正文读取**：是：官方产品/责任页、客户案例、Arvada 政府正文、DOJ 已索引正文；DOJ 直接 HTTP 重读返回404，保留该访问限制。
- **来源链接**：[AXO01](https://www.axon.com/products/draft-one)；[AXO02](https://www.axon.com/responsibility/draft-one)；[AXO03](https://www.axon.com/resources/how-lafayette-pd-used-draft-one)；[AXO04](https://www.arvadaco.gov/1531/Axon-Draft-One)；[AXO05](https://cops.usdoj.gov/html/dispatch/01-2025/ai_reports.html)。

### P10｜Veritone Investigate / iDEMS（aiWARE 平台）

- **厂商/地区**：Veritone；美国；官网列总部 Irvine, California，另有英国/以色列/澳大利亚办公室。
- **定位**：相邻/平台竞品：多模态数字证据管理、AI 索引与跨系统整合。
- **核心功能**：
  - Investigate 为证据管理与分析 hub；iDEMS 是多个公共部门 AI 应用的组合，不能把所有子模块都叫 Investigate Agent。
  - 开放架构摄取第三方证据、AI 处理、索引、关联、音视频资料检索与共享。
  - aiWARE 编排认知与生成式模型；本调研只比较证据整理/分析，不展开身份识别或跟踪子模块。
- **目标工作流重合**：
  - **卷宗摘要**：部分：认知/生成式处理明确；本轮没有足够具体证据证明全案卷宗摘要界面。
  - **时间线**：未核实 Investigate 专属案情时间线；其他子模块有时间关联不移植为此产品功能。
  - **关系图**：部分：correlated/analyzed 主张；原生刑事情报关系图未证。
  - **矛盾检查**：未见。
  - **证据引用**：部分：证据摄取/管理与索引；生成式回答逐条 citations 未证。
- **部署/可用性**：官方新闻称 iDEMS 支持 secure clouds 与 on-premises systems；2025-04-17 稿写可放客户 public cloud tenant 或 secure data center。这是产品部署声明，不是所列每种模型均离线可用或中国公安合规证明。
- **客户/采购证据与阶段**：
  - **K：采购资格/渠道，非实际订单**：2025-04-17 官方稿称 Investigate 获 DoD Tradewinds “Awardable” 状态。等于可被采购/评审状态，不等于 DoD 已授予 Investigate 订单；本轮未独立打开 marketplace 验证。 [VER04]
  - **D：具名官员表达潜在收益，不能当客户上线**：iDEMS 集成稿引用 Beverly Hills Police Chief 的句子为“would benefit from”，是潜在价值表达；这段不能证明 BHPD 已部署/采购 Investigate 或 iDEMS。 [VER05]
- **未核实**：具名 Investigate/iDEMS 警方部署与原始采购合同；实际多模态/引用/关系图输出与模型离线清单；Tradewinds 条目/订单原件；“10.09.2024”发布日期字符串的日期顺序。
- **正文读取**：是：官方产品、公共部门页、集成/marketplace 发布与公司页；不把仅 RIPA/Contact 或其他子模块的采购当 iDEMS 证据。
- **来源链接**：[VER01](https://www.veritone.com/applications/investigate/)；[VER02](https://www.veritone.com/industries/state-local-government/)；[VER04](https://www.veritone.com/newsroom/press-releases/tradewinds-investigate/)；[VER05](https://www.veritone.com/newsroom/press-releases/idems-data-integrations/)；[VER06](https://www.veritone.com/about-us/)。

## 采购证据与产品边界

### 已签合同，不等于同品牌新AI模块采购

英国Leicestershire的**Digital Forensics Software Renewal for Cellebrite Software（2025/S 000-016210）**为取证产品续约，清单含Inseyets On-Prem Pro、Online Pro、PA Stand Alone等，供应商CELLEBRITE UK LIMITED。2025-03-31签署，合同期2025-04-01—2026-03-31。[GOV11]

正文总值**£273,906.58未税 / £328,687.90含税**。这是多取证产品组合的历史合同价，不是Genesis/Guardian Investigate/Pathfinder报价，更不是标准单席位价。采购说明写工具已嵌入SOP/工作指引，替换涉及再认可、培训和管理成本；可参考To G集成/迁移策略，不能据此声称中国公安资质。[GOV11]

### 政府自述部署与被阻采购

- Hessen内政部2025-09-11说明警方自2017年用HessenData，服务器/分析数据在本州安全数据中心，有权限/访问记录与抽查；证明平台部署，不证明生成式AIP。[PAL05]
- Arvada政府确认警局在用Draft One，自2025-09警员可选使用，经培训审核签名；未取得采购合同/金额。[AXO04]
- 伦敦议会2026-06-17逐字稿第5页明确拟采购系统没有在用，另有separate pilot；拟议UOA采购因流程和性价比问题受阻。软件属于Gotham/AIP、后续是否重启成交仍未核实，不写成成功中标上线。[GOV12][GOV13]

### Procurement vehicle / Awardable 不等于订单

DataWalk官网的GSA、DOJ BPA、SEWP、SLSA是通道；FBI/DEA“can utilize”不是全部已用，更大的$500m BPA不是DataWalk订单收入。2026 DOJ延续项目只有厂商公告，仍为B而非政府原始合同A。[DAT06][DAT08]

Veritone Investigate的Tradewinds Awardable是可采购资格，本轮未查到订单原件；Beverly Hills警长的would benefit是潜在价值表态，不是已部署。[VER04][VER05]

## 对拟做中文To G刑侦助手的含义（分析判断）

1. **材料级闭环**：合法材料/取证导出/转写导入→摘要、时间线、关系→每个断言定位到证据页/段/时码→人工复核→有版本的输出。“Agent”标签不能代替验收项。
2. **矛盾单独验收**：区分来源冲突、时间差、OCR/转写错误、主观陈述差异与推论冲突；给双方证据引用和待核查说明，不自动判断谁说谎。Genesis/Guardian已有公开矛盾主张，关键词并非独有。[CEL01][CEL04]
3. **部署逐模块核对**：每个模型、API、索引与备份写清出域情况；Pathfinder的本地、K9本地模型或某个Palantir客户本地方案不能代证其他AI模块。[CEL02][SIR09][PAL05]
4. **留痕优先于流畅**：不覆盖原证据，保留草稿/修订、模型版本、操作者、检索上下文与反证。Draft One页面对草稿保留不同的表述是具体版本/政策验收点。[AXO01][AXO02]
5. **专业工作流差异化**：中文卷宗结构、权限、鉴定边界、无证据拒答、证据强度分层、反向假设与可撤销人工标注、既有系统接入，都需刑警/法务参与验证；本轮未认定市场空白或法定合规。

## 未核实与访问限制
- 本轮检索非穷尽市场盘点：主搜索覆盖9个候选厂商与政府采购维度，补查5次未覆盖的官方采购/部署，另用已发现链接读正文；没有产品试用、登录验证或客户访谈。
- 部分站点触发403/CloudFront地理限制、反爬或正文抽取服务429；改用浏览器DOM/直接HTTP/官方技术文档。共享浏览器曾回到无关域名，已按目标域名及路径剔除，不纳入证据。
- 英国公共采购搜索页面GET/POST返回的关键词过滤不可靠（输入未保留/返回无关全部结果），故未用“0条”或返回总量判断该厂商无采购。最终只采用能读到准确目标正文的 notice。
- 部分抽取文本被服务省略；来源逐项标明。Magnet Greensboro PDF 的抽取标题误称 Kerr County，正文明确Greensboro，本报告采用正文，不混淆客户。
- 没有取得 Genesis、Guardian Investigate、Intelligent Insights、K9、CoAnalyst 的政府授标原件。传统工具真实采购不证明最新生成式模块已验收。
- 本轮没有核实中国采购可用性、公安资质、国产操作系统/数据库/密码适配、信创、涉密/等保认证、中文手写/OCR及检察/法院采信；国外CJIS/FedRAMP声明不能直接替代。
- 没有独立准确率、幻觉率、矛盾检出率、证据引用准确率或标准报价；厂商快多少、破案率多少等陈述不作对比基准。
- AI只作为整理、检索、假设/线索生成助手；输出按辅助草稿处理，不自动具有新证据、鉴定结论或证言的地位，也不作为自动定罪依据。所有关键断言回到原始材料并由有资质人员复核。

## 来源登记：URL、日期、关键摘录、是否读到正文

英文/德文仅作为原文留证，中文释义与结论为主；没有发布日期就保持未知，不从页脚年份或图片路径推测。原文留档用于核查，不意味着版权转授。

### [AXO01] Draft One - Axon

- **URL**：https://www.axon.com/products/draft-one
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：Review your draft alongside the original footage and transcript, all in one view, to quickly verify details.
  - **中文释义**：支持并排看原始记录与转写核对草稿，而不是无审核提交。
- **关键原文**：without storing the draft itself.
  - **中文释义**：该产品页对草稿留存的表述与责任页可选保留说法不一致，需要区域/版本核对。
- **关联条目**：P09。

### [AXO02] Draft One - Axon.com

- **URL**：https://www.axon.com/responsibility/draft-one
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：agencies can optionally retain AI-generated drafts for additional auditing and oversight.
  - **中文释义**：责任页面写可选保留 AI 草稿，与产品页旧留存表述需要按租户版本进一步核对。
- **关联条目**：P09。

### [AXO03] How Lafayette PD used Draft One to help officers spend more time in the community

- **URL**：https://www.axon.com/resources/how-lafayette-pd-used-draft-one
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商具名客户案例；B：厂商具名客户或合同发布（非独立合同原件）。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：After AI generates the narrative, the officer is required to review, edit and approve the final report.
  - **中文释义**：Lafayette 案例也要求警员审阅、编辑并批准最终报告。
- **关联条目**：P09。

### [AXO04] Axon Draft One | Arvada, CO

- **URL**：https://www.arvadaco.gov/1531/Axon-Draft-One
- **日期**：未见可确认发布日期；使用时点 As of September 2025；客户页面无发布日期；2025-09 仅为正文描述的使用时点。
- **来源/层级**：政府合同/会议/客户公开资料；A：政府原始材料。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：The Arvada Police Department utilizes Axon Draft One
  - **中文释义**：Arvada 政府官网自行确认实际使用，强于厂商 Demo。
- **关联条目**：P09。

### [AXO05] Using AI to Write Police Reports

- **URL**：https://cops.usdoj.gov/html/dispatch/01-2025/ai_reports.html
- **日期**：2025-01；政府期刊正文 January 2025 | Volume 18 | Issue 1；未猜具体日。
- **来源/层级**：政府合同/会议/客户公开资料；A：政府原始材料。
- **是否读到正文**：是（web_extract）；已读检索/抽取服务返回的政府正文，内容在人员访谈处截断；直接 HTTP 复读返回404。保留来源与访问方式，不假装完整全文或当前版本政策。
- **关键原文**：The AI tools are not able to parse or summarize the video’s visual content.
  - **中文释义**：2025-01 DOJ 介绍当时版本为音频驱动，不能当完整多模态卷宗 Agent。
- **关联条目**：P09。

### [CEL01] Cellebrite Genesis - Agentic AI for Investigations

- **URL**：https://cellebrite.com/en/products/cellebrite-genesis/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：Question the evidence in plain language to uncover relationships, timelines, entities, patterns, contradictions and cross-file connections.
  - **中文释义**：自然语言询问证据，发现关系、时间线、实体、模式、矛盾与跨文件连接。
- **关键原文**：Because Genesis is cloud-based, you can get started quickly without deploying infrastructure.
  - **中文释义**：Genesis 专属 FAQ 明确云产品形态。
- **关键原文**：Every response links back to source material
  - **中文释义**：官方主张每个回答回链源材料；未实测定位粒度。
- **关键原文**：No. Customer data is not used to train or improve models.
  - **中文释义**：厂商声明客户数据不用于模型训练或改进；仍需合同与技术验收。
- **关联条目**：P01, P02。

### [CEL02] Multi-Device Investigative Analytics Platform | Cellebrite

- **URL**：https://cellebrite.com/en/products/pathfinder/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：It can be deployed on-premise — as a virtual machine or physical server — or in the cloud via AWS VPC.
  - **中文释义**：Pathfinder 明确可部署在本地虚拟机/实体服务器或 AWS VPC；此证明不适用于 Genesis。
- **关联条目**：P02。

### [CEL03] Digital Evidence Management Software | Cellebrite

- **URL**：https://cellebrite.com/en/products/guardian/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：Guardian integrates natively with Cellebrite Inseyets (UFED and Physical Analyzer).
  - **中文释义**：Guardian 与 Inseyets（UFED 和 Physical Analyzer）原生集成；角色是取证数据输入而非同一个 AI 助手。
- **关键原文**：Guardian is cloud-native digital evidence management software built for investigations.
  - **中文释义**：Guardian 本体是云原生数字证据管理，不是移动端提取工具。
- **关键原文**：Guardian Collaborate is available
  - **中文释义**：FedRAMP 说明作用于 Guardian Collaborate 特定联邦环境，不能扩张到全套产品。
- **关联条目**：P02。

### [CEL04] Guardian Investigate: AI Investigation Management - Cellebrite

- **URL**：https://cellebrite.com/en/products/guardian/guardian-investigate/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：Guardian Investigate empowers teams to manage high-profile incidents, major crimes and cold cases so they can quickly review evidence, summarize documents, spot inconsistencies and connect the dots.
  - **中文释义**：Guardian Investigate 支持证据审阅、文档摘要与不一致提示，覆盖重大案/冷案调查管理。
- **关键原文**：Guardian Investigate provides a secure, cloud-based investigation management solution
  - **中文释义**：Investigate 明确为云端调查管理。
- **关键原文**：Create a timeline of case details and relevant evidence
  - **中文释义**：明确时间线能力。
- **关联条目**：P02。

### [CEL05] The New Age of Investigations: Cellebrite’s Journey to Genesis

- **URL**：https://cellebrite.com/en/blog/the-new-age-of-investigations-cellebrites-journey-to-genesis/
- **日期**：未见可确认发布日期；正文产品阶段日期，不等于该文章初发日期。
- **来源/层级**：厂商具名客户案例；B：厂商具名客户或合同发布（非独立合同原件）。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：– Lt. Jim Hill, Lab Director, Ocean County Prosecutor’s Office.
  - **中文释义**：具名客户来自 Ocean County 检察官办公室实验室；只能认定为厂商刊载的客户证言。
- **关键原文**：first introduced in early access in March 2026
  - **中文释义**：早期访问于2026年3月引入。
- **关键原文**：generally available
  - **中文释义**：同文说明于2026年6月进入一般可用；首发 early access 稿不应误当 GA。
- **关键原文**：Lt. Jerod K. Abshire of the Digital Forensics Unit with the Calcasieu Parish Sheriff’s Office.
  - **中文释义**：另一个具名案例来自 Calcasieu Parish 警长部门。
- **关联条目**：P01。

### [CEL06] Agentic AI for Digital Investigations

- **URL**：https://cellebrite.com/en/resources/press-releases/cellebrite-launches-genesis-agentic-ai-for-digital-investigations-cellebrite/
- **日期**：2026-03-16；官方发布稿正文 dateline；early access 日期。
- **来源/层级**：厂商发布稿；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：Availability:
  - **中文释义**：发布稿明确为 early access，不能只凭首发稿认定全面正式开放。
- **关联条目**：P01。

### [DAT01] Law Enforcement Intelligence Software powered by Graph and AI

- **URL**：https://datawalk.com/industries/law-enforcement/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：Leverage built-in automation and LLM-generated summaries to streamline reporting
  - **中文释义**：执法方案明确使用内置自动化和 LLM 生成摘要。
- **关联条目**：P07。

### [DAT02] Case Study: Federal Police Agency Sees Spectacular Results With DataWalk 10-Week Project

- **URL**：https://datawalk.com/case-study-federal-police-agency/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商匿名案例；C：匿名厂商案例。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：During the project, Generative AI has been used to extract entities from text, transcript audio files, and generate a short summary for transcription
  - **中文释义**：匿名警方案例明确 GenAI 用于文本实体提取、音频转写和摘要；这不是政府采购原件。
- **关联条目**：P07。

### [DAT04] DataWalk: Unified Graph + AI Investigations Platform for Financial Crime & Public Safety

- **URL**：https://datawalk.com/company/
- **日期**：2025-11-10；修改日期 2025-11-20；article:published_time 元数据；公司页内容可后续变动。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：The European Office
  - **中文释义**：公司正文列波兰 Wroclaw 的 DataWalk S.A. 及美国办公室，支撑地区归属。
- **关联条目**：P07。

### [DAT06] Contract Vehicles | DataWalk

- **URL**：https://datawalk.com/contract-vehicles/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；K：采购渠道/资格声明，非订单。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：All DOJ agencies including FBI, DEA, ATF, BOP, OJP and others can utilize this contract to procure analytical services and DataWalk products.
  - **中文释义**：可使用采购渠道不等于每个 DOJ 单位已购买 DataWalk。
- **关联条目**：P07。

### [DAT07] Anderson Police Department Selects DataWalk

- **URL**：https://datawalk.com/anderson-police-department-selects-datawalk/
- **日期**：2019-10-16；修改日期 2024-11-26；厂商正文与 article:published_time；不把 2024 元数据修改日期当新客户公告。
- **来源/层级**：厂商发布稿；B：厂商具名客户或合同发布（非独立合同原件）。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：Anderson (SC) Police Department has selected DataWalk
  - **中文释义**：具名 Anderson 警局选择 DataWalk 的厂商公告；不证明新生成式 AI 的当前使用。
- **关联条目**：P07。

### [DAT08] DataWalk Retained by the U.S. Department of Justice to Power Landmark Financial Crime Investigations

- **URL**：https://datawalk.com/datawalk-retained-by-the-u-s-department-of-justice-to-power-landmark-financial-crime-investigations/
- **日期**：2026-02-04；修改日期 2026-03-11；正文与 article:published_time。
- **来源/层级**：厂商发布稿；B：厂商具名客户或合同发布（非独立合同原件）。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：as part of a multi-year contract extension awarded to Research Innovations Incorporated (RII).
  - **中文释义**：2026 厂商稿声称 DOJ 项目主承包商 RII 获延续合同，尚缺政府授标原件。
- **关键原文**：Since 2019, RII has utilized DataWalk as a key component
  - **中文释义**：厂商把 DataWalk 描述为自2019年在 RII/DOJ SIFT 环境的组件；未独立查到政府授标原件。
- **关联条目**：P07。

### [DAT09] Product Overview | DataWalk

- **URL**：https://datawalk.com/product/
- **日期**：未见可确认发布日期；修改日期 2025-02-27；只有 article:modified_time，未见初次发布日期。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：Ensure full lineage,
  - **中文释义**：产品强调血缘、可解释、可复现和监控；尚不足以证明 LLM 每句话给出证据引用。
- **关联条目**：P07。

### [GOV11] Digital Forensics Software Renewal for Cellebrite Software

- **URL**：https://find-tender.service.gov.uk/Notice/016210-2025
- **日期**：2025-04-22；政府 notice 搜索索引可见 Published 22 April 2025, 12:28pm；抽取正文保留合同内容但省略页眉；合同签署日期为2025-03-31（不是发布日期）。
- **来源/层级**：政府合同/会议/客户公开资料；A：政府原始材料。
- **是否读到正文**：是（web_extract）；原始政府 notice 提取可读合同正文；直接 HTTP 曾403、PDF子路径404。政府页眉发布日期来自搜索索引，合同签署和条款由正文证实。
- **关键原文**：These tools are embedded within our Standard Operating Procedures and Working Instructions.
  - **中文释义**：Leicestershire 警方的正式合同说明既有 Cellebrite 取证工具已嵌入 SOP/工作指引，替换涉及再认可与培训。
- **关键原文**：x 5 Inseyets On-Prem Pro
  - **中文释义**：合同清单证明 Inseyets 取证产品具体采购。
- **关键原文**：£273,906.58 excluding VAT £328,687.90 including VAT
  - **中文释义**：整体多产品续约合同的金额，不是 Genesis 或单产品标准报价。
- **关键原文**：Date signed 31 March 2025
  - **中文释义**：已签合同，不是招标计划/试点。
- **关联条目**：P02。

### [GOV12] (Public Pack)Minutes - Appendix 1 - Transcript - Q&A with MOPAC Minutes Supplement  for Police and Crime Committee, 17/06/2026 10:00

- **URL**：https://www.london.gov.uk/about-us/londonassembly/meetings/documents/b31762/Minutes%20-%20Appendix%201%20-%20Transcript%20-%20QA%20with%20MOPAC%20Wednesday%2017-Jun-2026%2010.00%20Police%20and%20Crime%20Co.pdf?T=9
- **日期**：未见可确认发布日期；文档/会议日期 2026-06-17；PDF 逐字稿首页会议日期；未把会议日期当上网发布日期。
- **来源/层级**：政府合同/会议/客户公开资料；A：政府原始材料。
- **是否读到正文**：是（web_extract）；已阅读含 Palantir 采购问题的 PDF 前段（含第1—7页）；抽取文本其余部分有省略，对非 Palantir 议程不作结论。
- **关键原文**：there is no system in line with the procurement that was coming forward in current use.
  - **中文释义**：伦敦政府逐字稿明确拟议采购对应系统没有在用；下一段区分已有单独 pilot。
- **关键原文**：OK, because that is a separate pilot.
  - **中文释义**：议会逐字稿第5页区分另一个试点，不是拟议大合同系统已在用。
- **关联条目**：P04。

### [GOV13] Police and Crime Committee Letter on tough choices

- **URL**：https://london.gov.uk/who-we-are/what-london-assembly-does/london-assembly-work/london-assembly-publications/police-and-crime-committee-letter-tough-choices
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：政府合同/会议/客户公开资料；A：政府原始材料。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：following MOPAC's blocking of the Palantir contract
  - **中文释义**：政府页面确认采购受阻，不能把拟议合同列为成功落地。
- **关联条目**：P04。

### [I201] i2 Group | Link analysis software | Discover, create & exploit actionable intelligence

- **URL**：https://i2group.com/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（browser-dom）；已读返回正文；不是登录后产品实测。
- **关键原文**：i2® Analyst's Notebook®
  - **中文释义**：官网仍明确 Analyst’s Notebook 系列，不应杜撰正式 Copilot 名称。
- **关联条目**：P06。

### [I202] Transforming intelligence with i2: Ryan’s story | i2 Group

- **URL**：https://i2group.com/articles/transforming-intelligence-with-i2-ryans-story
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商具名客户案例；B：厂商具名客户或合同发布（非独立合同原件）。
- **是否读到正文**：是（browser-dom）；已读返回正文；不是登录后产品实测。
- **关键原文**：access their own data and the province‑wide repository via secure virtual desktops
  - **中文释义**：具名客户故事说明自有数据和省级仓库通过安全虚拟桌面访问。
- **关联条目**：P06。

### [I203] i2 Analyst's Notebook - Discover and deliver actionable intelligence | i2

- **URL**：https://i2group.com/solutions/i2-analysts-notebook
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：Model and visualize
  - **中文释义**：官方产品对实体、链接、事件与时间线建模/可视化；它是传统可视分析竞品。
- **关联条目**：P06。

### [I204] Responsible AI | i2 Group

- **URL**：https://i2group.com/trust/responsible-ai
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：官方技术/治理文档；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：Today, we are extending this foundation with machine learning and natural language capabilities, developed in close collaboration with our customers.
  - **中文释义**：官网说明正扩展机器学习/自然语言能力；不能据此断言一个具名 Copilot 已正式销售。
- **关键原文**：AI supports analysis. It does not replace human judgement.
  - **中文释义**：AI 辅助分析，不替代人类判断。
- **关联条目**：P06。

### [I205] About Us | i2 Group

- **URL**：https://i2group.com/about-i2
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：In January 2022, i2 entered a new chapter when it became part of
  - **中文释义**：现属 Harris Computer / Constellation；不要继续把 IBM 当当前厂商。
- **关联条目**：P06。

### [MAG01] Magnet AI for Digital Forensics | Magnet Forensics

- **URL**：https://www.magnetforensics.com/magnet-ai/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：Every AI-generated insight remains grounded in verifiable evidence with built-in citation verification
  - **中文释义**：厂商明确声明 AI 洞见基于可验证证据，并内置引用验证。
- **关联条目**：P03。

### [MAG02] Magnet Forensics Unveils Magnet AI for Investigations

- **URL**：https://www.magnetforensics.com/news/magnet-forensics-unveils-magnet-ai-advancing-the-next-era-of-digital-investigative-intelligence/
- **日期**：2026-04-21；官方发布稿正文 dateline。
- **来源/层级**：厂商发布稿；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：It generates investigative leads — not conclusions — leaving investigative verification, analysis, and decision making firmly in the hands of human judgment.
  - **中文释义**：产生调查线索而非结论，验证、分析和决策仍由人负责。
- **关键原文**：all grounded in verifiable citations linked directly to the source evidence.
  - **中文释义**：结构化调查摘要带可验证引用，链接源证据。
- **关联条目**：P03。

### [MAG03] Magnet ATLAS Case Study - Kerr County

- **URL**：https://www.magnetforensics.com/wp-content/uploads/2022/08/MF_AXIOM_DVR-E_Greensboro_CaseStudy_8.5x11.pdf
- **日期**：未见可确认发布日期；可见文本 PDF URL 含 /2022/08/；搜索索引全文有 © 2022；不是已确认发布日期；不从 URL 或版权年份推断发布日期。
- **来源/层级**：厂商具名客户案例；B：厂商具名客户或合同发布（非独立合同原件）。
- **是否读到正文**：是（web_extract）；抽取服务返回标题 Magnet ATLAS Case Study - Kerr County，与 PDF 文件名/正文的 Greensboro 内容不一致；只采用正文明确的机构/产品，不采用错误标题归属；PDF 部分正文被服务省略。
- **关键原文**：pre-tagging images using Magnet.AI is the number one feature in AXIOM that accelerates his investigative process
  - **中文释义**：Greensboro 案例里的 Magnet.AI 是 AXIOM 的历史图像预标注能力，不证明新 Intelligent Insights 已部署。
- **关联条目**：P03。

### [MAG04] Magnet Review

- **URL**：https://www.magnetforensics.com/products/magnet-review/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；当前产品页明确 early access 与地区限制，权重高于泛化发布稿 available。直接访问曾触发 Client Challenge；成功抽取的正文可读。
- **关键原文**：Intelligent Insights early access is available in the U.S. and UK regions.
  - **中文释义**：当前产品页限定 Intelligent Insights 早期开放为美国和英国区域。
- **关联条目**：P03。

### [MAG07] Metro Nashville Police Department Uses Magnet AUTOMATE to Eliminate Months-Long Device Backlog in Days, Accelerating the Pursuit of Justice - Magnet Forensics

- **URL**：https://www.magnetforensics.com/news/metro-nashville-police-department-uses-magnet-automate-to-eliminate-months-long-device-backlog-in-days-accelerating-the-pursuit-of-justice/
- **日期**：2023-02-27；官方新闻页面可见 February 27, 2023。
- **来源/层级**：厂商发布稿；B：厂商具名客户或合同发布（非独立合同原件）。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：forensics unit completely eliminated a months-long violent crimes case backlog
  - **中文释义**：具名 Nashville 客户的证据只覆盖 AUTOMATE 取证编排，非自动破案 Agent。
- **关联条目**：P03。

### [PAL01] Palantir Gotham Europa

- **URL**：https://www.palantir.com/platforms/gotham/europa/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：Organisations can adopt hybrid hosting solutions and plug in preferred local AI vendors at the place where each vendor can deliver the most value.
  - **中文释义**：Gotham Europa 的官方部署声明含混合托管与可选本地 AI 厂商。
- **关联条目**：P04。

### [PAL03] Gotham | Palantir

- **URL**：https://www.palantir.com/platforms/gotham/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；官网当前以国防/全球决策展示为主，不能从军事能力反推警方刑侦产品特性。
- **关键原文**：The Operating System for Global Decision Making.
  - **中文释义**：当前 Gotham 页面重点为全球决策/国防，不应由首页泛化出完整刑侦助手功能。
- **关联条目**：P04。

### [PAL05] Innenminister zur Plenardebatte über die Plattform HessenData | Hessen Innen

- **URL**：https://innen.hessen.de/presse/innenminister-zur-plenardebatte-ueber-die-plattform-hessendata
- **日期**：2025-09-11；政府页面正文与 time datetime。
- **来源/层级**：政府合同/会议/客户公开资料；A：政府原始材料。
- **是否读到正文**：是（requests-beautifulsoup）；已读完整政府正文；部署/数据安全与采购论点是内政部门自述，不等于独立安全评估。
- **关键原文**：Die Server und die Analysedaten befinden sich in gesicherten Rechenzentren der Hessischen Zentrale für Datenverarbeitung.
  - **中文释义**：德国 Hessen 内政部明确：服务器及分析数据位于该州中央数据处理机构的安全数据中心。
- **关联条目**：P04。

### [PAL06] Overview • AIP • Palantir

- **URL**：https://www.palantir.com/docs/foundry/aip/overview/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：官方技术/治理文档；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：AIP's builder tools like AIP Logic, AIP Chatbot Studio (formerly known as AIP Agent Studio), and AIP Evals enable the development of production-ready AI-powered workflows, agents, and functions on top of the Ontology and developer toolchain.
  - **中文释义**：AIP 可在 Ontology 上构建工作流和 Agent；文档中的正式名称为 Chatbot Studio，原称 Agent Studio。
- **关联条目**：P04。

### [PEN01] CoAnalyst: Generative AI for Digital Investigations | Penlink

- **URL**：https://www.penlink.com/platform/coanalyst/
- **日期**：未见可确认发布日期；修改日期 2026-04-14；article:modified_time，仅为改动时间。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：From semantic search and summarizations to anomalies detection and pattern recognition
  - **中文释义**：CoAnalyst 官方列语义搜索、摘要、异常与模式识别。
- **关联条目**：P08。

### [PEN02] Penlink Unveils the Next Evolution of CoAnalyst: Agentic AI for Digital Investigations

- **URL**：https://www.penlink.com/press-release/agentic-ai-for-digital-investigations/
- **日期**：2025-02-11；Date Posted: February 11th, 2025。
- **来源/层级**：厂商发布稿；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：CoAnalyst automates complex investigative workflows
  - **中文释义**：2025 官方宣布 Agentic 迭代，但不是具名警方验收证据。
- **关联条目**：P08。

### [PEN03] CoAnalyst for PLX: Turning Digital Evidence into Decisive Action

- **URL**：https://www.penlink.com/blog/coanalyst-plx-digital-evidence/
- **日期**：2026-04-30；Date Posted: April 30th, 2026。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：Outputs are clearly distinguished from source data, and workflows are designed to support transparency, auditability, and defensibility.
  - **中文释义**：厂商说明 AI 输出与源数据区分、支持透明和审计；精确引用回链粒度未证。
- **关键原文**：CoAnalyst for PLX
  - **中文释义**：2026文章确认 PLX 内嵌版本存在，仍需验收具体功能。
- **关键原文**：is available now.
  - **中文释义**：厂商声明可获得；不是客户采购证明。
- **关联条目**：P08。

### [PEN04] CoAnalyst in Action: Real-World Examples of AI-Powered Investigations | Blog | Penlink

- **URL**：https://www.penlink.com/blog/coanalyst-in-action/
- **日期**：2025-06-18；修改日期 2026-05-28；正文 Date Posted 与 article:published_time。
- **来源/层级**：厂商匿名案例；C：匿名厂商案例。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：Below are three real-world examples of how CoAnalyst has helped investigative teams move cases forward.
  - **中文释义**：厂商声称真实例子，但正文未具名机构/案号，不能当可独立核实的落地。
- **关联条目**：P08。

### [SIR01] SIREN INVESTIGATE - SIREN

- **URL**：https://siren.io/siren-investigate/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：Geo/Temporal analysis for multi-layer, interactive maps and time analysis.
  - **中文释义**：Siren Investigate 支持地理/时间分析；不能自动等同 K9 完整卷宗时间线。
- **关联条目**：P05。

### [SIR02] Case Study: Disconnected data in Criminal Investigations - SIREN

- **URL**：https://siren.io/case-studies/disconnected-data-in-criminal-investigations/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商匿名案例；C：匿名厂商案例。
- **是否读到正文**：是（browser-dom）；浏览器首个共享会话曾发生域名不匹配，数据丢弃；隔离会话确认 siren.io 的准确目标URL后重新读正文。
- **关键原文**：A busy US county sheriff’s department’s serious crime and policing intelligence team
  - **中文释义**：实施案例没有县名/机构名称，因此仅列匿名厂商案例。
- **关联条目**：P05。

### [SIR03] Law Enforcement and Intelligence Industry- SIREN

- **URL**：https://siren.io/law-enforcement-and-intelligence/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（browser-dom）；已读返回正文；不是登录后产品实测。
- **关键原文**：integrated capabilities including search & data discovery, analytics, big data monitoring, and advanced link analysis.
  - **中文释义**：执法方案提供搜索、数据发现、分析与关系分析。
- **关联条目**：P05。

### [SIR06] Siren AI plugin for Investigate :: SIREN DOCS

- **URL**：https://docs.siren.io/siren-ai/2.1/siren-ai/c_introduction.html
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：官方技术/治理文档；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；真实可安装插件与API文档，不是本轮实际产品测试；仅证实产品能力描述。
- **关键原文**：K9 Companion: AI chat assistant enabling intelligent, context-aware conversations by leveraging the configured LLM provider.
  - **中文释义**：K9 是 Siren AI 插件内的对话助手，接入配置的 LLM。
- **关联条目**：P05。

### [SIR07] K9 Companion :: SIREN DOCS

- **URL**：https://docs.siren.io/siren-ai/2.1/siren-ai/t_k9_chat_companion.html
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：官方技术/治理文档；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：the graph data is automatically attached to the conversation.
  - **中文释义**：在图谱内使用 K9 时图谱数据会附入会话；必须核对其实际模型服务与数据出域。
- **关键原文**：The data sent to the LLM consists of the graph name, nodes, edges and groups.
  - **中文释义**：文档明确模型接收图谱名字、节点、边与组；数据出域是采购验收点。
- **关联条目**：P05。

### [SIR08] Installing the Siren AI plugin :: SIREN DOCS

- **URL**：https://docs.siren.io/siren-ai/2.1/siren-ai/t_installing.html
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：官方技术/治理文档；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：The Siren AI plugin can be installed by downloading the plugin zip file and installing it using the Investigate CLI.
  - **中文释义**：公开文档描述可安装的插件，不是只有营销 Demo；本调研不提供调查操作教程。
- **关联条目**：P05。

### [SIR09] OpenAI compatible configuration :: SIREN DOCS

- **URL**：https://docs.siren.io/siren-ai/2.1/siren-ai/t_configuring_openai_compat.html
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：官方技术/治理文档；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：Examples of providers that use this API spec include Ollama, llama.cpp, vLLM, TensorRT-LLM, Scaleway, and more.
  - **中文释义**：公开文档支持 OpenAI-compatible 模型接口，并明确本地模型服务示例。
- **关联条目**：P05。

### [SIR10] Introduction to Siren Platform :: SIREN DOCS

- **URL**：https://docs.siren.io/siren-platform-user-guide/16.0/index.html
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：官方技术/治理文档；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：It consists of the user interface component,
  - **中文释义**：当前平台文档确认 Investigate 前端和 Federate 后端；可与营销页的旧版本文案区别。
- **关联条目**：P05。

### [VER01] Investigate - Veritone

- **URL**：https://www.veritone.com/applications/investigate/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。
- **关键原文**：a single, secured, AI-powered hub
  - **中文释义**：Investigate 是安全 AI 证据处理 hub；并未据此核实完整破案 Agent。
- **关联条目**：P10。

### [VER02] AI for State & Local Government - Veritone

- **URL**：https://www.veritone.com/industries/state-local-government/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：Our solutions are cloud agnostic, FedRAMP Authorized, and support CJIS compliance.
  - **中文释义**：此为厂商公共部门组合声明；必须进一步核对具体产品/区域/认证原件，非中国公安资质。
- **关联条目**：P10。

### [VER04] Veritone Achieves “Awardable” Status on DoD’s Tradewinds Solutions Marketplace with AI-Powered Investigate Solution - Veritone

- **URL**：https://www.veritone.com/newsroom/press-releases/tradewinds-investigate/
- **日期**：2025-04-17；可见日期 04.17.2025，数字17排除日月另一解析。
- **来源/层级**：厂商发布稿；K：采购渠道/资格声明，非订单。
- **是否读到正文**：是（requests-beautifulsoup）；已读返回正文；不是登录后产品实测。
- **关键原文**：Veritone’s Investigate solution has been added to the Tradewinds Marketplace.
  - **中文释义**：加入采购 marketplace / Awardable 不是已拿到政府订单。
- **关键原文**：within their public cloud tenant or in their secure data center.
  - **中文释义**：官方稿描述客户云租户/安全数据中心部署。
- **关联条目**：P10。

### [VER05] Veritone Expands iDEMS Data Integrations to Enhance Public Safety and Law Enforcement Efficiency

- **URL**：https://www.veritone.com/newsroom/press-releases/idems-data-integrations/
- **日期**：未见可确认发布日期；可见文本 10.09.2024；新闻稿可见字符串，未凭此猜 10月9日/9月10日；保留原样。
- **来源/层级**：厂商发布稿；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（requests-beautifulsoup）；使用 HTTP 读到完整稿，修复初次抽取省略掉 would benefit 的客户引用；该语气不能作为实际部署证明。日期字符串10.09.2024保留不猜。
- **关键原文**：Beverly Hills PD would benefit from the ability to aggregate the data
  - **中文释义**：Beverly Hills 警长说“将受益”，不能写成已部署 iDEMS 的具名客户。
- **关键原文**：currently available on secure clouds – AWS Marketplace, Azure Marketplace and FedRAMP Marketplace – and for on-premises systems.
  - **中文释义**：厂商声明云端与本地部署；Marketplace 条目不等于实际订单或全模型离线。
- **关联条目**：P10。

### [VER06] About Us - Veritone

- **URL**：https://www.veritone.com/about-us/
- **日期**：未见可确认发布日期；本轮未见可确认的发布日期；不以页脚年份、图片路径或版本号推断。
- **来源/层级**：厂商产品/公司/行业页面；D：官方产品/技术文档/发布，不等于客户已部署。
- **是否读到正文**：是（web_extract）；已读返回正文；不是登录后产品实测。 抽取服务返回文本含省略标记。
- **关键原文**：Veritone’s headquarters are in Irvine, California,
  - **中文释义**：官网列美国总部和全球办公室，地区归属有正文依据。
- **关联条目**：P10。
