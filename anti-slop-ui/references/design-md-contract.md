# DESIGN.md contract

This skill is a filter. Beauty comes from project direction — usually a `DESIGN.md` (or equivalent tokens / brand guidelines).

## Minimum DESIGN.md should name

| Token | Purpose |
|-------|---------|
| **Brand / product one-liner** | Who it is for; what must never look generic |
| **Color** | 4–6 named hex (bg, surface, text, muted, accent, status) |
| **Type** | Family(+ies) and roles (display, body, mono) — with license/source |
| **Radius + spacing** | Small scale (e.g. 4/8/12/16…); which controls get which radius |
| **Elevation** | When shadow/border is allowed |
| **Motion** | Static / hover-only / one entrance — and reduced-motion policy |
| **Do / don't** | Brand-specific overrides (e.g. "we *are* purple") |

Optional: density, photography style, icon set, dark/light rules.

## Sourcing it from references

When the owner has taste but no file:

1. Collect 3–5 screenshots of sites they like. Describe what each does well (layout, type, color, spacing). Edit nothing yet.
2. Let the owner pick the parts they want. Wait for the answer.
3. Write DESIGN.md with real values (sizes, weights, hex, spacing, radius). Mark anything read off a screenshot as an estimate. One screen at most.
4. Wire it in: import or reference it from `AGENTS.md` / `CLAUDE.md` ("Read DESIGN.md before any UI work") so every session loads it. If you use Google's DESIGN.md format, check it with `npx @google/design.md lint DESIGN.md`.

Borrow the references' decisions, not their brand. No clones.

## When DESIGN.md is missing

1. **Edit / Detect** — work from existing CSS variables, Tailwind theme, or shipped brand. Cite what you found.
2. **Draft** — label output **draft-without-direction**. Propose a short token stub (table above), do not invent a full marketing identity.
3. Do **not** fill the void with purple gradients or cream–terracotta. Sterile + honest > fake brand.
4. Point maintainers at their own brand or collections like [getdesign.md](https://getdesign.md) — do not vendor hundred of brand files into this skill.

## Sterile default vs slop

Sterile is an interim safety state only when direction is missing, not the target aesthetic. The target is directed tokens that look good.

| Interim sterile (only when direction is missing) | Slop (cut) |
|-----------------------------------------------|------------|
| Flat neutrals, clear type, real hierarchy, no decoration | Gradient orbs, Inter-everywhere, glass soup, fake metrics |
| “Needs DESIGN.md” labelled | Looks finished but mean or fake |

Raising liveliness **with** DESIGN.md is correct. Raising liveliness **without** direction is how purple/cream kits appear. Do not ship wireframe gray as “done”; add direction and make the result look good.
