---
name: Anti-slop UI
description: >-
  Use this when designing or reviewing UI (landings, product chrome, redesigns)
  so it does not look like generic AI. Edit/Detect/Draft modes cut purple gradients,
  Inter monoculture, glass soup, and other tells while respecting brand/DESIGN.md.
---

# Anti-slop UI

Filter for interfaces that look like the training-set mean. Cut convergent AI defaults. Keep brand, DESIGN.md, and content hierarchy. Skill id: `anti-slop-ui`.

Sibling of prose `anti-slop` (repo root). Landing/marketing *copy* that reads as AI (em dashes, puffery, fake proof) → that prose skill; this skill owns visual/UI tells. Load `references/` only when needed. Load a `recipes/` file when the surface matches.

Not a theme engine. Not a palette catalog. Your DESIGN.md (or existing tokens) stays the source of beauty.

## Modes

| Mode | When | Do |
|------|------|----|
| **Edit** (default) | Restyle existing UI | Surgical change. Preserve brand, routes, real content. Minimum diff that removes tells. Short **What changed**. |
| **Detect** | Audit / "is this AI UI?" | Name pattern, cite file/selector/region, short fix. Label evidence: **Source** (markup/CSS), **Render** (needs preview), **Judgment** (product fit). No rewrite unless asked. No fake scores. |
| **Draft** | Greenfield UI | Apply bans while building. Demand DESIGN.md or label **draft-without-direction**. |
| **Publish** (optional) | Pre-ship gate | Run `references/ui-checklist.md` pass/fail. One checklist only. |

Always-on only for design-dedicated agents. Coding agents: on-demand for UI tasks.

## Non-negotiables

1. **Purpose-gate color** — Purple/indigo/cyan–pink gradients, mesh/orb blobs are banned as unearned defaults. OK when brand or DESIGN.md specifies them.
2. **No font monoculture** — Ban unearned Inter / Roboto / Open Sans / Space Grotesk / Geist / Instrument Serif / unstated system-sans as identity defaults. Use DESIGN.md or project fonts. Do not crown a replacement default.
3. **Layout follows content** — No forced hero → 3 features → FAQ → purple CTA. No three identical icon+title+blurb cards unless the content is truly equal.
4. **Material dose** — Glass, glow, soft multi-shadow are accents (≤1–2 surfaces), not page-wide soup.
5. **Decoration earns meaning** — Side-tab stripes, eyebrows/kickers, 01/02/03 theater, emoji/sparkle icons, "AI Powered" capsules: keep only when semantic; otherwise cut.
6. **Evidence-bound chrome** — No fake metrics, Jane Doe feeds, div-built fake product screens. Real data, labelled placeholders, or honest empty states.
7. **Cream kit *and* acid-dark kit are tells** — Unearned cream + serif + terracotta, or near-black + acid-green/vermilion, rank with purple SaaS. Brand override only.
8. **Motion restraint** — One authored moment beats bounce/elastic/infinite pulse. Honor `prefers-reduced-motion`.
9. **Concentric radii** — Parent and padded child do not share the same radius. Spacing scale is deliberate.
10. **Full interaction states** — Hover, focus, disabled, loading, empty, error. Real SVG icons or none.

## Edit triage

1. Read the screen and any DESIGN.md / tokens. Note brand constraints.
2. Collect tell candidates (see `references/ui-tells.md`). Do not edit yet.
3. For each: slop or brand? False positive that flattens identity > surviving tell. When unsure, leave it (`references/ui-false-positives.md`).
4. Surgical CSS/markup only. Routes, real copy, and data untouched unless asked.
5. Self-check `references/ui-checklist.md`. Output + **What changed** (pattern category per change).

## Draft notes

- Marketing landing → `recipes/marketing-landing.md`
- App shell / dashboard / settings → `recipes/product-chrome.md`
- Restyle in place → `recipes/redesign.md`
- No DESIGN.md → label draft-without-direction; propose a short token stub via `references/design-md-contract.md`, do not invent a full brand.

## Style decisions

| Topic | Decision |
|-------|----------|
| Purple / brand accent | Ban as default; allow when DESIGN.md/brand names it |
| Inter / Geist / Space Grotesk / Instrument Serif | Ban unearned default; project fonts win; no new monoculture |
| Cream + terracotta | Treat as 2026 AI cluster tell unless brief asks for it |
| Near-black + acid-green / vermilion | Same — 2026 cluster; brand/category override only |
| Glass / glow / shadow | Dose-cap, not ban |
| Eyebrows / section numbers | Purpose-gate (sequence only), not hard ban |
| Single-word headline accent | Ban unearned italic/color-dip on one word; whole-line emphasis OK |
| UI landing copy | No em-dash theater in short UI strings; long marketing prose → sibling `anti-slop` |
| Detect output | Pattern + cite + fix; Source/Render/Judgment — no authorship accusation, no numeric "AI score" |
| Positive craft | Hierarchy via size/weight/space; one accent job; neutrals carry area |

## Reference map

- `references/ui-tells.md` — pattern cards (Tell / Why / Fix)
- `references/ui-false-positives.md` — brand purple, intentional glass/brutalist, authored variance
- `references/ui-checklist.md` — Publish / post-edit pass-fail
- `references/design-md-contract.md` — what DESIGN.md must supply; sterile-default escape
