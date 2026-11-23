# Recipe: Commit messages, PR descriptions, and code comments

The diff already says what changed. The message says what it is for. A comment earns its line only when it says what the code cannot.

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

## AI edit-summary / commit laundry lists

Wikipedia's *Signs of AI writing* (Edit summaries; among the most common Wikipedia AI signs as of October 2026) names rigid summary formulae that also show up in agent commit and PR text. Cut these:

- **Stacked abstract assurances** — "Improved clarity, flow, and readability… reduced redundancy and refined tone…", "ensure neutrality / improve attribution / comply with guidelines" with no specific change named. Prefer one concrete subject: what broke, what the constraint is, which guideline or ticket if it matters.
- **Procedural preserved / avoided lines** — "Revised X to ensure Y while preserving Z", "avoided changing…", lists of what was *not* edited. Humans rarely advertise non-edits; say what changed and why.
- **Sourcing theater over content** — "Added reliable / secondary / closely attributed sources" with no mention of the fact added. Prefer "Added debut album year from Billboard chart listing" (or the project's equivalent).
- **Markdown / emoji / list formatting** in a one-line summary (older chatbot paste). Keep the repo's plain subject line.

False positives: short project abbreviations (`ce`, `fix typo`, `wip`), a single specific style or ticket cite ("removed overlink per MOS:OVERLINK", "fix SCA-533"), and a brief "why" that names a real constraint.

## Chat residue

Agents write durable text to the person in the chat instead of to whoever reads the history later (ChufanS008/ship-the-result; SilvrDuck/skills defossil; tdkn exclude-prompt-data). It shows up in commit and PR text, comments, test names, and filenames. Cut:

- **Conversation echoes**: "as discussed", "per your feedback", "as requested", "as you asked". Name the change instead: "Fix redirect on expired session", not "Fix redirect as discussed".
- **The rejected draft, kept**: "Add retry logic (without exponential backoff)" when nobody asked for backoff; `test_parser_without_regex`; `grilled_cheese_no_ketchup.md`. A correction limits the work. It is not content for the message.
- **Revision markers**: "(fixed version)", "Sorry, previous commit used the wrong table", `retry_v2.py`, `# Shortened version`.

Test: would the line make sense a year from now to someone who never saw the chat? Keep a negation that describes the artifact ("Allow login without password for SSO users", "Run tests without network access") and a changelog line that compares two shipped versions ("no longer crashes on empty input").

## Inline comments

Comments that narrate the change or restate the next line are a recurring AI code tell (LeonardNJU/code-humanizer; scale-venture-partners/windbag). Keep thin:

- **Restates the next line** — `// increment the counter` above `counter += 1`. Delete.
- **History narration** — "was missing", "used to be", "no longer", ticket IDs embedded as changelog (`// SCA-533 fixed null`). Prefer a comment that states the *current* constraint, or put history in the commit / ticket. Docs twin: `references/patterns.md` #53.
- **Reviewer-facing pep** — "This change ensures correctness", "hopefully this works", "should be fine now". Delete or replace with the invariant.
- **Same-PR TODO theater** — TODO the agent wrote and resolved in the same change. Drop both.

Keep: invariants, why-not-the-obvious-way, security / race / perf constraints, and tracked `TODO(owner): …` the team actually uses.

## Don't

- Invent the why. If motivation isn't in the commits, the issue, or the author's words, ask.
- Report work as tested or verified when it wasn't. Say what you ran and what you skipped (→ `references/evidence-bound.md`).
