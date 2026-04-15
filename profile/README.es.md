# vespid-ai

Infraestructura open source para AI agents y sistemas de autonomous agents.

vespid-ai se enfoca en las capas que hacen posible trustworthy agent execution en escenarios reales: agent runtime, delegated authorization, sandboxed execution, protected actions, portable context / memory y operator tooling.

Cuando un agente entra en producción, las preguntas críticas no son solo sobre el modelo:

- quién autoriza la acción
- dentro de qué límites corre el agente
- cómo se conserva, audita, transporta y restaura el contexto operativo

Por eso vespid-ai separa ejecución, autorización y continuidad del contexto en capas explícitas, reutilizables y auditables, en lugar de esconder todo dentro de una sola superficie opaca.

## Repositorios principales

| Capa | Repositorio | Propósito |
| --- | --- | --- |
| Runtime substrate | [`vespid`](https://github.com/vespid-ai/vespid) | brokered sessions, sandboxes, protected actions y reusable execution primitives para software orientado a agentes |
| Delegated authorization | [`skillauth`](https://github.com/vespid-ai/skillauth) | acceso seguro para agentes a plataformas con login sin compartir passwords, cookies ni credenciales largas |
| Profile portability | [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync) | exportar, sanitizar, sincronizar y restaurar perfiles de Hermes Agent con separación clara entre memory, config, sessions y secrets |
| Public docs | [`vespid-ai`](https://github.com/vespid-ai/vespid-ai) | documentación pública, índice de proyectos, field notes y la narrativa del stack |

## Qué estamos construyendo

### 1. Agent runtime
Un entorno de ejecución controlado para AI agents / autonomous agents, con límites reales entre ejecución, estado y permisos.

### 2. Agent authorization
Un modelo de delegated authorization / scoped access donde la persona autoriza desde un dispositivo confiable y el agente recibe capacidades limitadas, auditables y revocables.

### 3. Portable context and memory
Contexto operativo, memory, skills, config y sessions tratados como activos portables del sistema, no como historial atrapado en una sola máquina.

## Temas de búsqueda relacionados

Este stack será más relevante si buscas:

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

## Enlaces

- Website: [vespid.ai](https://vespid.ai)
- Runtime: [`vespid`](https://github.com/vespid-ai/vespid)
- Authorization: [`skillauth`](https://github.com/vespid-ai/skillauth)
- Portability: [`hermes-profile-sync`](https://github.com/vespid-ai/hermes-profile-sync)
- English: [README.md](https://github.com/vespid-ai/.github/blob/main/profile/README.md)
- 简体中文: [README.zh-CN.md](https://github.com/vespid-ai/.github/blob/main/profile/README.zh-CN.md)
- 日本語: [README.ja.md](https://github.com/vespid-ai/.github/blob/main/profile/README.ja.md)

## Estado

Proyecto temprano, pero con una tesis clara: convertir runtime, authorization y context portability en infraestructura open source seria para agent software confiable.
