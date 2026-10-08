# 开源参考：不把底层组件误称为“完整刑侦Agent”

| 项目 | 可学习/复用的部分 | 不等于什么 | 官方来源 |
|---|---|---|---|
| Timesketch | 协作取证时间线、事件注释、评论/标签、时间线导入 | 不是完整中文卷宗分析助手；仓库明确不是官方Google产品 | [仓库](https://github.com/google/timesketch) / [官网](https://timesketch.org/) |
| Autopsy | 数字取证、对现有取证导出数据的组织思路 | 不是能自动定罪的AI；不自行重造设备提取 | [官网](https://www.autopsy.com/) / [许可](https://sleuthkit.org/autopsy/licenses.php) |
| PaddleOCR | 扫描件识别、结构化版面、文本/表格坐标 | 不保证手写/低质卷宗零错误 | [仓库](https://github.com/PaddlePaddle/PaddleOCR) |
| BGE-M3 | 中文/多语言向量与稀疏检索、混合检索基线 | 通用benchmark不等于本案证据支持度 | [模型卡](https://huggingface.co/BAAI/bge-m3/raw/main/README.md) |
| LangGraph | 持久任务、人审中断与恢复 | 不是越权防护或业务正确性保障 | [仓库](https://github.com/langchain-ai/langgraph) / [中断](https://docs.langchain.com/oss/python/langgraph/interrupts) |
| pgvector + PostgreSQL | 向量与业务数据集中、RLS防御 | 不自带高质量中文BM25/自动ACL，超级用户绕过RLS | [pgvector](https://github.com/pgvector/pgvector) / [RLS](https://www.postgresql.org/docs/current/ddl-rowsecurity.html) |
| PDF.js / Cytoscape.js | 原页查看、点击引用、关系图渲染 | 图中出现关联不证明共犯或违法 | [PDF.js](https://mozilla.github.io/pdf.js/) / [Cytoscape.js](https://github.com/cytoscape/cytoscape.js) |

只列实际查到的组件，不宣称“全网没有开源刑侦产品”。中文论文、通用RAG模板、剧本杀demo可以学习，但没有真实授权客户或生产效果证据时不与政务产品等量齐观。

许可注意：Autopsy 2与3/4许可不同，依赖另查；pgvector不是凭印象填写MIT；模型卡许可、代码许可、分发权重许可分开确认。固定版本后建立软件/权重清单。
