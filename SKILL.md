---
name: Anti-slop
description: >-
  Use this when writing or editing prose (digests, Slack, org copy, agent blurbs,
  social) so it does not read as AI. Edit, Detect, Draft, and related modes cut
  AI patterns while preserving the writer's voice.
---

# Anti-slop

Sharp human editor for prose. Cut AI patterns. Keep edge, humor, and uncertainty. Invent nothing. Skill id: `anti-slop`.

Load `references/` only when needed. Load a `recipes/` file when the venue matches.

## Modes

| Mode | When | Do |
|------|------|----|
| **Edit** (default) | User pastes a draft | Minimum phrasing change. Slop-vs-voice triage. Return full draft + short **What changed**. |
| **Detect** | Audit / "is this slop?" | Name pattern, quote line, short fix. No rewrite, no AI-authorship guess, no score. Forensic leaks (citation markup, unicode obfuscation) are DETECT-only. |
| **Draft** | Write from scratch | Apply cuts while writing. Lead with the fact. Light soul OK. No What changed unless editing a user draft. |
| **Evidence-bound** | Vague marketing/support/incident/recruiting | Gaps and questions, not invented owners/metrics/workflows. See `references/evidence-bound.md`. |
| **Publish** | Optional gate before ship | Run `references/eval.md` pass/fail + optional density questions. One checklist only — do not mix competing numeric scales. |
| **File** | Named file / embedded | Rewrite prose only. Keep code, YAML, data, link targets. Short summary after. |

Always-on only for dedicated writing agents. Coding agents: on-demand Edit/Detect.

## Non-negotiables

1. Invent no facts, quotes, stats, owners, metrics, or promises.
2. Concrete names, numbers, mechanisms. Portability test: if a sentence could move to another product unchanged, cut or specify. Mechanism test: say what it does, not how it feels.
3. Cut binary contrasts, throat-clearing, faux-insight, puffery, weasel attribution, synonym cycling, rule-of-three padding, dramatic fragment stacks, fake-profound endings, summary-recap endings, decorative emoji/bold/title-case.
4. Active voice; kill false agency ("the decision emerges"). Passive OK when actor unknown (methods/incidents).
5. No em dashes by default (Slack/digests/blurbs). Parentheses **allowed**. Sample may restore dashes in long essays. Semicolons fine.
6. Preserve the writer's edge, humor, and uncertainty. Do not professionalize blunt lines.
7. Chatbot residue out: "I hope this helps!", "Great question!", "Certainly!", "As an AI…".
8. Cut empty adverbs; KEEP voice-bearing (*actually*, *honestly*, *I think*).
9. Wh-openers: soft preference for subject-led headlines only — not a hard ban.
10. Brief ≠ artifact: instructions about the piece stay out of the piece.

## Edit triage

1. Read whole draft. Note voice: bluntness, humor, cadence, polish.
2. Collect candidates. Do not edit yet.
3. For each: slop or voice? False positive that flattens > surviving tell. When unsure, leave it.
4. Surgical phrasing only. Facts, numbers, structure untouched unless asked.
5. Self-check against `references/eval.md`. Output draft + **What changed** (pattern category per change).

## Draft notes

- Digests / video summaries → `recipes/digests.md` (title, who, length, what happened; no lesson closer).
- Slack → `recipes/slack.md`. Org/legal → `recipes/org-copy.md` + evidence-bound.
- Agent/eng blurbs → `recipes/agent-blurbs.md` (metaphor-jargon + false agency).
- Tweets/LinkedIn → `recipes/social.md` (anti-parataxis for long prose; fragments OK in short Slack).
- Manuscripts/grants → `recipes/scientific.md`.

## Style decisions

| Topic | Decision |
|-------|----------|
| Em dashes | None in short copy; sample may restore in essays; parentheses allowed. |
| Fragments / parataxis | Sparse OK in Draft/Slack; long essays prefer connected prose. Flag staccato *stacks*, not every short sentence. |
| Adverbs | Cut empty; keep voice-bearing. No absolute adverb ban. |
| Wh- starters | Soft preference for subject-led headlines. |
| Soul | Edit = preserve; Draft = light soul; Org/legal = no soul inject. |
| Scoring | Pass/fail checklist + optional density questions. One scale only. |
| Pattern catalogs | One pattern + false-positive reference set; forensic extras are DETECT-only — not a second always-loaded catalog. |

## Reference map

- `references/banned-words.md` — vocab + phrases + chatbot openers
- `references/patterns.md` — pattern cards
- `references/false-positives.md` — keep-list + neurodiversity caution
- `references/evidence-bound.md` — fabrication guardrails
- `references/voice-and-soul.md` — preserve vs inject; sample override
- `references/eval.md` — post-edit checklist + optional publish density
