# Stack
- Purpose: record the agreed technology stack for this repository. Fill this out before implementation.

## Languages and runtimes
- Languages: TypeScript
- Runtimes/versions: Node.js 20 LTS

## Package manager
- Manager: pnpm
- Lockfile and constraints: pnpm-lock.yaml; use `pnpm install --frozen-lockfile` in CI

## Project types and targets
- Project types: Web app (Remix v3), single repo (not a monorepo)
- Build/test tooling: Remix compiler; Vitest for unit/integration; Playwright for e2e

## Deployment/CI notes
- CI provider: GitHub Actions (align with pnpm lint/format:check/test/test:e2e)
- Deployment targets (if any): TBD (default: none yet)

## Additional constraints
- Coding standards or policies to highlight: See policies/coding_standards.md and policies/testing_policy.md; follow policies/quality_gates.md commands with pnpm.
