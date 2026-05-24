# HarnessKit 仓库维护规则

- 本仓库是 Markdown-first 文档项目。
- 不添加程序代码，不创建 CLI，不创建 `src/`。
- 不创建 `package.json`、`tsconfig.json`。
- 新增内容必须服务于 Harness 启动、HITL、模板、清单或示例。
- 不把用户项目事实写进通用模板。
- 未知信息写 `TODO`。
- 示例必须包含：`This is an example harness for demonstration only.`
- 涉及 sub-agent 时必须写明：目标、边界、输入、输出、验收标准。
- sub-agent 只可在授权范围内工作，不可修改未授权区域。
- 多个 sub-agent 不得并发修改同一文件；冲突由主 agent 统一整合。
