# UI false positives

Prefer leaving a tell over flattening real brand or intentional craft. Detect can still *name* the pattern; Edit should not force a rewrite when override applies.

## Directed beauty is not slop

Strong color systems, illustration, photography, bold type, and rich but authored materials are good when intentional and supported by DESIGN.md or brand direction. Keep them when they do real product or brand work. Anti-slop does not equal flat/no-color; remove defaults, not directed delight.

## Brand override

| Looks like slop | Keep when |
|-----------------|-----------|
| Purple / indigo / violet system | Stripe-class brand purple, DESIGN.md accent, or established product color |
| Gradient hero | Brand marketing system already ships that gradient (document the source) |
| Glass / blur | Product *is* glass-forward (visionOS-style, intentional frosted panels) and dose is controlled |
| Soft shadows | Elevation system from tokens; not random per-card glow |
| Rounded pills | Brand explicitly pill-shaped (consumer, playful) with a radius scale |
| Dark + neon / acid-green / vermilion accent | Brand or product category (creative tools, gaming) specifies it |
| Dark-only UI | Product is night-native (creative tools, trading, cinema) *and* neutrals are authored, not stock zinc+violet |
| Frosted sticky nav | Product is glass-forward with a controlled dose (not the starter logo/links/CTA blur bar) |
| Grey secondary labels | Truly secondary metadata (timestamps, captions), not body copy |
| Single-word italic or color in a headline | Editorial/fashion brief explicitly asks for that register |
| Background grid / blueprint | Brand or product category (CAD, engineering, map) specifies technical grid texture |
| "Trusted by" logo row | Logos are real customers with permission, full opacity, not a faded marquee costume |
| Lucide / outline icons | Product already standardized on that set *and* icons carry specific meaning (not decorative 3-up chips) |

**Rule:** If DESIGN.md, brand guidelines, or shipped production CSS already commits to the look, it is authored — not a default. Cite the source in What changed / Detect notes.

## Intentional aesthetics

| Look | Not slop when |
|------|----------------|
| Brutalist / raw | Deliberate harsh type, visible structure, no soft-card kit |
| Maximal marketing | Authored variance across sections (rhythm chosen, not pasted) |
| Editorial serif + cream | Brief or brand asks for warm print feel — not the unearned Claude-beige default |
| Broadsheet / hairline editorial | Brief or brand asks for print/newspaper/editorial register — authored, not the unearned cluster default |
| Hero led by a real primary metric | Metric is verified and *is* the product story — not filler stats |
| Monospace UI | Real data/code product where mono is the interface, not costume |
| Bento / mosaic | Content genuinely has mixed sizes to display |
| Middle plan highlighted | Real offer has a clear recommended tier *and* the badge is not the stock "Most Popular" costume |
| Two hero actions | Both actions are real and primary for the audience (rare); still prefer visual hierarchy |
| Multi-column footer | Site actually has that many top-level link groups |
| Scroll affordance | Long editorial/scrollytelling brief that *needs* an authored scroll prompt (rare) |
| AI illustration (abstract) | Openly abstract/illustrative work, not presented as a real person or customer |
| Real customer logos | Named, permitted, readable — proof, not grayscale wallpaper |

## Marketing variance

Landing pages *should* vary. Hero → features is fine when those sections earn their place with real product content. The tell is **defaulting** to the full template (including fake logos, three equal cards, purple CTA) when content does not require it.

Identical card grids are OK for truly parallel items (e.g. three equal pricing dimensions). Flag when hierarchy is flattened that should not be.

## Detect vs Edit

- **Detect:** list pattern + cite + suggested fix even for borderline cases; mark `override-likely` if brand may explain it.
- **Edit:** apply override; do not "de-purple" a brand purple product.
- **Draft:** without DESIGN.md, avoid the whole default cluster — do not replace purple SaaS with cream terracotta, acid-dark, or broadsheet kits as the new mean.
