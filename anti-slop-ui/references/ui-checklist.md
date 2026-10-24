# UI checklist

Pass/fail for Publish or post-Edit self-check. One list only — no numeric AI-score.

## Color & type

- [ ] Palette from DESIGN.md / tokens / named brand — not default purple–pink, unearned solid indigo/blue-500 primary, unearned cream–terracotta/sage, unearned near-black+acid-green/vermilion, unearned dark-only zinc–violet shell, or unearned broadsheet (hairlines + zero radius + dense columns)
- [ ] Accent used at key moments only; neutrals carry area
- [ ] Category/severity/difference encoded by order, grouping, type, or greys before hue — no rainbow chips, per-feature accent carnival, or hash-to-hue tags; charts use a controlled ramp if needed
- [ ] Body text is near-black (or light-on-dark) — not gray-400/500 as primary copy
- [ ] Result still looks intentional and finished—not a grayscale wireframe or drained of all accent; beauty comes from tokens/brand, not from removing craft
- [ ] Fonts from DESIGN.md / project — not unearned Inter/Roboto/Open Sans/Space Grotesk/Geist/Instrument Serif/Plus Jakarta Sans/Manrope monoculture or an italic display serif hero (Fraunces/Playfair/Newsreader) by reflex
- [ ] Type scale has real steps (≥1.25× between roles), and no whole sentence is set at display size
- [ ] No heading wraps to one lone last word: `text-wrap: balance` on headings, `pretty` on body, hand breaks only between phrases
- [ ] No gradient-clipped headlines; no single-word italic/color-dip costume unless brand specifies

## Layout & components

- [ ] Section order follows content; no empty template sections; hero is not the stock metric template unless metrics are the product
- [ ] Hero has one dominant CTA labelled with what the click does (not "Get started" alone, not equal "Get Started" + "Learn More" twins)
- [ ] Feature treatments reflect hierarchy (not three identical icon-tile cards by default)
- [ ] No unearned bento-grid mosaic (mixed-size tiles only when size encodes real hierarchy)
- [ ] No meaningless side-tab stripes or 01/02/03 theater on non-sequences
- [ ] Radius + spacing scale (not one oversized radius on every surface); concentric radii respected; spacing tight within groups and wider between them (not one gap everywhere)
- [ ] No tinted-near-black-as-default-ink; no identical-card soft-grey shadow soup or ghost cards (hairline + wide diffuse shadow on every card); mono not used as page-wide meta costume
- [ ] No untouched shadcn/Tailwind starter theme (stock Card + slate/zinc `baseColor` + default `--primary`/`--radius` shipped as brand)
- [ ] App screens built around the user decision, not sidebar+stats+chart+table by default
- [ ] Pricing follows the real offer (not three tiers + "Most Popular" capsule by default)
- [ ] Footer built from real IA (not four equal columns + newsletter + social by reflex)
- [ ] No "Scroll to explore" / bouncing chevron / mouse-wheel scroll costume

## Charts & metrics

- [ ] Every chart titles its finding, labels axes with units and window, and shows its numbers somewhere besides a hover tooltip; no 3D, glow, shadow, or gradient fill on data marks
- [ ] Every metric tile names its window and comparison; small-base percentages show the absolute; updating or columned numbers use tabular lining figures

## Material & motion

- [ ] Glass / glow / soft shadow within dose caps (accents, not soup); no reflexive sticky frosted starter nav
- [ ] Motion: ≤ one authored moment or purposeful feedback; no infinite pulse; `prefers-reduced-motion` honored
- [ ] No `transition-all` / `transition: all`; transitions list their properties, and a hover changes one thing
- [ ] Essential content is visible without JavaScript; nothing important starts at `opacity: 0` waiting for a scroll reveal

## Honesty & states

- [ ] No emoji/sparkle iconography or decorative "AI Powered" capsules; real SVG/set or none
- [ ] No unearned hero pill chip / eyebrow badge parked above the H1 (especially when it restates the headline); real taxonomy kicker OK without costume status-dot
- [ ] No decorative status dots (glowing/pulsing dots beside headings/labels that mark nothing live); real status only
- [ ] No always-true status badges ("Active", "Verified", "Live" that can never show another value for this viewer); every badge can flip and has a source
- [ ] No prompt leakage in copy (stack/editor names, "built with", the brief restated as a slogan) unless that is the page's real content
- [ ] No subtitle that only restates the page/panel title; keep a subtitle only when it adds a fact (count, date range, owner, status)
- [ ] Each fact is said once: no helper line under a card or field that restates its label, no status phrase beside a badge that says the same, no button that repeats the card's subject ("Reserve", not "Reserve this equipment")
- [ ] No generic Undraw/blob / Corporate Memphis illustrations standing in for product proof
- [ ] No model-drawn illustration: no SVG scene built from primitive shapes, no sketch/doodle SVG or `feTurbulence` grain, no shapes with the idea written on them; real asset, marked slot, or nothing
- [ ] No faint dotted/line/blueprint background grid as unearned texture
- [ ] No "Trusted by" grayscale logo strip or logo marquee without real, permitted logos
- [ ] No AI-generated people presented as real customers, teammates, or testimonials
- [ ] No unearned Lucide/Heroicons monoline icon-card grid as the whole feature vocabulary
- [ ] Metrics, names, logos, feeds are real or clearly labelled placeholders
- [ ] No scaffold leftovers: no letter-on-gradient avatars, placeholder images or grey logo boxes, `href="#"`, default `<title>` / favicon / missing share image, or "Lorem ipsum", "Your Company", template name, or example.com in copy
- [ ] No div fake product chrome or tilted fake-browser mockups standing in for screenshots
- [ ] Short UI strings free of em-dash / middle-dot theater; long landing prose checked with sibling `anti-slop` if needed
- [ ] Hover, focus-visible, disabled, loading, empty, error exist where interaction exists
- [ ] Empty/error copy names cause + next action

## Distinctness

- [ ] Plan was checked against what a similar brief would get by default, and matching parts were revised (noted in What changed)
- [ ] With a sibling product's name and logo swapped in, the page no longer fits unchanged

## Render pass

- [ ] Page rendered and screenshotted at desktop and mobile widths, then reviewed from the screenshots (not only from source)
- [ ] Core flows clicked through end to end; no dead buttons, broken links, or success message without a real request behind it (watch the network tab when you submit)
- [ ] Link pasted into a chat app shows a real title and share image
- [ ] Before/after screenshots attached to What changed for Edit and Redesign

## Override log

If any item fails but brand/DESIGN.md overrides, note the source here (or in What changed). Failure without override → fix before Publish.
