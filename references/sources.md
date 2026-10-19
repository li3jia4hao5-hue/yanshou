# 来源与能力边界

本技能由用户于 2026-10-19 要求，为子曰与婚恋 Agent 产品落地整合。采用独立撰写的中文工作流程，并参考以下公开项目的思路；不是上游文件逐字拼接，不声称已安装或捆绑其代码、数据库、脚本或依赖。

- UI UX Pro Max：https://github.com/nextlevelbuilder/ui-ux-pro-max-skill — 按产品需求选择设计规范。其样式/配色检索数据库未包含在此技能中。
- Anthropic frontend-design：https://github.com/anthropics/skills/tree/main/skills/frontend-design — 明确视觉方向、字体布局、真实内容与视觉复核。
- Anthropic webapp-testing：https://github.com/anthropics/skills/tree/main/skills/webapp-testing — 浏览器实际交互、截图和日志证据。本技能不固定其浏览器 API，以当前可用工具及其规则为准。
- Superpowers systematic-debugging：https://github.com/obra/superpowers/tree/main/skills/systematic-debugging — 复现、证据、根因假设、针对性修复与回归。
- Superpowers verification-before-completion：https://github.com/obra/superpowers/tree/main/skills/verification-before-completion — 完成声明需要当前验证证据。
- MLflow agent-evaluation：https://github.com/mlflow/skills/tree/main/agent-evaluation — 数据集、评分和执行追踪；本技能只在已有 MLflow 时复用，不强制安装。

项目依据见 projects.md。历史交付声明只用于寻找验收重点，不是本次实测。
若以后直接引入上游文件或脚本，先检查其当前许可证、依赖与兼容性并保留必要声明；不要把本技能的来源链接当作已获得所有上游资产。
