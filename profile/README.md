<div align="center">
  <h1>vespid-ai</h1>
  <p><strong>Open-source infrastructure for AI agents, autonomous agent systems, and trustworthy agent execution.</strong></p>
  <p>
    We build runtime, authorization, and portability layers for agent software that needs real boundaries:
    agent runtime, delegated authorization, sandboxed execution, protected actions, portable operator context,
    and durable memory / profile continuity.
  </p>
  <p>
    <a href="https://vespid.ai">Website</a>
    ·
    <a href="https://github.com/vespid-ai/vespid">Runtime</a>
    ·
    <a href="https://github.com/vespid-ai/skillauth">Authorization</a>
    ·
    <a href="https://github.com/vespid-ai/hermes-profile-sync">Portability</a>
  </p>
  <p>
    <a href="https://github.com/vespid-ai/.github/blob/main/profile/README.md">English</a>
    ·
    <a href="https://github.com/vespid-ai/.github/blob/main/profile/README.zh-CN.md">简体中文</a>
    ·
    <a href="https://github.com/vespid-ai/.github/blob/main/profile/README.ja.md">日本語</a>
    ·
    <a href="https://github.com/vespid-ai/.github/blob/main/profile/README.es.md">Español</a>
  </p>
</div>

## Multilingual overview

### 简体中文
vespid-ai 是一个面向 AI Agent / Autonomous Agent 的开源基础设施组织，重点覆盖 agent runtime、delegated authorization、sandboxed execution、protected actions、portable context / memory、operator tooling 等能力。我们希望把 AI 智能体真正进入生产环境时最关键的边界问题——执行、权限、上下文——拆成可验证、可复用、可组合的系统层。

### 日本語
vespid-ai は AI エージェント / autonomous agents 向けのオープンソース基盤です。agent runtime、delegated authorization、sandboxed execution、protected actions、portable context / memory、operator tooling を中心に、実運用で必要になる実行境界・認可・継続的コンテキストをブラックボックスではなく再利用可能なレイヤーとして設計しています。

### Español
vespid-ai construye infraestructura open source para agentes de IA y sistemas de autonomous agents: agent runtime, delegated authorization, sandboxed execution, protected actions, portable context / memory y operator tooling. Nuestro enfoque es separar ejecución, autorización y continuidad del contexto en capas auditables, reutilizables y componibles.

## Thesis

Most agent systems still fuse execution, identity, and memory into one opaque product surface.
That makes them easy to demo and hard to trust.

vespid-ai breaks the stack into explicit layers that can be inspected, reused, and composed:

- execution runtimes with real control boundaries
- delegated authorization instead of raw credential sharing
- portable agent context across machines and operator environments
- reference products that prove the model in practice

## Open-source stack

| Layer | Repository | Purpose |
| --- | --- | --- |
| Runtime substrate | [`vespid`](https://github.com/vespid-ai/vespid) | Brokered sessions, sandboxes, protected actions, and reusable execution primitives |
| Delegated authorization | [`skillauth`](https://github.com/vespid-ai/skillauth) | Safe agent access to login-gated platforms without handing over passwords or cookies |
| Profile portability | [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync) | Export, sanitize, sync, and restore operator profiles without copying unsafe machine state |
| Public docs and narrative layer | [`vespid-ai`](https://github.com/vespid-ai/vespid-ai) | Project documentation, field notes, and the public-facing systems story |

## Flagship repositories

### [`vespid`](https://github.com/vespid-ai/vespid)
Managed-agent runtime substrate for brokered sessions, sandboxes, and protected actions.
This is the systems layer underneath the rest of the stack: execution control, state boundaries,
and reusable runtime primitives for agent-native software.

### [`skillauth`](https://github.com/vespid-ai/skillauth)
Reference CLI and delegation toolkit for safe agent-driven platform access.
It demonstrates the authorization model directly: user authorization -> agent execution -> platform control.

### [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync)
Portable profile export, sanitization, sync, and restore for Hermes Agent setups.
It treats memories, config, sessions, logs, and secrets as different classes of state instead of one unsafe blob.

## Principles

### Authorization before automation
Agents should operate with scoped, revocable capability — not borrowed human identity.

### Runtime boundaries are product features
Isolation, brokered control, and protected execution matter as much as model quality.

### Durable context should be portable
A serious agent setup includes memory, config, and reusable skills, not just chat history.

### Open systems over hidden glue
We prefer inspectable primitives, reference implementations, and explicit tradeoffs over fragile magic.

## Current focus

The public repository set is converging on a coherent agent stack:

- `vespid` for runtime control
- `skillauth` for delegated authorization
- `hermes-profile-sync` for operator continuity and profile portability

Together they form a foundation for agent software that can survive production constraints:
human trust, system boundaries, reversibility, and operational realism.

## For builders

If you are building agent runtimes, operator tooling, controlled delegation, or memory portability,
these repositories are designed to be useful building blocks, not just concept demos.

Start here:

- Browse the docs at [vespid.ai](https://vespid.ai)
- Inspect the runtime direction in [`vespid`](https://github.com/vespid-ai/vespid)
- Study delegated authorization in [`skillauth`](https://github.com/vespid-ai/skillauth)
- Use [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync) to make local agent setups portable

## Status

Early, opinionated, and actively shaping the infrastructure layer for trustworthy agent systems.
