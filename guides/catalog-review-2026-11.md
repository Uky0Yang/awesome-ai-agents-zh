# 2026-11-18 收录核验

本轮处理 2 个贡献 PR 和 8 个提名 issue，目录从 28 项增至 32 项，并新增
“学习资源”分类。核验包括公开源码、许可证、发布记录、安装文档和目录生成；
没有安装或运行被提名的项目，没有调用付费 API、连接用户账号，也没有把项目
自述当作安全或效果认证。

## 新增条目

| 项目 | 固定来源 | 核验结果 | 使用前需要了解 |
| --- | --- | --- | --- |
| [Orbi](https://github.com/orbi-build/orbi/tree/596ab6be6aadec1f4d5e7ce9fd87c106101c3c89) | 上游提交 `596ab6b`；[PR #20](https://github.com/Uky0Yang/awesome-ai-agents-zh/pull/20) | AGPL-3.0，Python 源码，有中文 README，最新 release v0.7.48（2026-11-18）；贡献者披露维护者身份 | 它会自行写代码、合并 PR 并发版，先在不重要的测试仓库里限定权限试用。AGPL-3.0 对修改后提供网络服务有源码公开要求。模型调用可能产生费用 |
| [oh-my-hermes](https://github.com/rlaope/oh-my-hermes/tree/520d9f4c63a71b393030fc79b69c531a197c1c76) | 上游提交 `520d9f4`；[Issue #28](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/28) | MIT，Python 源码，有中文 README，最新 release v4.0.8（2026-11-15）；由项目贡献者自荐 | 它是 Hermes Agent 的插件与技能集，不是独立 agent，需要先配置 Hermes 和模型服务。官方安装方式是下载并执行远程脚本，运行前先阅读脚本内容 |
| [Doc2X MCP](https://github.com/NoEdgeAI/doc2x-mcp/tree/263da5a22f9c64129229a8704505cde85ad5bfc6) | 上游提交 `263da5a`；[Issue #24](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/24) | MIT，TypeScript 源码，npm 包 `@noedgeai-org/doc2x-mcp` 0.1.7 与源码版本一致；受项目方委托投稿 | 代码开源不代表服务免费：需要自己的 Doc2X API key，按用量计费。文档会上传到 Doc2X 服务解析，不要直接处理敏感文件 |
| [AI Agent 实战手册](https://github.com/Xwh630/ai-agent-handbook/tree/0a1e8eb38bad10f9a693ba1b242d255c42a4015a) | 上游提交 `0a1e8eb`；[Issue #25](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/25) | MIT，中文章节、示例目录和 CLI 源码，最新 release v1.5.0（2026-10-25）；作者本人自荐 | 核验时 PyPI 上查不到 `agent-handbook`，仓库描述里的 `uvx agent-handbook` 命令未能确认可用，目前按提名说明从 Git 安装。CLI 的打分是作者自定的检查表，不是第三方评测 |

Orbi 的 PR 只修改目录数据和生成的 README，按审查过的提交 `b02bc53` 合并。
其余三项由维护者根据 issue 写入 `data/tools.json`，README 由脚本重新生成并
确认无漂移。

## 未收录

| 提名 | 结论 | 原因 |
| --- | --- | --- |
| TANDIU（[PR #23](https://github.com/Uky0Yang/awesome-ai-agents-zh/pull/23)、[Issue #22](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/22)） | 待修改 | 官方 MCP Registry 中确有 `cn.tandiu/data`。但 PR 简介 107 字超过 100 字上限，README 为手工修改而非脚本生成，PR 与 issue 使用的域名不一致，提交者关系在表单和正文中的说法不一致 |
| Agent Payment Node（[Issue #26](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/26)） | 暂不收录 | 让 agent 发起并签名链上支付，一旦出错损失难以挽回。目前没有独立安全审计，提名方也未执行过支付流程，本目录无法核验其安全性 |
| PlaceCall（[Issue #27](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/27)） | 不收录 | 通话服务闭源托管，且只能拨打美国号码，对中文开发者的直接价值有限 |
| Twinkle Model（[Issue #30](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/30)） | 不收录 | 闭源的模型 API 中转服务，服务质量与上游授权均无法核验，不属于本目录收录的工具类型 |
| TANCO SkillHub（[Issue #12](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/12)） | 关闭 | 2026-08-24 要求补充安装/运行步骤和真实案例后一直没有回应；补齐后可重新提名 |
