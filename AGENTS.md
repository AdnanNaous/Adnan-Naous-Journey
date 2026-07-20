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

# Learning Capture and Authorship Protocol

This repository must document my real learning journey, but it must not require me to write a complete explanation every time.

I may provide learning material in several forms:

- A complete explanation in my own words
- Short or incomplete notes
- A list of topics
- A screenshot
- A course slide
- A document
- A video, article, chapter, lesson, or source
- Code I wrote
- An exercise attempt
- A brief statement such as “I learned these concepts today”
- A mixture of Arabic and English
- Informal language, fragmented sentences, or voice-transcribed text

The agent must adapt its workflow to the amount and quality of information I provide.

## 1. Core Principle

The repository must distinguish between:

1. What I explicitly said or demonstrated
2. What the agent inferred from my material
3. What came from an external source
4. What the agent added as an academic explanation
5. What has not yet been confirmed as part of my understanding

The agent must never present AI-generated or source-derived material as if I personally explained, understood, or mastered it.

The goal is to preserve my intellectual contribution while also reducing unnecessary documentation effort.

## 2. Learning Input Modes

The agent must identify the most appropriate input mode before processing the entry.

### Mode A — Full Personal Explanation

Use this mode when I provide a substantial explanation in my own words.

The agent should:

- Preserve my meaning and reasoning
- Translate my explanation into clear English
- Assess accuracy
- Identify misconceptions and gaps
- Create a separate academic explanation
- Preserve useful examples, uncertainty, and mistakes
- Avoid replacing my explanation with generic textbook content

### Mode B — Partial Personal Notes

Use this mode when I provide short, incomplete, fragmented, or informal notes.

The agent should:

- Reconstruct only what can reasonably be derived from my words
- Preserve uncertainty
- Ask a small number of focused questions only when the missing information materially affects accuracy
- Prefer two to five concise questions
- Avoid broad interviews or unnecessary questioning
- Use my answers to produce the faithful English version
- Clearly label any interpretation or inference

The agent must not pretend that incomplete notes represent a complete understanding.

### Mode C — Source-Assisted Learning Capture

Use this mode when I provide a source such as:

- Video
- Screenshot
- Lecture slide
- Document
- Article
- Course chapter
- Website
- Code example
- Assignment material

The agent should:

1. Analyze the source
2. Extract the main topics
3. Identify the concepts that were likely presented
4. Separate source content from my confirmed understanding
5. Ask a few focused questions when necessary
6. Produce a structured learning entry
7. Clearly mark which material came from the source
8. Avoid claiming I understood every topic merely because it appeared in the source

The agent may create a provisional learning entry when my understanding has not yet been confirmed.

Use labels such as:

- `Source Content`
- `My Confirmed Understanding`
- `Agent Inference`
- `Needs Confirmation`

### Mode D — Minimal-Effort Learning Log

Use this mode when I am tired, busy, or only want to record a small learning event.

Examples:

- “I learned about Java operators today.”
- “We studied arrays.”
- “I understood the difference between commit and push.”
- “Add these three concepts to my journey.”
- “I watched this lesson; record the important parts.”

The agent should not force me to write a complete explanation.

Instead, it should:

- Record the topic
- Extract or infer the minimum safe context
- Ask no questions when the entry can be accurately documented without them
- Ask only essential questions when needed
- Create a concise entry rather than an artificially long document
- Mark the depth of understanding honestly
- Add a future-review or practice item when appropriate

Small learning events should remain small. Do not inflate simple concepts into large academic chapters.

## 3. Required Authorship Layers

When enough personal input exists, substantial learning entries should contain the following layers.

### My Original Input

Preserve my original wording when it has educational value.

This section may contain Arabic, mixed language, informal language, mistakes, or incomplete phrasing.

Do not preserve unnecessary repetition, private information, or irrelevant conversation.

### My Understanding — Faithful English Version

Create a clear English reconstruction of what I personally expressed.

Requirements:

- Preserve my meaning
- Preserve my level of understanding
- Preserve uncertainty
- Preserve useful mistakes or misconceptions
- Correct language without falsely improving the technical depth
- Do not introduce ideas I did not express
- Do not make me appear more advanced than the evidence supports

### Understanding Assessment

Separate the assessment into:

- Correct points
- Inaccuracies or misconceptions
- Missing concepts
- Unclear or unconfirmed points

### Academic Explanation

Create a separate technically accurate explanation in formal academic English.

This section may:

- Correct technical errors
- Add important context
- Explain terminology
- Show examples
- Connect the topic to related concepts
- Explain limitations and common mistakes

This section must not be presented as my original explanation.

## 4. Source-Derived Entries

When the entry is based mainly on a source and not on my own explanation, use a structure such as:

```markdown
# Topic

## Learning Context

## Source Summary

## Concepts Presented

## My Confirmed Understanding

## Unconfirmed or Inferred Understanding

## Academic Explanation

## Examples

## Practice or Review Questions

## Sources
```

If I have not confirmed my understanding, do not create a misleading `My Understanding — Faithful English Version`.

Instead, use:

`## My Confirmed Understanding`

and include only what I explicitly demonstrated or confirmed.

## 5. Questioning Policy

The agent should ask questions only when they improve the accuracy or educational value of the entry.

Questions must be:

