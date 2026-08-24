# ONINT Builder OS

## Purpose

ONINT is the control plane for building software with AI. It separates planning, implementation, testing, deployment, and operations so projects remain understandable and recoverable.

## Standard project lifecycle

### 1. Intake
Capture the desired outcome, users, constraints, integrations, security requirements, and acceptance criteria.

### 2. Plan
Produce an architecture, task breakdown, file plan, data model, API surface, test strategy, and deployment plan.

### 3. Build
Implement in small, reviewable changes. Prefer existing platform capabilities over unnecessary custom infrastructure.

### 4. Verify
Run unit tests, integration tests, type checks, linting, security checks, and a basic end-to-end smoke test.

### 5. Deploy
Deploy only after verification. Keep development, staging, and production configuration separate.

### 6. Operate
Monitor errors, performance, costs, and agent behavior. Convert recurring failures into tests or reusable skills.

## Agent roles

- **Planner:** turns requests into executable specifications.
- **Builder:** writes and modifies code.
- **Reviewer:** checks correctness, security, maintainability, and scope.
- **Tester:** creates and runs validation strategies.
- **Deployer:** prepares and executes deployment workflows.
- **Researcher:** gathers technical information and evaluates implementation options.
- **Operator:** investigates production failures and proposes safe fixes.

## Permission model

Agents should default to read-only access. Write access is granted only to the capability required for the current task. Production changes, credential changes, destructive operations, and irreversible migrations require explicit approval.

## Definition of done

A project is not considered complete until it has:

- documented requirements and architecture
- reproducible local setup
- tests for critical behavior
- secrets handled outside source control
- deployment configuration
- basic observability
- rollback/recovery instructions
- concise documentation for future agents
