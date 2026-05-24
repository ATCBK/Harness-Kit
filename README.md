# HarnessKit

![HarnessKit Icon](./assets/harnesskit-icon.png)

HarnessKit 是一个 Markdown-first 的 Harness 文档库。  
目标是在编码前先固定：上下文、边界、任务拆解、验证标准、会话交接。

## 这是什么

- 不是代码框架
- 不是 CLI 工具
- 不是模板生成器网站
- 是一套可复用的 Harness 文档、流程、清单、示例

## 5 分钟快速开始

1. 选择一个模板目录（例如 `templates/minimal-harness/`）。
2. 复制模板到你的目标项目（通常放在项目根目录的 `ai/` 或同级 Harness 目录）。
3. 按 `workflows/01-08` 做 HITL 访谈，逐步填充 `TODO`。
4. 开发前先读：`AGENTS.md`、`product-origin.md`、`scope.md`、`feature-list.md`。
5. 开发后必更：`progress.md`、`verification.md`、`session-handoff.md`。

## 推荐使用路径（新用户）

1. 先读 `docs/concept.md` 和 `docs/harness-principles.md`，理解 Harness 作用。
2. 跑一遍 `checklists/harness-startup-checklist.md`，确认启动条件齐全。
3. 从 `examples/` 选一个最接近你的场景的示例，对照填模板。
4. 每完成一个功能，立刻补验证与交接，不要堆到最后。

## 最佳实践

- 小步更新：每轮开发只更新与本轮相关的 Harness 文档。
- 先范围后实现：`scope.md` 不清楚时，不进入编码阶段。
- 未知即 `TODO`：不要猜测，不要编造。
- 验收可执行：每个功能必须有可复现的验证步骤。
- 交接可落地：`session-handoff.md` 要写清下一步、阻塞点、风险。
- sub-agent 有边界：任务下发必须写目标、边界、输入、输出、验收标准；禁止并发改同一文件。

## 常见误区

- 只复制模板，不填 `TODO`。
- 只写过程，不写验收标准。
- 开发后不更新 `progress` 和 `session-handoff`。
- 在通用模板中写入具体业务事实。

## 仓库结构

- `docs/`：概念、原则、流程、指南、路线图
- `workflows/`：8 个 HITL 访谈流程
- `checklists/`：启动、开发前后、完整性、防漂移清单
- `templates/`：可复制 Harness 模板
- `examples/`：示例 Harness（仅演示）
- `skill/harnesskit-bootstrap/`：Bootstrap Skill、模板与参考资料

## 最小执行清单

1. 复制模板并创建项目专属 Harness。
2. 完成 `workflows/01-08` 的首轮填充。
3. 用 `checklists/harness-completeness-checklist.md` 自检。
4. 通过后再进入代码实现。

## 非目标

- 不提供 CLI
- 不提供 Web UI
- 不提供业务代码
- 不绑定具体技术栈

