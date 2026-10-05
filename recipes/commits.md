# Recipe: Commit messages and PR descriptions

The diff already says what changed. The message says what it is for.

## Defaults

- Follow the repo's convention first (Conventional Commits, scope, gitmoji or none, line length). Don't impose one.
- Subject names the specific thing changed, imperative: "return 429 on rate-limit breach", not "improve error handling".
- Body, when needed, explains why: symptom, cause, constraint, number, issue or incident link.
- Length matches the change. A one-line fix gets a line. A PR description opens with a few sentences of framing (goal, why now) before any detail; a reader can stop early and still be right.

## Cuts that matter most here

- Vague verbs with no object or significance announcements: "improve", "enhance", "update various", "comprehensive update", "major refactor".
- Restating the diff: file-by-file walkthroughs, tables that mirror the code, narrated steps ("first, we… then we… we also…").
- Self-referential openers: "This commit…", "This PR introduces a comprehensive refactor that improves maintainability."
- Decorative emoji where the project doesn't use them.
- Ceremony: headers and checklists that exist to look thorough.

## Don't

- Invent the why. If motivation isn't in the commits, the issue, or the author's words, ask.
- Report work as tested or verified when it wasn't. Say what you ran and what you skipped (→ `references/evidence-bound.md`).
