# Quality Gates
- Purpose: define concrete commands that must pass before merge. Align these with package scripts and CI.

## Lint
- Command: pnpm lint
- Notes: Remix ESLint config, runs on app code and tests; keep ignores in `.eslintignore` in sync with CI.

## Format
- Command: pnpm format:check
- Notes: Prettier `--check` across repo; use `pnpm format` to apply fixes before merge.

## Test
- Command: pnpm test && pnpm test:e2e
- Notes: `test` runs Vitest unit/integration suites; `test:e2e` runs Playwright smoke suite headless (Chromium) with minimal fixtures. Keep snapshots updated.

## Failure handling
- Policy: Fix failures and rerun locally; waivers require explicit approval from the human lead/maintainer for the change set.
- Reporting: Record command outcomes in the PR checklist/comment and attach CI job links; note any skipped suites with rationale.
