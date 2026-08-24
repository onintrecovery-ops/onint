# Builder Safety Policy

## Default permissions

Agents may inspect project files, propose changes, create tests, and work on non-production branches.

## Approval required

Explicit user approval is required before:

- deleting repositories or production data
- changing production credentials
- rotating or exposing secrets
- irreversible database migrations
- deploying an unreviewed production release
- spending material amounts on paid infrastructure
- granting a new external integration broad access

## Secret handling

Secrets belong in the platform's secret manager or environment configuration. Never commit API keys, passwords, private keys, tokens, or credential files.

## Failure behavior

If an action fails, preserve the failure details, stop before destructive retries, and report the smallest safe next step.
