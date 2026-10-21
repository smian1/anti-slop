# False positives and keep-list

A false positive that flattens a good sentence is worse than one surviving tell. Flag **clusters**, not isolated tells. One measured run of a deterministic detector over 376 human documents found 27% tripped at least one finding and 1.3% tripped more than six (avoid-ai-writing gate calibration, 2026-10-15).

## What not to flag alone

- Perfect grammar / consistent style — professionals and editors exist.
- Mixed casual and formal — field, age, or habit.
- Dry or "bland" prose without specific AI tells — just dry writing.
- Formal or academic vocabulary that is not on the banned Tier-1 list — do not dumb down every precise word.
- Letter-style greetings and sign-offs.
- One *however* / *additionally* — AI-coded only when piled up.
- Curly quotes alone — editors auto-curl; evidence only with other tells.
- Em dashes alone — journalists use them; sample override applies in long essays.
- **No em dashes ≠ clean.** Newer models (Opus 5.5 per Graphite, 2026) almost stopped using them. In Detect, weight phrase frames (`banned-words.md`, Model phrase frames) and grammar (patterns #42–43) over dash count. The no-dash rule for short copy still applies when writing.
- One short sentence for emphasis — flag only stacks of dramatic fragments.
- A list of three alone — keep three items when the meaning has three. A reference set of about a million words of human prose (Project Gutenberg) runs about 5 lists of three per 1,000 words. Rule-of-three padding (#16) is the third item that adds nothing, or triads stacked paragraph after paragraph.
- *Not only… but also* / *not X but Y* alone — ordinary correlatives. In one human-vs-machine corpus count, "not only… but" showed up 16 times in 143k human words and 5 times in 115k machine words. The binary-contrast tell (#7) is the minimizer-then-upgrade reveal (*isn't just X, it's Y*) or plain corrections stacked a few sentences apart.
- Modal plus negation (*could not possibly*, *might never*) — plain emphasis, not a qualifier stack (#35). In one human-corpus check, 3 of 4 hedge-stack flags were this over-match. The stack is *could potentially*, *may eventually*.
- Deliberate repeated openings that build rhythm ("She came. She saw…") when they earn it.
- *Honestly* / *look* mid-sentence — ordinary speech; theatrical standalone openers are the tell.
- Useful limits, legal/safety notices, real corrections, named FAQ answers.
- Real design alternatives the reader may choose — cut only fake alternatives set up to dismiss.
- Unsourced claims — common on the web; not proof of AI.
- Clean formatting from templates/CMSes.
- Quoted / titled / exemplified phrases being discussed, not used.
- Text clearly predating Nov 30, 2022 (ChatGPT public launch) — almost never model-written.

## Keep — voice, not slop

- Earned fragments after a long sentence, used sparingly.
- Deliberate parallelism the author would defend.
- Strong closing lines that are concrete, not aphorism kitsch.
- First-person conviction: *We think…*, *I'm not comfortable saying…*
- Bluntness, humor, profanity, self-interruptions, honest admissions that belong to the writer.
- Mixed feelings and unresolved tension.
- Specific unusual details, dated slang, genuine parentheticals/self-corrections.
- Non-native English choices that are clear and intentional (detectors over-flag ELL writing — do not "fix" accent or atypical grammar into generic Mid-Atlantic).
- Neurodivergent rhythm / info-dump density when it is the author's real cadence — cut formula, not cognition.
- Scientific domain terms (*weighted interval score*, gene names) — precision ≠ jargon.
- Legitimate *associated with* / *linked to* in science, epidemiology, or sourcing when the relationship is genuinely unknown or statistical — cut only when it hides a concrete role the source already names.
- Semicolons and complex punctuation (not a tell).
- Parentheses (allowed).

## Validation questions before cutting

1. Does cutting lose meaning? → keep or reword.
2. Formula or author choice they'd defend?
3. Announce rather than deliver?
4. Heat or light? Cut heat.
5. Would a skeptical reader trust the sentence more without it?

If it survives all five, leave it.

## Over-edit failure

Already-strong human text often wants a light edit or **leave alone**. Changing more than ~1/5 of a control sample without clear reason is a warning. Do not replace AI slop with a new formula (clipped aphorisms, tidy triads, consultant voice).
