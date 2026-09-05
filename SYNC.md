# Sync Shared ↔ GitHub

From a machine with this folder:

```bash
cd /Users/Shared/Developer/cursor/ui-catalog
git status
git add -A
git commit -m "Update UI catalog"
git push origin main
```

Fresh clone onto Shared (other machine / repair):

```bash
# backup if needed, then:
git clone https://github.com/baturmont/ui-catalog.git /tmp/ui-catalog-clone
# merge carefully into Shared path — do not wipe local-only notes without review
```

Cursor seats should keep the **user rule** `ui-catalog.mdc` and skill `~/.cursor/skills/ui-catalog/` in sync with this repo’s `SKILL.md` and `rules/ui-catalog.mdc` (mirrored under `/Users/Shared/Developer/cursor/rules/`).
