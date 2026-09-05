# Agent workflow — global UI catalog

**Skill:** `ui-catalog` · **Rule:** `ui-catalog.mdc` · **Root:** `/Users/Shared/Developer/cursor/ui-catalog/`

## Mandatory order (any frontend design)

1. **Read** [INDEX.md](./INDEX.md) for the component category.
2. **Detect stack** via [STACK-FILTERS.md](./STACK-FILTERS.md) (or user-stated greenfield stack).
3. **Open** matching rows in [SOURCES.md](./SOURCES.md); optionally [favorites/](./favorites/).
4. **Shortlist 2–3** real components with URLs (no invented APIs).
5. **Recommend** one; cite source in reply / PR.
6. **Implement** via official install or documented port path.
7. **Repo brand** only if that workspace defines tokens/docs.
8. **Superdesign (optional):** only **after** step 5 — use Superdesign to branch visual variants of the **chosen** catalog direction, not to invent a new component system from scratch.
9. **ui-ux-pro-max (optional):** a11y / touch / contrast pass after implementation.

## Never

- Freehand a full button/sheet/nav system when a catalog source covers it
- Install a React kit into a vanilla repo “because it’s nicer”
- Default to purple gradients / Inter-only / glassmorphism (see [refs/anti-generic.md](./refs/anti-generic.md))
- Skip citation (“used a modern button”) without source URL/name
- Treat Superdesign or ui-ux-pro-max as a substitute for this catalog

## Porting React → vanilla

When stack is `vanilla` but the best visual is from shadcn/21st:

1. Keep semantics: `<button>`, focus ring, disabled, loading, `aria-*`
2. Recreate layout with flex/grid + CSS variables
3. Match touch targets (≥44px; ≥48–56px for rugged/glove)
4. Do not copy Tailwind-only class strings without a Tailwind build — expand to CSS
5. Note in PR: `Ported from <source> for vanilla`

## Greenfield repos

When creating a new repo:

1. Confirm stack with Owner if unset
2. Scaffold with the stack’s preferred kit (`shadcn` init for React/Next/Vite; Shoelace or Daisy for vanilla)
3. Add a one-line pointer in that repo’s `AGENTS.md` or README: “UI: follow global catalog at Shared `ui-catalog` + stack filter”
4. Do **not** copy this entire catalog into the new repo

## Superdesign integration

| Step | Superdesign? |
|------|----------------|
| Discover components | No — use this catalog |
| Compare 2–3 catalog directions visually | Yes — `--mode branch` on the chosen baseline |
| Pixel-polish spacing/type of selected draft | Yes — iterate/replace |
| Replace catalog entirely | No |

## Output template (agent reply)

```markdown
### UI catalog shortlist
| # | Component | Source | Stack fit |
|---|-----------|--------|-----------|
| 1 | … | url | … |
| 2 | … | url | … |
| 3 | … | url | … |

**Recommendation:** #N — <one sentence why>
**Next:** install/port · Superdesign variants (optional) · brand map (if repo tokens)
```
