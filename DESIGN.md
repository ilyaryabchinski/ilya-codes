# Ilya Codes 8-bit design system

## 1. Atmosphere & identity

An approachable portfolio presented like a polished 8-bit game interface. The signature is a monochrome pixel frame with stepped corners, dashed construction lines, and small press feedback. The visual grammar comes from 8bitcn.com while the content and identity stay Ilya's.

## 2. Color

| Role | Token | Light | Dark | Usage |
|---|---|---|---|---|
| Canvas | `--canvas` | `#f5f5f5` | `#0a0a0a` | Page background |
| Surface | `--surface` | `#fafafa` | `#141414` | Cards and header |
| Surface muted | `--surface-muted` | `#ededed` | `#202020` | Inset areas |
| Ink | `--ink` | `#0a0a0a` | `#f5f5f5` | Primary text |
| Ink muted | `--ink-muted` | `#737373` | `#a3a3a3` | Supporting text |
| Rule | `--rule` | `#a3a3a3` | `#525252` | Pixel borders and rails |
| Primary | `--primary` | `#171717` | `#fafafa` | Buttons and strong states |
| Primary ink | `--primary-ink` | `#fafafa` | `#171717` | Text on primary |

## 3. Typography

Press Start 2P is used for display headings, navigation, labels, and controls. Geist Sans is used for paragraph copy. Hero display text scales from 1.5rem to 3rem. Retro labels range from 0.5rem to 0.75rem and use 1.6 line height. Body copy stays at 0.875rem or larger.

## 4. Spacing & layout

Spacing uses a 4px base. The page sits inside a 1240px shell with dashed vertical rails. Mobile gutters are 16px. Cards use a 4px pixel unit for stepped edges. The content grid uses one column on mobile and twelve columns above 900px.

## 5. Components

### Pixel frame
- **Structure:** semantic section or article with a square surface and stepped clip-path.
- **Variants:** standard, dark hero, compact item.
- **States:** linked frames lift at hover and translate down 4px when pressed.
- **Accessibility:** focus ring is 3px and never clipped.

### Pixel button
- **Structure:** anchor or button with text and decorative corner squares.
- **States:** default, hover inversion, active translate, focus, current page.
- **Accessibility:** decorations are CSS-only and ignored by assistive technology.

### Navigation
- **Structure:** dashed header rail, desktop links, mobile menu button and drawer.
- **States:** current page uses the primary fill.

### Full-stack loadout
- **Structure:** a labeled skill list in the hero's right-side panel.
- **Content:** front end, back end, AI systems, data, and infrastructure.
- **Accessibility:** labels remain readable in one column on mobile.

## 6. Motion & interaction

Press feedback translates controls down 4px in 100ms. Hover changes color without easing. Linked arrows may nudge by 3px with a two-step animation. Reduced motion disables all transforms and animation.

## 7. Depth & surface

Depth comes from pixel edges and hard offsets, never blur or soft shadows. Surfaces are square. Dashed rails organize the page. The identity and preview areas use CSS-built pixel art, not photographs or stock imagery.

## 8. Accessibility constraints & accepted debt

Target WCAG 2.2 AA. Body text keeps 4.5:1 contrast. All controls have visible focus, navigation works by keyboard, images have useful alternative text, and reduced motion is respected. There is no accepted design debt.
