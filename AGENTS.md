# Operational Instructions for AI Agents

## Purpose and scope

This file is the authoritative repository-wide guide for Codex, Claude Code, Cursor, Antigravity, other AI agents, automation, and human contributors. Work from the repository contents and the user's current request. Never assume access to previous chats or private context.

More specific `AGENTS.md` files may be added inside subdirectories. They may refine local procedures but must not weaken the safety, truthfulness, privacy, or approval requirements in this file.

## Instruction priority

1. The user's current explicit instructions.
2. The nearest applicable `AGENTS.md` file.
3. Root `AGENTS.md`.
4. [`CONTRIBUTING.md`](CONTRIBUTING.md) and local documentation.
5. Tool defaults and general conventions.

If instructions conflict materially, stop and ask the user before making an irreversible or high-impact change.

## Required workflow

1. Read this file and the relevant directory `README.md` files.
2. Inspect repository status and existing related files before proposing changes.
3. Search by concept, filename, and likely synonyms before creating content.
4. State assumptions when requirements are ambiguous; ask only when a choice would materially change the outcome.
5. Make the smallest coherent change that fulfills the request.
6. Preserve relevant attempts, mistakes, corrections, and personal reasoning.
7. Validate technical claims, examples, links, and code in proportion to risk.
8. Label validation status precisely.
9. Summarize changes, validation, limitations, and risks.

## Content architecture

- Put structured study material in `learning/<subject>/`.
- Put standalone builds in `projects/<project-name>/`.
- Put exercises in `challenges/<subject>/<challenge-name>/`.
- Put concise reference notes in `notes/<subject>/`.
- Put evaluated sources in `resources/<subject>/`.
- Put dated evidence and reviews in `progress/`.
- Put reusable starting points in `templates/`.
- Put superseded or inactive content in `archive/`, preserving context.

Use English only. Use lowercase kebab-case for directories and filenames, except conventional root files such as `README.md`, `AGENTS.md`, `CONTRIBUTING.md`, and `CHANGELOG.md`.

Do not create multiple files that explain the same concept independently. Prefer improving the canonical file and adding cross-links. When moving or superseding material, repair incoming links where practical.

## Knowledge-capture rules

- Never store raw AI or human conversation transcripts directly.
- Extract durable knowledge into self-contained documentation with enough context to stand alone.
- Separate facts, interpretations, personal reasoning, and open questions.
- Preserve failed attempts when they explain a misconception, tradeoff, or correction.
- Do not rewrite history to make the learning path appear cleaner than it was.
- Use dates only when useful; a date is not a substitute for subject classification.
- Cite primary or authoritative sources when a claim depends on external material.
- Never invent or embellish citations.

## Technical accuracy and validation

For code or technical instructions:

- Record prerequisites, versions, platform assumptions, and commands needed to reproduce results.
- Run the narrowest relevant checks when execution is safe and available.
- Do not claim that code works because it looks correct.
- Distinguish `Tested`, `Partially tested`, and `Untested` results.
- Record exact failed checks when useful; do not conceal failures.
- If verification is unavailable, explain why and identify the remaining check.
- Never fabricate benchmark numbers, output, progress, completion, tests, or achievements.

## Privacy and security

Never add credentials, tokens, private keys, session data, `.env` values, private conversations, personal identifiers not intentionally made public, or confidential material. Use obvious placeholders such as `YOUR_API_KEY` in examples. Check proposed changes for secrets before any commit request.

Do not introduce destructive commands, hidden telemetry, unsafe downloads, or unexplained privilege escalation. Treat copied code and dependencies as untrusted until reviewed.

## Approval boundaries

Without the user's explicit approval, do not:

- commit, amend, tag, push, force-push, merge, rebase, deploy, publish, or open/merge a pull request;
- delete substantial content or rewrite repository history;
- send data to external services;
- add secrets or private information.

Read-only inspection and local file edits requested by the user are allowed. Keep changes reviewable and reversible.

## Mandatory pre-Git-action report

Before any Git command or GitHub action, present this report and wait for explicit approval if the action can change local history, the index, branches, tags, remotes, or remote state:

1. **Objective**
2. **Files added**
3. **Files modified**
4. **Files deleted**
5. **Important decisions**
6. **Validation performed**
7. **Known limitations**
8. **Risks**
9. **Proposed commit message**

For a read-only Git inspection requested as part of diagnosis, provide the report before the command when practical; if the inventory is not yet knowable, state that the command is read-only and provide the complete report before any state-changing Git action.

Approval applies only to the described action and scope. A commit approval is not automatically push, merge, deploy, or deletion approval.

## Completion standard

A task is complete only when:

- requested files are present in the correct location;
- related content was checked for duplication;
- documentation is understandable without chat history;
- technical claims and code have an honest validation status;
- links and structure were checked;
- no secret or private data was introduced;
- changes, limitations, and risks are reported accurately.

