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
| 6 | **Cream + serif + terracotta / beige–brass kit** unearned (also cream+sage+charcoal anti-purple twin) | 2026 AI cluster (Claude-beige adjacent); sage swap is the same second-order default | Brand override only; else pick tokens for this product |
| 7 | **Near-black + acid-green / vermilion accent kit** unearned | 2026 AI cluster twin of cream kit | Brand/product category override only; else derive accent from subject |
| 8 | **Broadsheet / newspaper kit** unearned — hairline rules, zero border-radius, dense multi-column “print” layout | 2026 AI cluster look #3 (sibling of cream + acid-dark) | Brand/editorial brief only; else derive layout from subject, not the print costume |
| 9 | **Too many accents** — accent on buttons, icons, badges, links, glows at once | Accent stops being accent | One accent job; neutrals carry area; status colors only on status |
| 10 | **Low-contrast muted body** — `gray-400/500` / `slate-400` body on white or dark | AI default + WCAG fail; secondary grey used as primary text | Near-black body on light (≥ gray-700 / ~#1a1a1a); light body on dark (≥ slate-200); grey only for true metadata |
| 11 | **Unearned dark-only / unmodified zinc–violet SaaS shell** — forced dark page, zinc-950/900/800 + violet accent, no light theme | "Dark = premium" starter stack; hides layout sins | Default light unless the product lives at night; temperature the neutrals; replace violet with brand accent |

## Type

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 12 | **Inter / Roboto / Open Sans / Space Grotesk / Geist / Instrument Serif** (or unstated system stack) as unearned identity | Font monoculture / default roster | DESIGN.md / project fonts; do not crown a replacement default |
| 13 | **Tracked ALL-CAPS eyebrows** above every heading | Template chrome | Cut or keep once when the label is real taxonomy |
| 14 | **Single-word headline accent** — one word italic, bold, or color-dipped; two-tone H1 | Trying-to-look-editorial costume | Solid roman headline; emphasis via weight/size of the whole line |
| 15 | **Monospace-as-aesthetic** — mono headings, fake terminal hero, *or* mono on every small data/meta label | Developer/template costume | Real screenshot or brand type; mono only for real code/data UI |

## Layout & components

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 16 | **Hero → logos → 3 features → how-it-works(3) → testimonials → FAQ → purple CTA** | Narrative from template, not product | Section order from content; drop empty sections |
| 17 | **Hero-metric template** — huge number, tiny label, supporting stats as the hero | Layout picked from memory, not the product | Lead with product/artifact/verified claim; keep metrics only when real and primary |
| 18 | **Three identical icon+title+blurb cards** (often icon-tile on top) | Equal weight for unequal content | Vary size/treatment; flagship may be full-width; drop decorative icon tiles |
| 19 | **Nested cards / card-everything** | Soft rectangles as personality | Flat sections; cards only for discrete objects |
| 20 | **SaaS-card kit shadow** — identical rounded cards each with the same soft grey shadow (`rgba(0,0,0,.1)`), one radius everywhere, optional gradient wash | Anthropic cluster SaaS-card fingerprint | Elevation only where hierarchy needs it; vary or drop shadow; radius scale |
| 21 | **Side-tab / thick colored edge stripe** with no state meaning | Cheap "designed" cue | Stripe only for real state (active, warning, selected) |
| 22 | **01 / 02 / 03 section theater** | Numbers when content is not a sequence | Number only real steps/timelines |
| 23 | **Uniform pill radius on every control** | Hierarchy erased | Radius scale; CTA may be rounder than inputs |
| 24 | **Same radius on parent and padded child** | Concentric fail; visually muddy | Inner radius = outer − padding (approx) |
| 25 | **Default dashboard shell** — sidebar + 4 stat cards + chart + table before the job is named | App-side template mean | Name the user decision; build hierarchy around it |
| 26 | **"Most Popular" pricing theater** — three tiers, middle one ringed/scaled with a capsule badge | Default SaaS pricing shape, not a plan decision | Use the real plan count/structure; highlight only when the offer earns it |
| 27 | **Four-column template footer** — equal link columns + newsletter + social row by reflex | Universal generated footer whether or not the links exist | Build from real IA; fewer columns or a single link line is fine |
| 28 | **Dual equal hero CTAs** — same-size "Get Started" + "Learn More" (or solid + ghost twins) | Starter hero fingerprint; secondary is a non-action | One dominant CTA; demote secondary to a text link with a real label |
| 29 | **Sticky frosted starter nav** — logo / centered links / right CTA / `backdrop-blur` translucent bar by reflex | Universal shadcn/v0 header costume | Solid or transparent-over-hero; no reflexive blur; place links for this product |

## Decoration & content honesty

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 30 | **Emoji / sparkle / ✨ / 🚀 as icons or CTA flair** | Loudest "generated" shorthand | Real SVG/set icons or none |
| 31 | **"AI Powered" / glow capsule badges** (pill + glow + dot + uppercase) | Self-referential AI costume | Real status only (Beta/New when true); never decorative "AI Powered" |
| 32 | **Generic stock illustrations** — Undraw / Storyset / blob characters, *or* Corporate Memphis / Alegria noodle-limb flat people with no product link | Decorated, not designed; Memphis is the pre-AI twin of the blob pack | Real screenshot, domain diagram, distinctive commissioned style, or none |
| 33 | **Fake metrics / Jane Doe activity / invented logos** | Fabricated trust | Real data, labelled placeholder, or honest empty |
| 34 | **Div-built fake product chrome** — traffic-light windows, pretend UI, *or* tilted/isometric floating browser frames with invented dashboards | Costume screenshot; the tilt-frame is the same lie at an angle | Real capture flat and legible, or abstract diagram labelled as such |
| 35 | **Arrow on every button** (`→` / `↗`) | Direction cue becomes noise | Arrow only when navigation direction matters |
| 36 | **Scroll cues** — "Scroll to explore", "Swipe down", bouncing chevron, animated mouse-wheel icon | Labels a behavior the user already knows; hero costume | Cut; let fold composition imply continuation |
| 37 | **UI copy chrome** — em dashes in short UI strings; middle-dot meta (`A · B · C`); `WORD — fragment` labels | Anthropic template chrome; bleeds from prose slop | Sentence case; cut theater punctuation; for long landing prose see sibling `anti-slop` |
| 38 | **Tinted near-black ink** (`#0B0B0B`, `#111`) standing in for black across the page | Template chrome; reads “AI default dark” independent of subject | Token ink / true black, or brand-specified near-black with a written reason |


| 39 | **Faint background grid** — dotted / line / blueprint / graph-paper texture behind the hero or page (`bg-[url(/grid.svg)]`, `white/5` grid) | Technical costume with no identity job; purple-gradient companion | Brand-meaningful texture or clean space; grid only when DESIGN.md names it |
| 40 | **"Trusted by" logo strip** — grayscale / low-opacity logo row or auto-scrolling marquee under the hero (often with no real customers) | Trust costume; faded logos read as decoration, not evidence | Real logos with permission at readable opacity, or one named proof point, or omit |
| 41 | **AI-generated people as real** — photoreal generated faces/hands as customers, team, or testimonials (waxy skin, melted hands, dead eyes, garbled jewelry) | Fabricated humans; disclosure and trust failure | Real photography; never present a generated person as a real customer/teammate |
| 42 | **Lucide / Heroicons monoline icon-card grid** — identical 1.5px outline glyphs in rounded tinted squares as the whole feature vocabulary | Starter icon monoculture (Inter's cousin for icons) | One deliberate set with weight/treatment; icons that identify a specific thing; or none — do not crown a replacement library |

## Motion

| # | Tell | Why | Fix |
|---|------|-----|-----|
| 43 | **Bounce / elastic easing** as default | Toy motion on serious UI | Standard ease; spring only if brand asks |
| 44 | **Infinite pulse / float loops** without user trigger | Perpetual noise | One authored moment; stop; honor `prefers-reduced-motion` |
| 45 | **Fade-up on every section + hover lift on every card** (`hover:scale-105` / `-translate-y` + shadow) | Scattered motion, no focal point | Choreograph one entrance or none; hover only on genuinely clickable surfaces |

## Positive defaults (short)

- Palette, type, radius, spacing from DESIGN.md or existing tokens
- Color, photography, illustration, and motion are good when they come from DESIGN.md — this skill removes defaults, not delight
- Hierarchy via size, weight, and space before decoration
- Layout follows content shape
- Full states: hover, focus-visible, disabled, loading, empty, error
- Companion brands: point at project DESIGN.md or [getdesign.md](https://getdesign.md) collections — do not fork brand packs into this skill
