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

## Write rules an agent can check

An agent reads every line and guesses at adjectives. "Keep spacing generous", "modern", or "clean" gives it nothing; "8px inside a group, 32px between groups" does.

- Each rule names a value, a token, or a do/don't the output can be checked against.
- Each component lists its states (hover, focus, disabled, loading), what it is not for and what to use instead (`badge`: statuses, not categories or counts), and, when it helps, one short snippet. Without them the agent invents a new pattern on every generation or picks the wrong piece.
- Say what happens when a component is missing: the agent adds it to the system (or stops and names the gap), then uses it. "Never create new elements" alone fails the first time the system lacks one, and the agent builds it inline anyway.
- Move the mechanical rules into a linter and have the agent run it after every edit (one line in `AGENTS.md`, or a post-edit hook): raw colors and arbitrary values off the token scale (`bg-pink-500`, `p-[13px]`), color or font literals outside the token block, restyling a component that owns its own spacing. Write each error so it names the allowed move ("Button owns its padding: use size sm or lg, or gap on the parent"), not only the ban. The agent reruns it until it reports zero findings; any finding left gets a written reason in the final message. Keep judgment rules (hierarchy, what the user scans first) in prose.
- Read repeated overrides as gaps in the system. When the same classes keep landing on one component (one team found `<Panel padding="none" className="px-3 py-2">` written 41 times because the padding scale had no dense step), propose the missing variant or token to the owner, then move the overrides onto it. Don't write the override a 42nd time.
- On an existing codebase, record what the linter already finds as a baseline and hold only the lines you add to zero. In the same report the first run found 1,035 problems in a codebase that already had a design system; with a baseline, overrides fell from 377 to 175 over 19 days while UI files grew from 1,328 to 1,589. A check that starts at a thousand findings gets switched off.
- Keep DESIGN.md values identical to the token file, or generate one from the other. When the two disagree the agent copies the code: in one measured build the guide said 16px card corners, the code said 24, and the agent shipped 24.

## Keep corrections

A design correction that stays in the chat is lost; the next session repeats the mistake. When the owner corrects UI, write it into DESIGN.md before the session ends.

- Count silent edits, repeated nudges ("smaller", "still too big": record where they landed), and reverts, not only explicit "no, do X".
- Write the rule at the class level (raised surfaces, dropdowns), not the one screen, with a value or token and the owner's why in their words. If they gave no reason, mark yours *inferred* and confirm it. A wrong why gets stretched to cases it doesn't fit.
- Skip one-off tweaks (this page's headline, this campaign's color).
- If an existing rule already said it, the rule failed: make it stricter (a number, a token, "never") or move it into the linter. Don't add a duplicate.
- Propose the rules and write only what the owner approves.

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
