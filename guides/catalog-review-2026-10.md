# 2026-10-06 收录核验

本轮接收两位维护者的贡献，目录从 26 项增至 28 项。核验包括公开源码、
许可证、使用文档、服务入口与目录生成；没有运行付费模型、连接用户账号，
也没有把功能说明当作安全或效果认证。

| 项目 | 固定来源 | 核验结果 | 使用前需要了解 |
| --- | --- | --- | --- |
| [OrcaReplay](https://github.com/Continuum-AI-Corp/OrcaReplay/tree/a9178ca26af95cfd3231b8eb2da4ae11dbbd0a84) | 上游提交 `a9178ca`；[PR #17](https://github.com/Uky0Yang/awesome-ai-agents-zh/pull/17) | Apache-2.0，TypeScript 源码，npm CLI、trace 规范和 MCP 使用文档；贡献者披露维护者身份 | 文档说明重放仍会执行工具调用，工具自身的网络请求不一定被阻断；先在隔离的测试项目使用。模型对比可能产生费用 |
| [LogNorm](https://github.com/lognorm/lognorm-mcp/tree/74ee2ffbbf4980ca7ae2836fb3426ccc92d6c527) | 连接文档提交 `74ee2ff`；[PR #18](https://github.com/Uky0Yang/awesome-ai-agents-zh/pull/18) | 托管服务，配套 MIT 文档/skill/插件配置；[使用文档](https://lognorm.com/docs/agents) 返回 HTTP 200，MCP 入口返回 HTTP 401 并提供公开 OAuth resource metadata | 配套文档开源不代表托管服务开源，目录保留 `open_source: false`。账号授权后的实际调用、OAuth 全流程和服务效果尚未验证 |

两份 PR 都只修改目录数据和生成的 README；已检查原始提交、运行目录校验、
重新生成 README 并确认无漂移。外部贡献的 GitHub Actions 经审查后获准运行并通过。
两条目插入同一位置产生的合并冲突已解决，双方内容与贡献历史均保留。

[Issue #12](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/12) 截至核验时没有
补充此前要求的安装/运行和真实案例证据，继续保持待补充状态。
