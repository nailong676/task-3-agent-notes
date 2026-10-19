# ai-agent-book 学习笔记（第四章 · 工具 Tools 与 MCP）

记录阅读 [bojieli/ai-agent-book](https://github.com/bojieli/ai-agent-book) 第四章的学习心得，以及 2 个实验（4-4 执行工具 / 4-1 主动工具发现）的部署、运行与排障记录。

**课程来源标注**：本笔记基于开源教程 [github.com/bojieli/ai-agent-book/tree/main](https://github.com/bojieli/ai-agent-book/tree/main) 整理，在线教程见[第四章](https://bojieli.github.io/ai-agent-book/astro/book/chapter4/)。实验代码为书本配套源码，本地运行验证，未放入本仓库；本仓库只保存学习笔记与实验原始输出。

| 文件 | 内容 |
|---|---|
| [学习心得.md](学习心得.md) | 五类工具分类、感知/执行/协作工具要点、MCP 三能力区别、大规模工具按需加载；6 道自测题（均带实验证据）；踩坑记录与一句话总结 |
| [实验4-4-执行工具部署与运行记录.md](实验4-4-执行工具部署与运行记录.md) | execution-tools：七步 demo、8 个无效参数/安全拦截探针、在线 LLM 审批 vs 离线 fail-safe 对照、一个真实 bug 的定位与修复 |
| [实验4-1-主动工具发现部署与运行记录.md](实验4-1-主动工具发现部署与运行记录.md) | active-tool-discovery：离线三策略对比、Kimi 真实运行、429 限流排障、检索后端退化的影响 |
| [实验数据/](实验数据/) | 两次实验的完整原始输出（demo 日志、探针日志、离线汇总、真实运行日志） |

**环境**：Windows 11 + Python 3.12（仓库根共享 venv，纯 CPU）· shell 后端为 Git Bash · LLM 走 Kimi（Moonshot，OpenAI 兼容网关，组织级配额 3 RPM）
