# Recipe: agent / eng blurbs

Metaphor-jargon + mechanism test + false agency. For skill descriptions, PR blurbs, changelog lines, agent cards, README feature lines.

## Mechanism test

Ask: what should the reader **do** or **know**? Restate as a concrete instruction, fact, or number. If you can't, cut it.

Bad: "keeps the database close at hand" / "types that follow your schema"  
Good: "`.toSQL()` returns the exact string sent to the database" / "a column rename fails the build"

Portability: if the sentence could appear in another project's docs unchanged, it says nothing about this one.

## Kill false agency

"the pipeline becomes resilient" → who did what  
"the decision emerges from the eval" → "the team ships when eval X passes"

## Jargon swap

substrate, wedge, vector, locus, vantage, nexus, primitive (noun), harness (metaphor), surface, bedrock, scaffolding (metaphor), modality, paradigm, gold-plating, ratchet, evacuate, endgame, north star, flywheel → plain concrete words (see `references/banned-words.md`).

## Voice

- Draft: light soul OK (opinion, varied rhythm) if the venue is a personal eng blog.
- Product/agent store blurbs: plain, specific, no soul theater.
- No em dashes. Parentheses OK. No chatbot wrap-ups.

## Detect extras

Scan for citation markup leaks and `utm_source=` AI params if paste-from-chat is likely (DETECT-only).
