# 验收

个人 Codex Skill：为 Agent 产品完成 UI 设计与改版、真实流程测试、业务逻辑评测、根因排错、部署硬件容量评估和交付验收。

## 调用

安装后，在项目任务中输入：

```text
使用 $yanshou，把当前项目从头跑一遍，检查 UI、业务逻辑和 bug，给出验证证据及未完成项。
```

也可以只要求优化界面、修复具体 bug 或验收某条业务流程，不会强制重做整个项目。

部署前可以调用：

```text
使用 $yanshou，评估当前项目部署需要的 CPU、内存、磁盘、带宽和 GPU，结合在线并发与夜间任务量，给出配置、费用、扩容条件和待验证项。
```

资源评估先区分云端 API 与本地推理；不会默认要求 GPU，也不会把估算当成实测性能。不会自行购买服务器或启动生产压测。

## 安装到另一台 Codex

把此仓库根目录安装为个人技能目录中的 `yanshou` 文件夹，使 `yanshou/SKILL.md` 存在。也可在 Codex 中说明：

```text
请用 skill-installer 从 https://github.com/li3jia4hao5-hue/yanshou 安装仓库根目录的 Skill，名称为 yanshou。
```

私有仓库需要当前机器先拥有该 GitHub 仓库的读取权限。GitHub 保存与同步文件，实际调用依赖所在环境安装 Skill；上传本身不会让所有设备自动加载。

## 内容

- SKILL.md：工作范围、模式选择与交付规则。
- references/ui.md：设计方向、中文界面与真实截图验收。
- references/acceptance.md：四层测试证据、模型评测、排错与报告。
- references/deployment-capacity.md：部署资源、任务窗口、费用、验证与扩容条件。
- references/projects.md：子曰酒店与婚恋 CRM 的历史业务依据和专项回归案例，使用前需核对现状。
- references/sources.md：借鉴来源及未捆绑的上游能力。

不包含上游设计数据库、浏览器运行环境或 MLflow 安装包；不携带密钥和客户原始数据。技能安装与格式验证不等于项目已经验收。
