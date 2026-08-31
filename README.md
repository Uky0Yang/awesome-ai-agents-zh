# Awesome AI Agents 中文社区

面向中文开发者的 AI Agents、MCP、AI 编程工具和生产化实践社区：既能快速找到可靠工具，也能提问、分享作品和交流真实经验。

> 这个仓库用结构化数据维护清单，README 由脚本生成。社区交流使用 GitHub Discussions，项目收录使用 Issue 和 PR。

## 为什么做这个社区

AI agents、MCP、AI coding、TypeScript 和开发者工具正在成为开源增长最快的方向之一。英文资料很多，但中文开发者通常需要更快判断：

- 这个工具解决什么问题
- 适合个人学习还是团队生产
- 是否开源、是否活跃
- 从哪里开始上手

这个项目的目标是做一个克制、可维护、对实际开发有帮助的中文社区，而不是把所有链接都塞进来。导航负责降低信息筛选成本，讨论区负责沉淀中文问题、实践经验和可复用作品。

## 快速入口

| 分类 | 适合谁 | 代表方向 |
| --- | --- | --- |
| AI 编程助手 | 想提高日常编码效率的开发者 | IDE、终端 coding agent、代码审查 |
| Agent 框架 | 想构建复杂 AI 工作流的开发者 | 多智能体、状态图、任务编排 |
| MCP 生态 | 想把工具接入 AI agent 的开发者 | MCP server、工具调用、上下文连接 |
| RAG 与知识库 | 想做知识问答和企业搜索的团队 | 文档解析、向量检索、评估 |
| 浏览器自动化 | 想让 agent 操作网页和 SaaS 的开发者 | Web automation、Playwright、browser agents |
| 安全与评估 | 想把 agent 放进生产环境的团队 | 权限、提示注入、测试、监控 |

## 加入中文社区

社区以 GitHub 为场地，不需要加入新的聊天群。请选择最合适的入口：

