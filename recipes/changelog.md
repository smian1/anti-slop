# Recipe: Changelogs and release notes

Readers are users scanning for what affects them, not reviewers.

## Defaults

- One line per change, stated as the user-visible effect: what they can now do, or what stopped breaking. ("Invalid `config.toml` now exits with code 2 instead of crashing.")
- Keep flags, filenames, versions, exit codes, and API names exact.
- Use the project's existing headings and format if it has them.

## Cuts that matter most here

- Launch hype: "excited to", "amazing", "elevate", "significantly enhance", "under the hood", "overall experience", "seamlessly", "powerful and flexible".
- Celebration emoji bullets (🎉 🚀 ✨).
- Implementation narration a user can't act on.

## Don't

- Claim speedups or impact without a measurement ("2x faster") → `references/evidence-bound.md`.
- Pad a one-fix release into a feature tour.
