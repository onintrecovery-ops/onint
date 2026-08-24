# ONINT — Personal AI Builder OS

A personal AI software-building stack designed to turn ideas into tested, deployable projects.

## Mission

Describe an outcome. The builder plans the work, creates code, tests it, reviews it, and prepares deployment.

## Architecture

- `agents/` — AI agent roles and orchestration
- `apps/` — applications built with the stack
- `skills/` — reusable building instructions
- `mcp/` — Model Context Protocol integrations
- `infra/` — deployment and infrastructure configuration
- `docs/` — architecture and operating guides
- `tests/` — validation and regression tests
- `scripts/` — developer automation

## Builder loop

1. Define the outcome
2. Create a technical plan
3. Implement the smallest working version
4. Test and review
5. Deploy
6. Observe failures and iterate

## Safety

Agents should use least-privilege credentials, keep secrets out of source control, require approval for destructive or production-sensitive actions, and produce auditable changes.

## Status

Initial foundation.
