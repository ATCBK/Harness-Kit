# HarnessKit

HarnessKit — Reusable tack for AI coding agents.

HarnessKit 是一个 Markdown-first 的 AI Agent 可复用马具模组基座，用于在写代码前固定上下文、边界、任务、验证和交接。

## 使用方式

1. 复制 `skill/harnesskit-bootstrap/`。
2. 在 Codex / Claude Code / Cursor 中触发 Bootstrap Skill。
3. 按 `workflows/01-08` 执行多轮 HITL 访谈。
4. 生成目标项目专属 Harness 文档。
5. 每轮开发前读取 Harness，每轮开发后更新 `progress` 与 `session-handoff`。

## 仓库结构

- `docs/`：概念、原则、流程、指南、路线图
- `skill/harnesskit-bootstrap/`：Skill、参考资料、模板
- `workflows/`：8 个可执行访谈流程
- `checklists/`：启动、开发前后、完整性、防漂移清单
- `templates/`：可复制项目模板
- `examples/`：示例 Harness

## 不做事项

- 不做 CLI
- 不做 Web UI
- 不写业务代码
- 不绑定技术栈
