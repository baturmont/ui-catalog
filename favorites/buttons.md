# Favorites — Buttons / CTAs

Gold starters. Always re-check live docs; versions change.

| Name | Source | Stack | Why | URL |
|------|--------|-------|-----|-----|
| Button | shadcn | react/next/vite | Variants + asChild; industry default | https://ui.shadcn.com/docs/components/button |
| Button | Shoelace `sl-button` | vanilla | Web component; CDN-friendly | https://shoelace.style/components/button |
| Button | DaisyUI | vanilla/tailwind | Class recipes easy to port | https://daisyui.com/components/button/ |
| Button | Ionic | mobile | Large touch; rugged | https://ionicframework.com/docs/api/button |
| Button | Framework7 | mobile/vanilla | iOS/MD themes | https://framework7.io/docs/button.html |
| Destructive / danger | shadcn Button `variant=destructive` | react | Clear danger semantics | https://ui.shadcn.com/docs/components/button |
| Icon button | shadcn + Lucide | react | Pair with aria-label | https://lucide.dev |
| Loading button | shadcn + disabled + spinner | react | Prevent double-submit | (compose) |
| FAB / speed dial | Ionic fab | mobile | Thumb-zone actions | https://ionicframework.com/docs/api/fab |
| Link-styled button | Radix Slot / shadcn asChild | react | Correct a11y for nav CTAs | https://www.radix-ui.com/primitives/docs/utilities/slot |

## Selection heuristics

- **Office desktop:** shadcn or 21st.dev button blocks
- **Vanilla / Worker HTML:** Shoelace or Daisy port
- **Handheld / glove:** Ionic or Framework7 sizing (≥48px height)
- **Marketing hero CTA:** Magic UI / Aceternity only if brief is marketing
