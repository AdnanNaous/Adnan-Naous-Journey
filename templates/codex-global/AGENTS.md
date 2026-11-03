# VC351 — Global Codex Working Principles

These preferences apply when this document is installed as a user-level Codex AGENTS.md. Repository-specific AGENTS.md and the user's current request provide additional context; do not overwrite or weaken project-specific safety restrictions.

## Workspace model

- Device: local development environment and execution tools.
- Notion: personal knowledge base, planning, and notes.
- GitHub: project source of truth (source code, reviews, versions, releases and automation); not a substitute for independent backups.
- AI: Codex, Claude Code, or local assistants supporting scoped engineering tasks.
- Browser: Chrome and browser-based tools; do not infer access to private tabs or sessions.

## Default engineering workflow

1. **GitHub first.** Inspect the repository, its relevant instructions, current working tree, and version history before editing.
2. Prefer local development, meaningful tests, code review, and reproducible builds. Do not confuse a successful build with verified production behavior.
3. **Cloudflare is the default deployment preference**, but design the application for portability. Put vendor-specific database, authentication, storage, email, analytics, and payment integrations behind clearly defined boundaries. Vercel, a VPS, or another provider remain valid when justified.
4. When reasonable, build local-first features using browser/device storage and explicit export/import. Never add login, cloud data collection, or online dependence without the user's request.
5. Keep secrets, private user data, credentials, personal histories, .env files, and database exports out of repositories, logs, and artifacts. Treat public source, public releases, and private development history separately.
6. Protect existing work. Never change repository visibility, delete branches/history, move critical data, deploy publicly, enable paid features, or modify account permissions without explicit user authorization.
7. For significant changes, explain tradeoffs, test evidence, remaining limitations, rollback and backup implications. Avoid claims of zero bugs, guaranteed security or exaggerated skill/completion.
8. Prefer clean, responsive, accessible, performant interfaces. Do not redesign unrelated existing UI without request.
9. Use least-privilege access for integrated apps and separate production/secrets from client-side code.
10. Keep instructions concise, verifiable, and compatible with the existing project instead of inventing scaffolding.

## Repository independence

Read the nearest repo-specific AGENTS.md before changing code; the global guide is not a substitute for understanding a project. Notion files, secrets, and personal context must not be assumed accessible from this guide.
