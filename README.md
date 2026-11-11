# Agent 工程：项目推进式学习仓库

用同一个知识库工单处理台，交付传统实现、单 Agent、多 Agent 三个独立可运行的版本。资料、笔记和应用变更都经过 branch → PR → review → merge。

## 当前状态

- 大纲与六项选型已由用户于 2026-11-11 确认，正在通过首个文档 PR 落库。
- 本仓库当前只有项目大纲与协作规则；尚无可运行应用、启动实测或 Agent 评测结果。
- 本次不编写学习排期、不实现应用、不生成 PPT、不批量整理原始资料。
- 下一步是构造学习计划并提交独立 PR，随后推进 s0。

## 阅读入口

| 内容 | 入口 |
| --- | --- |
| 阶段目标、结构、失败预判与验收 | [项目大纲](docs/outline.md) |
| 已确认选择与代价 | [决策记录 0001](notes/decisions/0001-project-outline.md) |
| 十页演示结构 | [PPT 大纲](docs/presentation-outline.md) |
| Agent 执行规则 | [AGENTS.md](AGENTS.md) |
| 角色输入、记忆分区和 PR 交接 | [上下文地图](.agent/context-map.md) |
| 本阶段提交与审查 | [PR 列表](https://github.com/AutsKlam/study-projects/pulls?q=is%3Apr) |

## 已确认的项目边界

知识库工单处理台；Python 后端与 TypeScript 前端分离；s1 使用 LangChain Agent 接口；只提供真实模型模式；在已确认范围内，独立 review 与检查通过后由执行 Agent 合并；三天扩展重点为 MCP 接入与部署复现，暂不实际微调。

每个受审 commit 都必须有 reviewer 发布的 GitHub commit comment，最终通过结论必须对应 PR 当前 HEAD。可以使用 CodeGraph，但纯文档任务不创建索引。

原有课程材料仍保留在本地 `agentstudy/`，本次没有纳入 Git；后续按任务需要选取资料，并记录来源与适用边界。
