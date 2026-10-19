# 来源与能力边界

本技能由用户于 2026-10-19 要求，为子曰与婚恋 Agent 产品落地整合。采用独立撰写的中文工作流程，并参考以下公开项目的思路；不是上游文件逐字拼接，不声称已安装或捆绑其代码、数据库、脚本或依赖。

- UI UX Pro Max：https://github.com/nextlevelbuilder/ui-ux-pro-max-skill — 按产品需求选择设计规范。其样式/配色检索数据库未包含在此技能中。
- Anthropic frontend-design：https://github.com/anthropics/skills/tree/main/skills/frontend-design — 明确视觉方向、字体布局、真实内容与视觉复核。
- Anthropic webapp-testing：https://github.com/anthropics/skills/tree/main/skills/webapp-testing — 浏览器实际交互、截图和日志证据。本技能不固定其浏览器 API，以当前可用工具及其规则为准。
- Superpowers systematic-debugging：https://github.com/obra/superpowers/tree/main/skills/systematic-debugging — 复现、证据、根因假设、针对性修复与回归。
- Superpowers verification-before-completion：https://github.com/obra/superpowers/tree/main/skills/verification-before-completion — 完成声明需要当前验证证据。
- MLflow agent-evaluation：https://github.com/mlflow/skills/tree/main/agent-evaluation — 数据集、评分和执行追踪；本技能只在已有 MLflow 时复用，不强制安装。

项目依据见 projects.md。历史交付声明只用于寻找验收重点，不是本次实测。

2026-10-19 补充检索的部署容量参考（已阅读技能说明，未运行其脚本）：
- capacity-and-cost-engineering：https://github.com/magnus919/agent-skills/tree/main/capacity-and-cost-engineering — 工作负载、峰值、容量证据与单位成本的规划方法。
- llm-capacity-planner：https://github.com/Gao-pw/LLM-Capacity-Planner-skill — 本地推理显存、KV Cache、上下文与并发规划；属于社区项目。未捆绑或验证其计算器，不能引用其理论吞吐作为承诺。
- qdrant-sizing：https://github.com/qdrant/skills/tree/main/skills/qdrant-sizing — Qdrant 专用容量估算；仅在实际使用 Qdrant 时参考，不把它的公式直接套给 SQLite 或其他引擎。

新增 deployment-capacity.md 为独立编写的通用与项目化流程；没有引入上游脚本、依赖或固定硬件型号。具体选型时仍需核对实际软件版本与官方硬件资料。
若以后直接引入上游文件或脚本，先检查其当前许可证、依赖与兼容性并保留必要声明；不要把本技能的来源链接当作已获得所有上游资产。
