# UI tell cards

Load for Edit/Detect depth. SKILL.md already covers non-negotiables.

Format: **Tell** · **Why** · **Fix**. Cite file, selector, or region when Detecting.

## Color & material

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 1 | **Purple / indigo / cyan–pink gradient system** as primary treatment | Training-set default; signals no brand | Pull palette from DESIGN.md; keep gradient only with a written hierarchy job |
| 2 | **Mesh / orb / blurred radial blobs** behind hero | Same default family as gradient wash | Solid or brand texture; or one purposeful light if DESIGN.md allows |
| 3 | **Gradient-clipped headline text** | Instant "AI SaaS" read | Solid type; accent a whole line or none |
| 4 | **Glass / backdrop-blur everywhere** | Flattened hierarchy; frosted wallpaper | ≤1–2 glass surfaces as accent |
| 5 | **Glow / neon / soft multi-shadow soup** | Attention amplifier with no focus | Shadow for elevation only; glow on one focus element max |
| 6 | **Cream + serif + terracotta / beige–brass kit** unearned | 2026 AI cluster (Claude-beige adjacent) | Brand override only; else pick tokens for this product |
| 7 | **Near-black + acid-green / vermilion accent kit** unearned | 2026 AI cluster twin of cream kit | Brand/product category override only; else derive accent from subject |
| 8 | **Broadsheet / newspaper kit** unearned — hairline rules, zero border-radius, dense multi-column “print” layout | 2026 AI cluster look #3 (sibling of cream + acid-dark) | Brand/editorial brief only; else derive layout from subject, not the print costume |
| 9 | **Too many accents** — accent on buttons, icons, badges, links, glows at once | Accent stops being accent | One accent job; neutrals carry area; status colors only on status |

## Type

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 10 | **Inter / Roboto / Open Sans / Space Grotesk / Geist / Instrument Serif** (or unstated system stack) as unearned identity | Font monoculture / default roster | DESIGN.md / project fonts; do not crown a replacement default |
| 11 | **Tracked ALL-CAPS eyebrows** above every heading | Template chrome | Cut or keep once when the label is real taxonomy |
| 12 | **Single-word headline accent** — one word italic, bold, or color-dipped; two-tone H1 | Trying-to-look-editorial costume | Solid roman headline; emphasis via weight/size of the whole line |
| 13 | **Monospace-as-aesthetic** — mono headings, fake terminal hero, *or* mono on every small data/meta label | Developer/template costume | Real screenshot or brand type; mono only for real code/data UI |

## Layout & components

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 14 | **Hero → logos → 3 features → how-it-works(3) → testimonials → FAQ → purple CTA** | Narrative from template, not product | Section order from content; drop empty sections |
| 15 | **Hero-metric template** — huge number, tiny label, supporting stats as the hero | Layout picked from memory, not the product | Lead with product/artifact/verified claim; keep metrics only when real and primary |
| 16 | **Three identical icon+title+blurb cards** (often icon-tile on top) | Equal weight for unequal content | Vary size/treatment; flagship may be full-width; drop decorative icon tiles |
| 17 | **Nested cards / card-everything** | Soft rectangles as personality | Flat sections; cards only for discrete objects |
| 18 | **SaaS-card kit shadow** — identical rounded cards each with the same soft grey shadow (`rgba(0,0,0,.1)`), one radius everywhere, optional gradient wash | Anthropic cluster SaaS-card fingerprint | Elevation only where hierarchy needs it; vary or drop shadow; radius scale |
| 19 | **Side-tab / thick colored edge stripe** with no state meaning | Cheap "designed" cue | Stripe only for real state (active, warning, selected) |
| 20 | **01 / 02 / 03 section theater** | Numbers when content is not a sequence | Number only real steps/timelines |
| 21 | **Uniform pill radius on every control** | Hierarchy erased | Radius scale; CTA may be rounder than inputs |
| 22 | **Same radius on parent and padded child** | Concentric fail; visually muddy | Inner radius = outer − padding (approx) |
| 23 | **Default dashboard shell** — sidebar + 4 stat cards + chart + table before the job is named | App-side template mean | Name the user decision; build hierarchy around it |

## Decoration & content honesty

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 24 | **Emoji / sparkle / ✨ / 🚀 as icons or CTA flair** | Loudest "generated" shorthand | Real SVG/set icons or none |
| 25 | **"AI Powered" / glow capsule badges** (pill + glow + dot + uppercase) | Self-referential AI costume | Real status only (Beta/New when true); never decorative "AI Powered" |
| 26 | **Generic stock illustrations** — Undraw / Storyset / blob characters with no product link | Decorated, not designed | Real screenshot, domain diagram, or none |
| 27 | **Fake metrics / Jane Doe activity / invented logos** | Fabricated trust | Real data, labelled placeholder, or honest empty |
| 28 | **Div-built fake product chrome** (traffic-light windows, pretend UI) | Costume screenshot | Real capture or abstract diagram labelled as such |
| 29 | **Arrow on every button** (`→` / `↗`) | Direction cue becomes noise | Arrow only when navigation direction matters |
| 30 | **UI copy chrome** — em dashes in short UI strings; middle-dot meta (`A · B · C`); `WORD — fragment` labels | Anthropic template chrome; bleeds from prose slop | Sentence case; cut theater punctuation; for long landing prose see sibling `anti-slop` |
| 31 | **Tinted near-black ink** (`#0B0B0B`, `#111`) standing in for black across the page | Template chrome; reads “AI default dark” independent of subject | Token ink / true black, or brand-specified near-black with a written reason |

## Motion

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 32 | **Bounce / elastic easing** as default | Toy motion on serious UI | Standard ease; spring only if brand asks |
| 33 | **Infinite pulse / float loops** without user trigger | Perpetual noise | One authored moment; stop; honor `prefers-reduced-motion` |
| 34 | **Fade-up on every section + hover on every card** | Scattered motion, no focal point | Choreograph one entrance or none |

## Positive defaults (short)

- Palette, type, radius, spacing from DESIGN.md or existing tokens
- Hierarchy via size, weight, and space before decoration
- Layout follows content shape
- Full states: hover, focus-visible, disabled, loading, empty, error
- Companion brands: point at project DESIGN.md or [getdesign.md](https://getdesign.md) collections — do not fork brand packs into this skill