- Focused
- Limited in number
- Directly related to the topic
- Designed to test understanding rather than collect unnecessary detail

Prefer questions such as:

1. How would you explain this concept in one sentence?
2. What problem does it solve?
3. Can you give one example?
4. What part is still unclear?
5. How is it different from a related concept?

Do not ask questions when:

- The learning event is simple
- The provided material is already sufficient
- I explicitly ask for a quick entry
- The questions would add more effort than educational value
- The entry can be marked honestly as partial or provisional

## 6. Automatic Completion Rules

The agent may automatically complete structure, grammar, formatting, examples, terminology, and academic context.

The agent may also:

- Summarize a source
- Extract topic names
- Organize fragmented notes
- Add definitions
- Add common mistakes
- Add practice questions
- Add connections to earlier repository content
- Add source references
- Suggest a review task

However, the agent must not automatically invent:

- My personal interpretation
- My level of confidence
- My examples
- My conclusions
- My mistakes
- My experience
- My mastery
- My completion of exercises
- My agreement with the source

Anything not directly supported by my input must be labeled as source-derived, inferred, suggested, or unconfirmed.

## 7. Learning Depth Labels

Each learning entry may include a learning-status label.

Recommended values:

- `Exposed` — I encountered the topic
- `Introduced` — I understand the basic definition
- `Developing` — I can explain parts of it but still have gaps
- `Practiced` — I applied it in an exercise or example
- `Applied` — I used it in a project
- `Reviewed` — I revisited and corrected the topic
- `Verified` — I demonstrated accurate understanding through explanation or practice

Do not assign `Applied`, `Reviewed`, or `Verified` without evidence.

## 8. Concision and Proportionality

The length and depth of the repository entry must match the significance of the learning event.

Examples:

- A simple command may require only a short note.
- A language concept may require a structured learning entry.
- A completed exercise may require the problem, attempt, correction, and explanation.
- A major project may require full project documentation.
- A video covering many unrelated topics may require multiple entries or a course-note summary.

Do not create long, repetitive, or generic content merely to make the repository appear larger.

## 9. Language Policy

My input may be written in Arabic, English, or a mixture of both.

The repository documentation should normally be written in English.

The agent should:

- Translate my words faithfully
- Preserve technical terminology accurately
- Retain Arabic terminology in parentheses only when educationally useful
- Avoid literal translations that distort meaning
- Keep the faithful translation separate from the academic rewrite

## 10. Recommended Processing Workflow

For every learning submission:

1. Read the relevant repository instructions
2. Identify the input mode
3. Inspect related existing files
4. Determine whether to create or update content
5. Separate personal input, source content, inference, and academic additions
6. Ask only essential questions
7. Create a proportional learning entry
8. Validate technical claims and code
9. Update progress records only when justified
10. Provide the required review summary
11. Do not commit or push without explicit approval

## 11. Examples

### Example: Full Explanation

Input:

“I learned that a Java variable has a type and stores a value. I think its type can change later.”

Expected behavior:

- Preserve the explanation
- Translate it faithfully
- Mark the claim about changing the type as incorrect
- Explain static typing academically

### Example: Short Note

Input:

“Today I learned Java arithmetic operators.”

Expected behavior:

- Create a concise entry
- Cover the operators actually mentioned or present in the supplied material
- Do not claim full mastery
- Add a small review question if useful

### Example: Screenshot

Input:

“Add what I learned from this screenshot.”

Expected behavior:

- Analyze the screenshot
- Extract the visible concepts
- Mark them as source content
- Ask one or two confirmation questions only if needed
- Avoid claiming that all visible content was understood

### Example: Video

Input:

“I watched this lesson. Extract the important topics and add what I learned.”

Expected behavior:

- Analyze the lesson or available transcript
- Create a source summary
- Extract major concepts
- Ask focused questions when confirmation is necessary
- Separate source coverage from confirmed personal understanding

### Example: Tired or Minimal Input

Input:

“I am tired. We learned arrays today. Just record it properly.”

Expected behavior:

- Create a concise provisional entry
- Record the topic and learning context
- Mark the status as `Exposed` or `Introduced`
- Avoid forcing a full explanation
- Add an optional future review task

## 12. Human Control

Before modifying files, explain the intended classification and file plan when the change is substantial.

After modifying files, provide:

- Objective
- Input mode used
- Files added
- Files modified
- Personal content preserved
- Source-derived content added
- Agent inferences
- Academic additions
- Validation performed
- Unconfirmed points
- Proposed commit message

Do not stage, commit, or push until I explicitly approve.

## Simple User Summary

After processing any learning entry, always give me a short and simple summary first.

The summary should explain:

- What I learned
- Whether my understanding was correct
- What file was created or updated
- Whether anything still needs clarification
- Whether the changes are ready for approval

Keep this summary concise and easy to read.

Use this format:

```markdown
## Simple Summary

- Topic: [topic]
- Your understanding: Correct / Mostly correct / Partially correct / Needs correction
- Repository action: Created [file] / Updated [file]
- Important correction: [one short sentence, or “None”]
- Needs clarification: [yes/no and short reason]
- Status: Ready for review / Waiting for your answer
```

After the simple summary, provide the full technical review required by `AGENTS.md`.

Do not commit or push without my explicit approval.

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
