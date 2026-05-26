# GitHub Copilot Instructions

You are contributing to an open-source, cloud-native, multi-tenant, composable, lightweight, and cost-optimized SaaS platform template.

## Core engineering principles

- Prefer modular, composable architecture over monolith coupling.
- Design for portability across cloud vendors and self-hosted environments.
- Keep dependencies minimal and runtime images small.
- Default to secure-by-design implementation patterns.
- Support multi-tenancy from the beginning.
- Avoid vendor lock-in whenever possible.
- Prefer open standards and open-source tooling.
- Optimize for developer experience, maintainability, and operational simplicity.
- Ensure accessibility, API-first interoperability, and automation friendliness.

## Multi-tenant requirements

- All domain models should be tenant-aware.
- Authentication and authorization must support organization/workspace boundaries.
- APIs should support rate limits, quotas, and audit logging.
- Avoid hardcoded tenant assumptions.

## Cloud-native requirements

- Services should expose health/readiness endpoints.
- Prefer stateless workloads.
- Configuration must come from environment variables or secret stores.
- Emit structured logs and metrics.
- Design for autoscaling and rolling deployments.

## Cost optimization rules

- Minimize idle infrastructure.
- Prefer event-driven and scale-to-zero patterns where appropriate.
- Avoid unnecessary background jobs and oversized dependencies.
- Measure and expose resource usage.

## Repository conventions

- apps/: user-facing applications
- services/: backend APIs and workers
- packages/: shared libraries and SDKs
- infra/: infrastructure as code
- docs/: architecture and operational documentation
- examples/: starter implementations

## Code quality

- Add tests for business-critical logic.
- Use linting and formatting.
- Prefer typed interfaces and explicit contracts.
- Document architecture decisions.
- Keep commits focused and reviewable.
