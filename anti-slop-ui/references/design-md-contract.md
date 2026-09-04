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

## When DESIGN.md is missing

1. **Edit / Detect** — work from existing CSS variables, Tailwind theme, or shipped brand. Cite what you found.
2. **Draft** — label output **draft-without-direction**. Propose a short token stub (table above), do not invent a full marketing identity.
3. Do **not** fill the void with purple gradients or cream–terracotta. Sterile + honest > fake brand.
4. Point maintainers at their own brand or collections like [getdesign.md](https://getdesign.md) — do not vendor hundred of brand files into this skill.

## Sterile default vs slop

| Sterile (acceptable interim) | Slop (cut) |
|------------------------------|------------|
| Flat neutrals, clear type, real hierarchy, no decoration | Gradient orbs, Inter-everywhere, glass soup, fake metrics |
| "Needs DESIGN.md" labelled | Looks finished but mean |

Raising liveliness without direction is how cream kits and purple SaaS appear. Demand tokens first.
