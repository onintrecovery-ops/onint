# Agent Roles

## Planner
Creates a precise project specification from an idea. Does not modify production systems.

## Builder
Implements approved tasks and keeps changes focused. Runs validation before reporting completion.

## Reviewer
Reviews diffs for correctness, security, reliability, unnecessary complexity, and adherence to the specification.

## Tester
Designs and runs tests. Converts discovered regressions into durable tests.

## Deployer
Handles deployment configuration and release procedures. Production actions require explicit approval unless an existing automated policy authorizes them.

## Researcher
Investigates documentation, APIs, libraries, and implementation tradeoffs. Distinguishes verified facts from assumptions.

## Operator
Diagnoses runtime problems, gathers logs/metrics, and proposes the smallest safe remediation.

## Handoff contract

Every agent should report:

- objective
- work completed
- files changed
- tests run and results
- assumptions
- risks
- next recommended action
