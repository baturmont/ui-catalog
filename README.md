# Global UI catalog (agent-first)

**Purpose:** Cross-repo universe of modern UI sources. Agents consult this **before inventing UI**.

**Not** a product design system. Repo brand/tokens apply **only after** stack filter, when that repo defines them.

```
Universe (this catalog)
    → filter by repo stack (vanilla | React | Next | Vue | …)
    → shortlist 2–3 components (cite source)
    → apply repo brand/tokens if present
    → optional: Superdesign variants of the chosen direction
```

## Files

| File | Role |
|------|------|
| [INDEX.md](./INDEX.md) | Category map → where to look |
| [SOURCES.md](./SOURCES.md) | Approved live stores + tags |
| [STACK-FILTERS.md](./STACK-FILTERS.md) | How to narrow by frontend language |
| [WORKFLOW.md](./WORKFLOW.md) | Mandatory agent steps + Superdesign |
| [favorites/](./favorites/) | Gold patterns (curated starters) |
| [refs/](./refs/) | Extra notes / anti-patterns |

## Sync

- **Canonical on disk:** `/Users/Shared/Developer/cursor/ui-catalog/` (all Mac profiles)
- **GitHub mirror:** `https://github.com/baturmont/ui-catalog` (pull/push to keep Shared ↔ remote aligned)
- **Cursor rule:** `ui-catalog.mdc` (Developer + Shared rules)
- **Skill:** `~/.cursor/skills/ui-catalog/`

## License note

Catalog indexes point at third-party sites. Respect each source’s license when copying code into a repo. Prefer official install paths (`npx shadcn@latest add`, package managers) over blind paste.