| 你想做什么 | 入口 | 发帖前准备 |
| --- | --- | --- |
| 遇到工具或开发问题 | [Q&A 求助](https://github.com/Uky0Yang/awesome-ai-agents-zh/discussions/categories/q-a) | 说明目标、环境、已经尝试的方法和完整错误信息 |
| 展示自己的项目或实验 | [Show and tell](https://github.com/Uky0Yang/awesome-ai-agents-zh/discussions/categories/show-and-tell) | 提供可访问链接、实际用途、验证结果和你与项目的关系 |
| 建议新栏目或社区改进 | [Ideas](https://github.com/Uky0Yang/awesome-ai-agents-zh/discussions/categories/ideas) | 先搜索重复讨论，再说明问题和预期价值 |
| 推荐一个工具进入导航 | [推荐项目](https://github.com/Uky0Yang/awesome-ai-agents-zh/issues/new?template=tool.yml) | 提供维护、文档和实际使用证据 |
| 直接改进目录或文档 | [贡献指南](CONTRIBUTING.md) | 编辑结构化数据并运行本地校验 |

参与前请阅读 [社区公约](COMMUNITY.md) 和 [行为准则](CODE_OF_CONDUCT.md)。中文优先，英文贡献同样欢迎；项目名、命令和技术术语请保留准确原文。

## 精选项目

<!-- BEGIN GENERATED -->

### AI 编程助手

| 项目 | 简介 | 语言 | 开源 | 适合阶段 |
| --- | --- | --- | --- | --- |
| [OpenAI Codex](https://openai.com/codex) | 云端和本地开发环境中的 AI coding agent，适合把 issue、修复和重构交给 agent 处理。 | N/A | 否 | 进阶 |
| [Claude Code](https://www.anthropic.com/claude-code) | 终端里的 agentic coding 工具，强调理解大型代码库并执行多步开发任务。 | N/A | 否 | 进阶 |
| [Cursor](https://www.cursor.com/) | AI-first 代码编辑器，适合日常补全、重构、解释代码和多文件编辑。 | N/A | 否 | 入门 |
| [Continue](https://github.com/continuedev/continue) | 开源 AI 代码助手，可连接不同模型并集成 VS Code / JetBrains。 | TypeScript | 是 | 入门 |
| [Aider](https://github.com/Aider-AI/aider) | 命令行 AI pair programming 工具，适合在 Git 仓库内进行可审查的代码修改。 | Python | 是 | 入门 |

### Agent 框架

| 项目 | 简介 | 语言 | 开源 | 适合阶段 |
| --- | --- | --- | --- | --- |
| [LangGraph](https://github.com/langchain-ai/langgraph) | 用图结构构建可控、可恢复的 agent 工作流，适合生产级多步骤任务。 | Python / TypeScript | 是 | 进阶 |
| [AutoGen](https://github.com/microsoft/autogen) | 微软开源的多 agent 框架，适合研究协作式 agent 和复杂任务编排。 | Python | 是 | 进阶 |
| [CrewAI](https://github.com/crewAIInc/crewAI) | 面向角色和任务的 agent 编排框架，适合快速搭建多 agent demo 和业务流程。 | Python | 是 | 入门 |
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) | 开源软件开发 agent 平台，目标是让 agent 像开发者一样修改代码和运行命令。 | Python / TypeScript | 是 | 进阶 |
| [Orkas](https://github.com/Orkas-AI/Orkas) | MIT 开源的本地优先多 agent 桌面应用，通过 Commander 协调专业 agent 并行或串行完成复杂任务。 | TypeScript | 是 | 进阶 |

### MCP 生态

| 项目 | 简介 | 语言 | 开源 | 适合阶段 |
| --- | --- | --- | --- | --- |
| [Model Context Protocol](https://modelcontextprotocol.io/) | Anthropic 推出的开放协议，用于让模型安全连接工具、数据源和上下文。 | Spec | 是 | 入门 |
| [Awesome MCP Servers](https://github.com/punkpeye/awesome-mcp-servers) | 社区维护的 MCP server 清单，适合查找现成工具连接器。 | Markdown | 是 | 入门 |
| [FastMCP](https://github.com/jlowin/fastmcp) | Python MCP server 开发框架，适合快速把内部工具包装成 agent 可调用能力。 | Python | 是 | 入门 |
| [SandBase Harness](https://github.com/sandbaseai/sandbase-harness) | 本地优先、自托管的 AI agent runtime 与 MCP bridge，提供 sessions、memory、credentials、audit/replay 和本地 Console。 | TypeScript | 是 | 进阶 |

### RAG 与知识库

| 项目 | 简介 | 语言 | 开源 | 适合阶段 |
| --- | --- | --- | --- | --- |
| [LlamaIndex](https://github.com/run-llama/llama_index) | 面向 LLM 应用的数据框架，常用于 RAG、知识库和文档问答。 | Python / TypeScript | 是 | 入门 |
| [RAGFlow](https://github.com/infiniflow/ragflow) | 开源 RAG 引擎，关注文档解析、知识库和企业搜索场景。 | Python / TypeScript | 是 | 入门 |
| [Dify](https://github.com/langgenius/dify) | 开源 LLM 应用开发平台，支持工作流、RAG、agent 和应用发布。 | TypeScript / Python | 是 | 入门 |

### 浏览器自动化

| 项目 | 简介 | 语言 | 开源 | 适合阶段 |
| --- | --- | --- | --- | --- |
| [browser-use](https://github.com/browser-use/browser-use) | 让 AI agent 控制浏览器完成网页任务的开源项目。 | Python | 是 | 入门 |
| [Playwright](https://github.com/microsoft/playwright) | 可靠的浏览器自动化和端到端测试框架，是许多 browser agent 的底层能力。 | TypeScript | 是 | 入门 |
| [Agent QA](https://github.com/vostride/agent-qa) | 用自然语言编写和运行 Web/移动端测试，保存测试记忆，并在界面变化时自动修复流程；提供 CLI、Dashboard、MCP 和 Agent Skills。 | TypeScript | 否 | 进阶 |

### 安全与评估

| 项目 | 简介 | 语言 | 开源 | 适合阶段 |
| --- | --- | --- | --- | --- |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) | AI 系统评估框架，适合构建可重复的模型和 agent 评测。 | Python | 是 | 进阶 |
| [Promptfoo](https://github.com/promptfoo/promptfoo) | LLM 应用测试和评估工具，适合回归测试、红队测试和质量对比。 | TypeScript | 是 | 入门 |
| [Gitleaks](https://github.com/gitleaks/gitleaks) | 检测 Git 仓库中的密钥泄露，适合作为开源项目前的安全检查。 | Go | 是 | 入门 |

<!-- END GENERATED -->

## 收录标准

- 项目有明确用途，而不是只有概念介绍
- 最近仍有维护迹象
- 文档能让新用户在 30 分钟内开始
- 对中文开发者有学习、开发或生产价值
- 优先收录开源项目；闭源工具只在影响力足够大时作为生态参考

## 不收录

- 纯营销页面
- 无法运行、无文档、无维护迹象的 demo
- 需要泄露 API key 或要求过高权限的工具
- 重复度高、没有差异化价值的项目

## 本地维护

需要 Python 3.10+。

```bash
python scripts/generate_readme.py
python scripts/validate_catalog.py
```

新增项目请编辑 [data/tools.json](data/tools.json)，然后运行生成脚本。

## 贡献

请先阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。推荐通过 issue 提名项目，再由维护者或贡献者整理进清单。

## Agent OSS Toolkit

这个项目属于一组面向 AI coding agents 和开源发布流程的小工具：

- [repo-agent-bench](https://github.com/Uky0Yang/repo-agent-bench): 在真实仓库中 A/B 测试 AGENTS.md、Agent Skills、MCP 与 coding-agent 工作流
- [agent-repo-kit](https://github.com/Uky0Yang/agent-repo-kit): 一键生成 agent-ready 开源项目骨架
- [oss-launch-check](https://github.com/Uky0Yang/oss-launch-check): 检查仓库是否已经准备好开源发布
- [repo-context-card](https://github.com/Uky0Yang/repo-context-card): 为 AI coding agents 生成紧凑仓库上下文卡片
- [agent-rules-lint](https://github.com/Uky0Yang/agent-rules-lint): 检查 AGENTS.md、CLAUDE.md、Cursor rules 等 agent 指令文件
- [awesome-ai-agents-zh](https://github.com/Uky0Yang/awesome-ai-agents-zh): 中文 AI Agents / MCP / AI DevTools 导航

## License

MIT
