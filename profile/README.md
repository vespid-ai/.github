<div align="center">
  <h1>vespid-ai</h1>
  <p><strong>Agent infrastructure for real-world execution.</strong></p>
  <p>
    We build the runtime, authorization, and portability layers that make AI agents
    usable beyond demos: brokered execution, protected actions, scoped delegation,
    and durable operator context.
  </p>
  <p>
    <a href="https://vespid.ai">Website</a>
    ·
    <a href="https://github.com/vespid-ai/vespid">Core runtime</a>
    ·
    <a href="https://github.com/vespid-ai/skillauth">SkillAuth</a>
    ·
    <a href="https://github.com/vespid-ai/hermes-profile-sync">Hermes Profile Sync</a>
  </p>
</div>

## What we build

Most agent products still collapse trust, execution, and memory into a single black box.
vespid-ai takes a different approach: break the agent stack into explicit system layers
that can be audited, reused, and safely composed.

- Runtime substrate for sandboxed and brokered agent execution
- Authorization patterns for login-gated and high-trust actions
- Durable profile and memory portability across machines and environments
- Product shells and reference implementations that prove the model in practice

## Featured repositories

| Project | What it is | Why it matters |
| --- | --- | --- |
| [`vespid`](https://github.com/vespid-ai/vespid) | Managed-agent runtime substrate for brokered sessions, sandboxes, and protected actions | The systems layer: execution control, state boundaries, and reusable runtime primitives |
| [`skillauth`](https://github.com/vespid-ai/skillauth) | Reference CLI and delegation toolkit for safe agent-driven platform access | Shows how users can authorize agents without sharing raw credentials or cookies |
| [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync) | Toolkit for exporting, sanitizing, syncing, and restoring Hermes profiles | Makes agent memory, skills, and config portable without blindly copying secret state |
| [`vespid.ai`](https://github.com/vespid-ai/vespid-ai) | Public site and documentation shell | The narrative layer for projects, docs, and field notes |

## Design principles

### 1. Authorization before automation
Agents should not inherit full human authority by default. Access should be scoped,
revocable, auditable, and tied to explicit intent.

### 2. Runtime boundaries matter
Useful agents need isolation, brokered control, and system-level contracts — not just
prompt engineering and browser macros.

### 3. Context should be portable
A serious agent setup is more than a chat log. Configuration, memory, and reusable skills
must move across machines cleanly and safely.

### 4. Open systems beat hidden glue
We prefer explicit primitives, reference implementations, and inspectable tradeoffs over
magic abstractions that break under real operational load.

## Current focus

Right now the open-source surface is converging on a clear stack:

- `vespid` for execution and protected runtime control
- `skillauth` for delegated authorization and platform-safe access
- `hermes-profile-sync` for profile portability and operator continuity

This is the foundation for agent-native software that can actually operate in production
settings with human trust, system boundaries, and repeatable workflows.

## For builders

If you're working on agent runtimes, operator tooling, delegated access, or durable memory,
these repos are meant to be useful as building blocks, not just demos.

Start here:

- Read the project docs on [vespid.ai](https://vespid.ai)
- Inspect the runtime direction in [`vespid`](https://github.com/vespid-ai/vespid)
- Study delegated authorization in [`skillauth`](https://github.com/vespid-ai/skillauth)
- Use [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync) for portable agent setups

## Status

Early, opinionated, and shipping. We optimize for clear architecture, operational realism,
and reusable open-source building blocks for the agent era.
