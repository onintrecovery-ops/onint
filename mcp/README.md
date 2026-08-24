# MCP Integration Layer

MCP integrations should expose narrowly scoped capabilities to Builder agents.

## Principles

- one integration per capability boundary
- least-privilege authentication
- explicit input/output contracts
- timeouts and failure handling
- auditable operations
- no secret values in prompts, logs, or source control

Potential integrations include GitHub, Cloudflare, project databases, documentation systems, and other developer services.
