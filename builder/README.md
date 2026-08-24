# ONINT Builder Engine

The Builder Engine is the orchestration contract for turning a request into a validated software change.

## Pipeline

`INTAKE -> PLAN -> BUILD -> TEST -> REVIEW -> RELEASE`

Each stage produces an artifact and a structured handoff. Failed validation returns the work to the smallest stage that can resolve the failure.

## Core contracts

- Input: user outcome, constraints, and approval boundaries
- Plan: architecture, task graph, acceptance criteria, risk assessment
- Build: focused code changes
- Test: reproducible validation results
- Review: security, correctness, maintainability, and scope assessment
- Release: deployment plan and explicit production approval where required

## Design rules

1. Keep agents specialized and composable.
2. Keep state in durable external systems rather than process globals.
3. Make every important action auditable.
4. Prefer deterministic automation for repetitive operations.
5. Never place secrets in the repository.
6. Require explicit approval for destructive or production-sensitive operations.
