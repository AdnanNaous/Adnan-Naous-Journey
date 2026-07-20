# Contributing

Contributions should improve the accuracy, clarity, reproducibility, or educational value of this learning journey. Read [`AGENTS.md`](AGENTS.md) before making changes.

## Before writing

1. Search for related files, headings, terms, and synonyms.
2. Decide whether to update an existing canonical document or create a genuinely new item.
3. Select the correct content directory and subject.
4. Start from a file in [`templates/`](templates/) when applicable.
5. Remove secrets, private information, and raw conversation content.

## Content expectations

- Use English and clear, direct language.
- Make every document understandable on its own.
- Preserve useful attempts, misconceptions, corrections, and reasoning.
- Cite sources accurately and prefer primary or authoritative references.
- Distinguish verified facts from interpretations and open questions.
- Mark examples and code as Tested, Partially tested, or Untested.
- Do not claim progress or completion without evidence.
- Link to canonical explanations rather than duplicating them.

## Git workflow

Use small, focused changes. A recommended workflow is:

1. Begin from an up-to-date `main` branch.
2. Create a descriptive branch such as `docs/add-networking-notes` or `project/build-cli-calculator`.
3. Make one coherent change and validate it.
4. Review the diff for accuracy, scope, secrets, and accidental files.
5. Update `CHANGELOG.md` for meaningful user-visible changes.
6. Request approval with the mandatory report below.
7. Only after explicit approval, commit with a concise imperative message.
8. Request separate approval before pushing, opening a pull request, merging, or deploying.

Never commit directly because an AI agent suggested it. Never force-push or rewrite shared history without explicit, action-specific approval.

## Mandatory approval report

Before any Git action, report:

1. Objective
2. Files added
3. Files modified
4. Files deleted
5. Important decisions
6. Validation performed
7. Known limitations
8. Risks
9. Proposed commit message

State-changing Git and GitHub actions require explicit user approval. Approval for one action does not authorize later actions.

## Commit messages

Use an imperative summary, preferably 72 characters or fewer. Optional prefixes can clarify scope:

- `docs: add operating systems process notes`
- `learn: document recursion corrections`
- `project: add calculator input validation`
- `challenge: solve binary search variants`
- `chore: update repository templates`

Do not mention an AI tool as the author of the learning unless that fact is materially relevant.

## Review checklist

- Correct location and subject classification
- No duplicate canonical content
- Clear context and reproducible steps
- Honest validation status
- Accurate sources and working relative links
- Useful mistakes and corrections preserved
- No secrets, private data, raw transcripts, or generated clutter
- Changelog updated when appropriate

