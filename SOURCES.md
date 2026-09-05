# Approved UI sources (universe)

Agents may pull from these stores. Prefer **official docs / CLI / registry** over hallucinated APIs. Tag keys match [STACK-FILTERS.md](./STACK-FILTERS.md).

## Primary registries (start here)

| ID | Name | URL | Tags | Notes |
|----|------|-----|------|-------|
| `shadcn` | shadcn/ui | https://ui.shadcn.com | `react` `next` `vite` `tailwind` `registry` | Default for React/Next/Vite+Tailwind. `npx shadcn@latest add` |
| `21st` | 21st.dev | https://21st.dev | `react` `next` `vite` `tailwind` `gallery` `blocks` | Large community gallery; many shadcn-compatible |
| `radix` | Radix Primitives | https://www.radix-ui.com | `react` `headless` `a11y` | Headless; style yourself or via shadcn |
| `base-ui` | Base UI | https://base-ui.com | `react` `headless` | MUI’s unstyled lineage; modern alternative |

## CSS-first / vanilla-friendly

| ID | Name | URL | Tags | Notes |
|----|------|-----|------|-------|
| `shoelace` | Shoelace / Web Awesome | https://shoelace.style · https://webawesome.com | `vanilla` `webcomponents` `html` | Best drop-in for vanilla HTML/JS |
| `daisy` | DaisyUI | https://daisyui.com | `vanilla` `tailwind` `css` `react` `vue` | Class-based; easy to skim for patterns |
| `flowbite` | Flowbite | https://flowbite.com | `vanilla` `tailwind` `html` `react` | HTML snippets; good port source |
| `open-props` | Open Props | https://open-props.style | `vanilla` `tokens` `css` | Tokens without a full component kit |
| `bootstrap` | Bootstrap | https://getbootstrap.com | `vanilla` `css` `html` | Ubiquitous; prefer for legacy only |

## Full React / Vue kits (use when brief wants a system)

| ID | Name | URL | Tags | Notes |
|----|------|-----|------|-------|
| `mui` | MUI Material | https://mui.com | `react` `system` | Heavy; only if repo already on MUI |
| `chakra` | Chakra UI | https://chakra-ui.com | `react` `system` | |
| `mantine` | Mantine | https://mantine.dev | `react` `system` | Strong forms/hooks |
| `antd` | Ant Design | https://ant.design | `react` `enterprise` | Dense admin |
| `ark` | Ark UI | https://ark-ui.com | `react` `vue` `solid` `headless` | Multi-framework headless |
| `nuxt-ui` | Nuxt UI | https://ui.nuxt.com | `vue` `nuxt` | Default for Vue/Nuxt |
| `primevue` | PrimeVue | https://primevue.org | `vue` | |

## Mobile / rugged

| ID | Name | URL | Tags | Notes |
|----|------|-----|------|-------|
| `ionic` | Ionic | https://ionicframework.com | `mobile` `react` `vue` `angular` `pwa` | Handheld / glove UIs |
| `framework7` | Framework7 | https://framework7.io | `mobile` `vanilla` `react` `vue` | iOS/Android look; vanilla OK |
| `onsen` | Onsen UI | https://onsen.io | `mobile` `hybrid` | |

## Marketing / motion (tagged `marketing` — not floor/industrial default)

| ID | Name | URL | Tags | Notes |
|----|------|-----|------|-------|
| `magicui` | Magic UI | https://magicui.design | `react` `marketing` `motion` | |
| `aceternity` | Aceternity UI | https://ui.aceternity.com | `react` `marketing` `motion` | |
| `origin` | Origin UI | https://originui.com | `react` `tailwind` `blocks` | Cleaner admin/marketing blocks |
| `cult` | Cult UI | https://www.cult-ui.com | `react` `marketing` | |

## Data / charts

| ID | Name | URL | Tags | Notes |
|----|------|-----|------|-------|
| `tremor` | Tremor | https://www.tremor.so | `react` `charts` `dashboard` | |
| `recharts` | Recharts | https://recharts.org | `react` `charts` | |
| `tanstack-table` | TanStack Table | https://tanstack.com/table | `react` `vue` `solid` `table` `headless` | |
| `ag-grid` | AG Grid | https://www.ag-grid.com | `react` `table` `enterprise` | Heavy; justify before adding |

## Icons

| ID | Name | URL | Tags |
|----|------|-----|------|
| `lucide` | Lucide | https://lucide.dev | `icons` `react` `vanilla` |
| `phosphor` | Phosphor | https://phosphoricons.com | `icons` |
| `heroicons` | Heroicons | https://heroicons.com | `icons` `tailwind` |
| `radix-icons` | Radix Icons | https://www.radix-ui.com/icons | `icons` |

## Design / variant tools (not component stores)

| ID | Name | URL | Role |
|----|------|-----|------|
| `superdesign` | Superdesign | Cursor plugin + https://superdesign.dev | **After** catalog pick: generate/compare variants of the chosen direction |
| `ui-ux-pro-max` | UI/UX Pro Max skill | `~/.claude/skills/ui-ux-pro-max` | A11y / style / palette checks — not a component registry |
| `figma` | Figma Community | https://www.figma.com/community | Visual refs; still port via stack filter |

## How to search (agent tips)

1. **shadcn:** docs search or `npx shadcn@latest add <name> --dry-run` / registry browse.
2. **21st.dev:** search by component name (Button, Sheet, Sidebar); prefer entries with clear React+Tailwind source.
3. **Shoelace:** component docs include HTML examples — copy for vanilla.
4. **Ionic:** look under “Button”, “Action Sheet”, “Modal” for touch sizes.
5. Never invent a fake `import` path — verify against the source URL or Context7 docs.
