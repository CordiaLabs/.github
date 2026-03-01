# Cordia Labs

Building infrastructure for durable, agentic workflows. 
We focus on state and control at the boundary between autonomous execution and human oversight.

## Focus Areas

* **Durable wait protocols:** Primitives that let agents pause execution without holding compute or losing state.
* **Human-in-the-loop (HITL):** Standard interfaces for manual verification and hot-patching of agent outputs.
* **Safety infrastructure:** Tool-use authorization, behavioral guardrails, and audit trails for high-stakes agent actions.

## Active Projects

### [LetsPing](https://github.com/CordiaLabs/LetsPing)

The agent trust layer: behavioral firewall, HITL, and Cryo-Sleep state for AI agents. Framework-agnostic SDKs (Python and Node/TypeScript), adapters for LangGraph and Vercel AI SDK, MCP server, and CLI. One client connects your agent to a hosted dashboard, triage, approvals, and audit. Optional agent-first layer: verifiable credentials, signed handoffs, and usage-based billing so agents can transact without a human.

### [OpenClaw-Skill](https://github.com/CordiaLabs/OpenClaw-Skill)

Sudo for OpenClaw. Intercepts high-risk agent actions (files, infra, payments) for human approval. Hot-patch payloads in real time via a zero-config mobile PWA.


[Website](https://letsping.co) · [Twitter](https://x.com/letspingai) · [Status](https://letsping.co/status)
