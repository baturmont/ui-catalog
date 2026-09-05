# Stack filters — narrow the universe

Detect the repo (or greenfield choice), then **only** shortlist sources whose tags match. Do not install React kits into vanilla pages.

## Detect stack (cheap checks)

| Signal | Stack label |
|--------|-------------|
| No `package.json` / only `.html` `.css` `.js` | `vanilla` |
| `next` dependency or `next.config.*` | `next` |
| `react` + Vite (`vite.config.*`) | `vite-react` |
| `react` without Next/Vite clues | `react` |
| `vue` / `nuxt` | `vue` / `nuxt` |
| `svelte` / `@sveltejs/kit` | `svelte` |
| Ionic / Capacitor present | `mobile` (+ framework) |
| User says “new Next app” etc. | Use stated stack; skip detect |

If ambiguous and greenfield: ask once — vanilla / React+Vite / Next / Vue / mobile.

## Allow-list by stack

### `vanilla` (HTML/CSS/JS, Workers embedding HTML, static sites)

**Prefer:** `shoelace`, `daisy`, `flowbite`, `open-props`, `framework7` (vanilla mode), `lucide` (SVG/CDN)

**Port OK:** Structure + a11y from `shadcn` / `21st` / `ionic` — **re-express** as HTML + CSS; do not add React.

**Avoid installing:** MUI, Chakra, full shadcn CLI into the repo unless migrating to React.

### `vite-react` / `react`

**Prefer:** `shadcn`, `21st`, `radix`, `base-ui`, `lucide`, `tanstack-table`, `recharts` / `tremor`

**Optional:** `origin`, `magicui` / `aceternity` only if `marketing` brief

**Avoid:** Vue kits; Bootstrap unless matching existing app

### `next`

**Prefer:** same as React + Next-aware shadcn docs (App Router / RSC notes)

**Extra care:** client components for interactive Radix; don’t ship marketing motion libs to RSC by default

### `vue` / `nuxt`

**Prefer:** `nuxt-ui`, `primevue`, `ark`, `daisy`, `flowbite`

### `svelte`

**Prefer:** bits-ui / shadcn-svelte ecosystem, DaisyUI, Flowbite-Svelte — verify current docs via Context7

### `mobile` (handheld, glove, rugged)

**Prefer:** `ionic`, `framework7`, `onsen` first for CTA / sheets / lists

**Then:** port sizing lessons into web UI if the app is not Ionic

## Shortlist rule

After filter, pick **2–3** candidates max for the same need (e.g. three Button styles). Cite:

```
Source: shadcn/ui Button — https://ui.shadcn.com/docs/components/button
Alt: 21st.dev <name> — <url>
Alt: Shoelace <sl-button> — https://shoelace.style/components/button
```

Recommend one with reasons (a11y, touch size, bundle, fit to stack). Owner picks when ship gates apply; otherwise agent may proceed with the recommendation and cite it in the PR.

## Repo brand (last)

Only after shortlist:

1. If repo has design tokens / `design-system.md` / CSS variables → map colors/spacing to those.
2. If none → use catalog defaults for the chosen kit; do not invent a purple SaaS theme.
3. Product-specific kits (e.g. Tomoe Trace) live **in that repo**, not in this global catalog.
