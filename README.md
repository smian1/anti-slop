# Anti-slop

Cut convergent AI defaults — in **prose** and in **UI** — while keeping the writer's voice and the product's brand. Public MIT repo: [`smian1/anti-slop`](https://github.com/smian1/anti-slop).

Two sibling skills, one filter mindset:

| Skill | Id | What it filters |
|-------|----|-----------------|
| **Anti-slop** (repo root) | `anti-slop` | AI writing tells in digests, Slack, org copy, blurbs, social |
| **Anti-slop UI** (`anti-slop-ui/`) | `anti-slop-ui` | Generic AI interface tells on landings, product chrome, redesigns |

Thin routers + deep references + venue recipes. Not a detector-evasion kit. Not a theme engine. Your voice and your DESIGN.md stay the source of beauty.

## Install

**skills.sh / npx**

```bash
# Prose
npx skills add https://github.com/smian1/anti-slop --skill anti-slop

# UI
npx skills add https://github.com/smian1/anti-slop --skill anti-slop-ui
```

**Clone into agent skills**

```bash
git clone https://github.com/smian1/anti-slop.git

# Prose (root SKILL.md — backward compatible)
cp -R anti-slop ~/.cursor/skills/anti-slop
# or: cp -R anti-slop .agents/skills/anti-slop

# UI sibling only
cp -R anti-slop/anti-slop-ui ~/.cursor/skills/anti-slop-ui
# or: cp -R anti-slop/anti-slop-ui .agents/skills/anti-slop-ui
```

Point writing agents at the prose skill; design/UI tasks at `anti-slop-ui`. Coding agents should load on demand, not always-on (especially don't load UI tells on every TypeScript edit).

## Modes (both skills)

| Mode | Prose | UI |
|------|-------|----|
| **Edit** | Minimum phrasing change; voice keep; What changed | Surgical restyle; brand keep; What changed |
| **Detect** | Pattern / quote / fix — no rewrite | Pattern / cite / fix — no rewrite |
| **Draft** | Cuts while writing; no fabrication | Bans while building; DESIGN.md or draft-without-direction |
| **Publish** | Optional checklist | Optional UI checklist |

Details: [`SKILL.md`](SKILL.md) (prose), [`anti-slop-ui/SKILL.md`](anti-slop-ui/SKILL.md) (UI).

## Layout

```
anti-slop/
├── SKILL.md                 # prose router
├── LICENSE
├── README.md
├── references/              # prose — load on demand
├── recipes/                 # digests, slack, org-copy, …
└── anti-slop-ui/
    ├── SKILL.md             # UI router
    ├── references/          # ui-tells, false-positives, checklist, design-md-contract
    └── recipes/             # marketing-landing, product-chrome, redesign
```

## Acknowledgements

**Prose** ideas drawn from open anti-slop writing skills, including stop-slop (Hardik Pandya), no-ai-slop (Peter Yang), humanizer (Siqi Chen / @blader), unslop (Lauren Tan / cursor·pstack), slopbeth (ehmo / @synopsi), humanizer (Aboudjem / @AdamBoudj), deslop (Stephen Turner / @strnr), anti-slop (elithrar), humanize / soundshuman (aashaexo / @aashatwt), anti-ai-slop-writing (jalaalrd / @jalaal_tweets). Also Wikipedia WikiProject AI Cleanup (Signs of AI writing).

**UI** ideas informed by public design anti-slop and craft skills (filter patterns, tell catalogs, DESIGN.md practice), including work associated with miqdadbadjuber/anti-slop (antislop-ui), discountry/ritmex-skills (anti-ui-slop), Leonxlnx/taste-skill, Nutlope/hallmark, pbakaus/impeccable, anthropics/skills (frontend-design), Gesso-Build anti-slop guards, and DESIGN.md collections such as VoltAgent/awesome-design-md / getdesign.md. This repo is a thin filter sibling — not a merge of those projects.

See [`LICENSE`](LICENSE) for MIT terms and upstream attribution.

## Not in scope

- Code deslop (comments, defensive try/catch, `any` casts) — separate skill
- Theme catalogs, 192 palettes, motion encyclopedias, CLI detectors
- Detector-proofing / unicode tricks as writing tips (forensic DETECT only)
- Always-on for every coding agent
