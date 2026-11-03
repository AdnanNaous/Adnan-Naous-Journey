# GitHub-first operations

GitHub First → Develop → Test → Review → Deploy Anywhere.

Device + VS Code provide development and execution; GitHub holds canonical code, history, reviews and releases. Notion holds knowledge and planning. Codex Cloud/CLI, Claude Code and local AI agents assist engineering. Chrome is the web workspace. Cloudflare is the preferred future hosting provider. Security, backups and portability cross every layer.

## Agent instructions

A repository-root `AGENTS.md` is discoverable by Codex for that repository; nested files refine their directory scope. A template elsewhere on GitHub is not a global instruction. Preserve generated framework guidance and project-specific privacy rules.

For local Codex CLI, review [the global template](../../templates/codex-global/AGENTS.md), then manually merge its preferences into `~/.codex/AGENTS.md` (or `$CODEX_HOME/AGENTS.md` when using a custom Codex home). Back up an existing file first. On Windows, the default is `%USERPROFILE%\.codex\AGENTS.md`. Do not replace existing instructions wholesale. Test discovery in a fresh Codex session by asking it to summarize applicable instructions. Codex Cloud needs the instructions committed in each selected repository and the correct repository/branch selected for the task; local configuration does not configure Cloud tasks.

Claude Code uses `CLAUDE.md`; for a repository using AGENTS.md, merge an `@AGENTS.md` import into an existing CLAUDE.md, or create a short CLAUDE.md containing that import after review. Do not assume other agents read AGENTS.md: configure their supported instruction mechanism explicitly. No global agent configuration is activated by this document.

## Independent backups

Default schedule: weekly repository/release backup, monthly retained snapshot, quarterly restore check. Use an existing encrypted device/external drive or owner-controlled backup destination; this guide does not configure storage or recurring jobs.

For each repository, clone an independent mirror into a non-public encrypted backup location with `git clone --mirror <repository-url> <backup-directory>`. Refresh it with `git -C <backup-directory> remote update`; retain dated offline snapshots so upstream changes cannot overwrite every recovery point. A Git mirror does not include release assets, issues, Git LFS objects or submodule repositories: back these up separately when used. Preserve releases and checksum files with the associated tags/commits. Keep an encrypted record of required configuration names and recovery procedures; store secret values in a password manager, never in public Git.

Restore to a separate test directory with `git clone <backup-directory> <restore-directory>`, run `git fsck --full`, compare refs and test a clean build. Test release checksums and restore LFS/submodules as needed. Record the actual backup and restore dates privately. No backup is verified until restored.

Back up databases with the database's supported export/snapshot mechanism, encrypted separately from source. Test restore against an isolated database. For local-first browser apps, export user data using the app's backup tools and preserve the browser origin, encryption password and any required file permissions. Git and redeployment do not restore IndexedDB or user documents. Never commit exports or personal content to public or private source repositories.

## Deployment portability

Keep a documented build command, required runtime version and configuration-variable names. Keep provider bindings in adapters/configuration and expose ordinary application interfaces to the core. Record any platform-specific authentication/database assumptions and test replacement adapters before moving providers. Existing Vercel, Cloudflare or VPS deployments remain in place until a destination, migration and rollback are explicitly reviewed. Do not add paid infrastructure as routine maintenance.
