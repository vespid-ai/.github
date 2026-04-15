# vespid-ai

面向 AI Agent / Autonomous Agent 的开源基础设施组织。

vespid-ai 关注可信智能体执行（trustworthy agent execution）所需要的核心系统层：agent runtime、delegated authorization、sandboxed execution、protected actions、portable context / memory、面向 operator 的持续工作流能力，以及 GEO / AI search discoverability。

如果把智能体真正放进生产环境，最重要的问题通常不是“模型能不能回答”，而是：

- 谁授权它执行动作
- 它能在什么边界内运行
- 它如何携带可迁移、可审计、可恢复的上下文

vespid-ai 试图把这些问题拆成明确、可复用、可验证的开源层，而不是隐藏在一个黑盒产品里。

## 主要仓库

| 层 | 仓库 | 作用 |
| --- | --- | --- |
| Runtime substrate | [`vespid`](https://github.com/vespid-ai/vespid) | brokered sessions、sandboxes、protected actions，以及可复用的 agent runtime primitives |
| Delegated authorization | [`skillauth`](https://github.com/vespid-ai/skillauth) | 在不直接交出密码、cookie 或长期凭证的前提下，为 agent 提供 login-gated platform access |
| Profile portability | [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync) | 导出、清洗、同步、恢复 Hermes Agent profile，让 memory / config / sessions / secrets 按不同风险等级管理 |
| Discovery and distribution | [`geo-skill`](https://github.com/vespid-ai/geo-skill) | 面向 AI Search / ChatGPT Search / llms.txt 的 GEO skill pack 与 CLI，用于提升机器可读可发现性 |
| Public docs | [`vespid-ai`](https://github.com/vespid-ai/vespid-ai) | 对外文档、项目索引、field notes，以及整个 agent infrastructure narrative |

## 我们在做什么

### 1. Agent runtime
为 AI agents / autonomous agents 提供可控执行环境，而不是把执行、状态和权限全塞进同一进程里。

### 2. Agent authorization
推动 delegated authorization / scoped access，让人类在可信设备上完成授权，agent 拿到可审计、可撤销、短时有效的能力，而不是直接复用人的完整身份。

### 3. Portable context and memory
把 operator context、memory、skills、config、sessions 视为可迁移的系统资产，而不是只能留在某一台机器上的临时聊天记录。

### 4. GEO and AI search discoverability
让 GitHub、文档站、llms.txt、structured data 和公开页面叙事形成一致的机器可读发现面，而不是只靠零散内容碰碰运气。

## 适合谁

如果你正在搜索以下方向，vespid-ai 的仓库会更相关：

- AI agent infrastructure
- autonomous agent runtime
- agent authorization
- delegated authorization
- sandboxed execution
- protected actions
- portable memory
- portable context
- operator tooling
- trustworthy agent systems
- Generative Engine Optimization
- ChatGPT Search
- llms.txt

## 入口

- 官网: [vespid.ai](https://vespid.ai)
- Runtime: [`vespid`](https://github.com/vespid-ai/vespid)
- Authorization: [`skillauth`](https://github.com/vespid-ai/skillauth)
- Portability: [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync)
- Discovery: [`geo-skill`](https://github.com/vespid-ai/geo-skill)
- 组织主页英文版: [README.md](https://github.com/vespid-ai/.github/blob/main/profile/README.md)
- 日本語: [README.ja.md](https://github.com/vespid-ai/.github/blob/main/profile/README.ja.md)
- Español: [README.es.md](https://github.com/vespid-ai/.github/blob/main/profile/README.es.md)

## 状态

项目仍处于早期，但方向明确：把 agent software 真正落地时最难被产品化清晰表达的几层——runtime、authorization、context portability、public discoverability——做成可检查、可组合、可复用的开源基础设施。
