# Anti-slop

Prose skill that cuts AI writing tells while keeping the writer's voice (`skill id: anti-slop`). Public MIT repo: [`smian1/anti-slop`](https://github.com/smian1/anti-slop).

Thin router + deep references + venue recipes. Default behavior is minimum-edit Edit/Detect (voice keep, What changed). Not a detector-evasion kit.

## Install

**Clone into agent skills**

```bash
git clone https://github.com/smian1/anti-slop.git
# Cursor / Claude-style skills dirs — pick what your agent uses:
cp -R anti-slop ~/.cursor/skills/anti-slop
# or
cp -R anti-slop .agents/skills/anti-slop
```

**skills.sh / npx (when published)**

```bash
npx skills add https://github.com/smian1/anti-slop --skill anti-slop
```

Point writing agents at this folder. Coding agents should load it on demand, not always-on.

## Modes

| Mode | Behavior |
|------|----------|
| **Edit** | Minimum phrasing change; slop-vs-voice triage; draft + What changed |
| **Detect** | Pattern / quote / fix only — no rewrite, no authorship guess |
| **Draft** | Cuts while writing; light soul; no fabrication |
| **Evidence-bound** | Vague source → gaps/questions, not invented specifics |
| **Publish** | Optional checklist before ship |
| **File** | Prose-only rewrite; preserve code/frontmatter/links |

Details and style decisions live in [`SKILL.md`](SKILL.md).

## Layout

```
anti-slop/
├── SKILL.md
├── LICENSE
├── README.md
├── references/     # load on demand
└── recipes/        # digests, slack, org-copy, agent-blurbs, social, scientific
```

## Acknowledgements

Ideas and patterns drawn from open anti-slop writing skills, including:

- stop-slop (Hardik Pandya)
- no-ai-slop (Peter Yang)
- humanizer (Siqi Chen / @blader)
- unslop (Lauren Tan / cursor·pstack)
- slopbeth (ehmo / @synopsi)
- humanizer (Aboudjem / @AdamBoudj)
- deslop (Stephen Turner / @strnr)
- anti-slop (elithrar)
- humanize / soundshuman (aashaexo / @aashatwt)
- anti-ai-slop-writing (jalaalrd / @jalaal_tweets)

Also informed by Wikipedia WikiProject AI Cleanup (Signs of AI writing).

See [`LICENSE`](LICENSE) for MIT terms and upstream attribution.

## Not in scope

- Code deslop (comments, defensive try/catch, `any` casts) — separate skill
- Detector-proofing / unicode tricks as writing tips (forensic DETECT only)
- Always-on for every coding agent
