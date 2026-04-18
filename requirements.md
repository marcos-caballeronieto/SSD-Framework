# Project Requirements & Environment Source of Truth

This file is the source of truth for the project requirements and environment, so the models have a place to look the versions and frameworks being used.

## 1. System Environment
*The base layer required to run the project.*
- **Runtime:** [e.g., Node.js v22.x (LTS), Python 3.12+]
- **Package Manager:** [e.g., pnpm v9.x, npm v10.x]
- **OS Constraints:** [e.g., Cross-platform, Linux-only for Production]

## 2. Core Dependencies (Pinned Versions)
*The Agent must strictly adhere to these versions when writing code.*
- **Framework:** [e.g., Next.js v15.0.0]
- **UI Library:** [e.g., Tailwind CSS v4.0.0-alpha]
- **AI SDK:** [e.g., Anthropic SDK v0.30.0, Vercel AI SDK v3.x]
- **State/Data:** [e.g., TanStack Query v5.x]

## 3. Development & Tooling
- **Testing:** [e.g., Playwright v1.48+, Vitest v2.1]
- **Linting/Formatting:** [e.g., Biome v1.9 (No ESLint/Prettier)]
- **Agentic Tools:** [e.g., Google Antigravity IDE, Claude Code CLI]

## 4. Environment Variables (Templates)
*List all required variables. DO NOT include real secrets.*
- `NEXT_PUBLIC_APP_URL`: The base URL for the app.
- `ANTHROPIC_API_KEY`: Required for agentic features.
- `DATABASE_URL`: Connection string for PostgreSQL.

## 5. Deployment Requirements
- **Platform:** [e.g., Vercel, Railway, Docker]
- **Build Command:** `npm run build`
- **Output Directory:** `.next/` or `dist/`

## 6. Dependency Update Policy
- **Strict Mode:** The Agent is **NOT** allowed to install new dependencies without explicit User approval.
- **Version Updates:** Do not update major versions unless specified in a new `feature_plan.md`.
- **Conflict Resolution:** If a dependency conflict arises, the Agent must stop and run `/refactor-check` before proceeding.