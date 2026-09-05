# Seat install — global UI catalog

Run once per Mac profile (`work`, `AlCheung`, `tomoe`) so agents see the catalog.

## Already on `work` (2026-09-05)

- Rule: `/Users/work/Developer/.cursor/rules/ui-catalog.mdc`
- Skill: `/Users/work/.cursor/skills/ui-catalog/SKILL.md`
- Shared SSOT: `/Users/Shared/Developer/cursor/ui-catalog/`
- Shared rule mirror: `/Users/Shared/Developer/cursor/rules/ui-catalog.mdc`
- GitHub: https://github.com/baturmont/ui-catalog

## Other profiles

```bash
# Rule (Developer workspace rules)
mkdir -p ~/Developer/.cursor/rules
cp /Users/Shared/Developer/cursor/rules/ui-catalog.mdc ~/Developer/.cursor/rules/ui-catalog.mdc

# Skill
mkdir -p ~/.cursor/skills/ui-catalog
cp /Users/Shared/Developer/cursor/ui-catalog/SKILL.md ~/.cursor/skills/ui-catalog/SKILL.md
```

Optional: clone the GitHub mirror elsewhere for editing; Shared path remains the live SSOT on these Macs.

## Superdesign

Use Superdesign **after** a catalog shortlist pick (variants of that direction). Do not skip the catalog for freehand UI.
