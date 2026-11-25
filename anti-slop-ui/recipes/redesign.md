# Recipe: Redesign in place

Restyle without a product rewrite. Surgical anti-slop, not a theme swap.

## Defaults

- **Edit** mode. Preserve routes, IA, real copy, and data bindings.
- Diff should read as "removed defaults," not "new brand."
- If brand is undefined, propose DESIGN.md stub — don't invent a full identity mid-PR.
- Run `references/ui-checklist.md` before claiming done.

## Triage order

1. Color defaults (gradient systems, unearned purple/cream kits)
2. Type defaults (Inter monoculture, eyebrow spam / hero pill above H1)
3. Material soup (glass/glow/shadow)
4. Layout templates (equal cards, nested cards, side stripes)
5. Honesty (fake metrics/chrome) — flag; fix only with real sources
6. Motion (loops, elastic, per-section fade-up)

## Keep

- Existing brand tokens and intentional accents
- Asymmetric layouts that already reflect content
- Working interaction states
- Anything that makes data or state faster to read (a chart's area fill, a large condition icon), even when it looks generated. Before accepting each fix, ask whether the page reads faster after it; if the AI-looking version reads faster, keep it. A page built with care may need no changes: in one blind before/after test, 3 of 3 judges preferred the untouched original of a hand-built dashboard over the de-slopped version

## Don't

- Drive-by IA changes or copy rewrites unless asked
- Move, rename, or remove a control people already use. A restyle keeps every existing action where it was and under the same name; if one must move, say where it went. In 1,200 hand-labelled low-rated app reviews (from 5M on the App Store and Google Play), about 5 to 7% complained that a redesign moved or removed something, while purple gradients almost never came up
- Crown a new default font for the whole app
- "Polish" by adding decoration
- Loop "make it look less AI" over the same page. Make one pass, run `references/ui-checklist.md`, and run another pass only to fix a named failing item. In a 10-edit test (DesignArena, Nov 2026: four frontier models, each edit a fresh call on the latest HTML), every model's own judge called its page fixed after edit 1, yet later edits kept rewriting working layouts (one model changed about four times as much per edit as another), one model drifted into pale beige pages with serif headlines, and one page grew to 9.5 times its text with invented backstory that the same model's judge then cited as a reason to score it clean
- Merge-dump a taste-skill theme pack

## Output

Full changed surfaces + **What changed** (pattern category each). List overrides you respected.
