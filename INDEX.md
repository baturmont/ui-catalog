# Catalog INDEX — categories → sources

Use this map to pick **what kind** of UI you need, then open [SOURCES.md](./SOURCES.md) for stores tagged for that need. Always apply [STACK-FILTERS.md](./STACK-FILTERS.md) before installing.

## Primitives

| Need | Prefer sources (tags) | Favorites |
|------|----------------------|-----------|
| Button / CTA | `shadcn`, `21st`, `radix`, `daisy`, `shoelace` | [favorites/buttons.md](./favorites/buttons.md) |
| Input / Form | `shadcn`, `radix`, `react-hook-form` stacks | [favorites/forms.md](./favorites/forms.md) |
| Checkbox / Switch / Select | `radix`, `shadcn`, `shoelace` | forms |
| Dialog / Modal / Sheet / Drawer | `shadcn`, `vaul`, `ionic` (mobile) | [favorites/overlays.md](./favorites/overlays.md) |
| Tabs / Accordion | `radix`, `shadcn` | overlays |
| Tooltip / Popover / Dropdown | `radix`, `shadcn` | overlays |
| Toast / Sonner | `shadcn` (sonner), `radix` | overlays |

## Layout & chrome

| Need | Prefer sources | Favorites |
|------|----------------|-----------|
| Nav / Sidebar / Header | `shadcn`, `21st`, `origin-ui` | [favorites/chrome.md](./favorites/chrome.md) |
| Card / Panel / Section | `shadcn`, `daisy`, `flowbite` | chrome |
| Breadcrumb / Pagination | `shadcn`, `flowbite` | chrome |
| Command palette | `shadcn` (cmdk) | chrome |

## Data & dashboards

| Need | Prefer sources | Favorites |
|------|----------------|-----------|
| Table / Data grid | `shadcn` + TanStack Table, `ag-grid` (heavy) | [favorites/data.md](./favorites/data.md) |
| Charts | Recharts, Tremor, Chart.js, Apache ECharts | data |
| KPI / Stat strip | Tremor, `21st`, custom on tokens | data |
| Calendar / Date picker | `shadcn` (react-day-picker), FullCalendar | data |

## Marketing / landing

| Need | Prefer sources | Favorites |
|------|----------------|-----------|
| Hero / CTA blocks | Magic UI, Aceternity, `21st` (`marketing`) | [favorites/marketing.md](./favorites/marketing.md) |
| Pricing / Feature grid | `21st`, Origin UI | marketing |
| Motion / reveal | Magic UI, Framer Motion | marketing — **not** for industrial floor UIs |

## Mobile / rugged / handheld

| Need | Prefer sources | Favorites |
|------|----------------|-----------|
| Large touch CTAs | Ionic, Framework7, Onsen | [favorites/mobile.md](./favorites/mobile.md) |
| Bottom sheet / action sheet | Ionic, Vaul, Framework7 | mobile |
| List / Infinite scroll | Ionic, Framework7 | mobile |

## Vanilla / no-framework

| Need | Prefer sources | Favorites |
|------|----------------|-----------|
| Web Components | Shoelace / Web Awesome | [favorites/vanilla.md](./favorites/vanilla.md) |
| CSS-only kits | DaisyUI, Flowbite, Open Props | vanilla |
| Port from React kit | Copy **structure + a11y**; re-express CSS | WORKFLOW § Porting |

## Icons & tokens

| Need | Prefer sources |
|------|----------------|
| Icons | Lucide, Phosphor, Heroicons, Radix Icons |
| Design tokens / props | Open Props, Radix Colors, Tailwind theme |

## Anti-defaults (avoid unless brief asks)

See [refs/anti-generic.md](./refs/anti-generic.md) — purple-on-white SaaS, Inter-only, glassmorphism-by-default, etc.
