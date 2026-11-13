# Design System Inspired by SKALA

> Auto-extracted from `https://skala.or.id/` on 2026-11-12

## 1. Visual Theme & Atmosphere

Friendly, approachable design with rounded shapes and generous whitespace.

The hero section leads with "Papua Barat Daya Luncurkan Portal Cenderawasih untuk Perkuat Perencanaan Pembangunan dan Layanan Das".

**Key Characteristics:**
- Spartan as the heading font
- Spartan as the body font for all running text
- Light/white background (#ffffff) as the primary canvas
- Primary accent `#00a9a3` used for CTAs and brand highlights
- 8 shadow level(s) detected — tinted shadows
- Rounded corners (5px+) creating a friendly, approachable feel
- Tags: light, rounded, accented, compact, sans-serif

## 2. Color Palette & Roles

### Primary
- **Primary Accent** (`#00a9a3`) · `--color-primary`: Brand color, CTA backgrounds, link text, interactive highlights.
- **Secondary Accent** (`#4169e1`) · `--color-secondary`: Secondary brand, hover states, complementary highlights.
- **Background** (`#ffffff`) · `--color-bg`: Page background, primary canvas.
- **Background Secondary** (`#ceebec`) · `--color-bg-secondary`: Cards, surfaces, alternating sections.

### Text
- **Text Primary** (`#212529`) · `--color-text`: Headings and body text.
- **Text Secondary** (`#54595f`) · `--color-text-secondary`: Muted text, captions, placeholders.

### Borders & Surfaces
- **Border** (`#020101`) · `--color-border`: Dividers, outlines, input borders.

### Full Extracted Palette

| # | Hex | CSS Variable | Role | Area | Contrast |
|---|---|---|---|---|---|
| 1 | `#ffffff` | `--palette-1` | section | large | text-dark |
| 2 | `#ceebec` | `--palette-2` | section | large | text-dark |
| 3 | `#223d60` | `--palette-3` | badge | large | text-light |
| 4 | `#020101` | `--palette-4` | block | large | text-light |
| 5 | `#20344d` | `--palette-5` | block | medium | text-light |
| 6 | `#00a9a3` | `--palette-6` | button | medium | text-light |
| 7 | `#f1f4f8` | `--palette-7` | button | small | text-dark |
| 8 | `#4169e1` | `--palette-8` | text-accent | small | text-light |
| 9 | `#54595f` | `--palette-9` | badge | small | text-light |

## 3. Typography Rules

- **Heading Font:** `Spartan`, sans-serif
- **Body Font:** `Spartan`, sans-serif

### Type Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing |
|---|---|---|---|---|---|
| H2 | Spartan | 22px | 600 | 70px | normal |
| H3 | Spartan | 20px | 800 | 28px | normal |
| H4 | Spartan | 30px | 900 | 60px | normal |
| Body | Spartan | 15px | 400 | 27px | normal |

### Type Scale

| Token | Size | Suggested Usage |
|---|---|---|
| Display | `40px` | headings |
| H1 | `30px` | headings |
| H2 | `28px` | headings |
| H3 | `25px` | headings |
| H4 | `22px` | headings |
| Body L | `21px` | body / supporting text |
| Body | `20px` | body / supporting text |
| Small | `18px` | body / supporting text |
| XS | `16px` | body / supporting text |
| Caption | `15px` | body / supporting text |

## 4. Component Stylings

### Primary Button

```css
.btn-primary {
  background: transparent;
  color: #00a9a3;
  border-radius: 0px;
  padding: 0px 15px;
  font-size: 15px;
  font-weight: 700;
  border: none;
  cursor: pointer;
}
```

### Ghost Button

```css
.btn-ghost {
  background: transparent;
  color: #000000;
  border-radius: 0px;
  padding: 0px 15px;
  font-size: 15px;
  font-weight: 700;
  border: none;
  cursor: pointer;
}
```

### Filled Button

```css
.btn-filled {
  background: #223d60;
  color: #ffffff;
  border-radius: 0px;
  padding: 0px 0px;
  font-size: 10px;
  font-weight: 400;
  border: none;
  cursor: pointer;
}
```

### Ghost Button 2

```css
.btn-ghost-2 {
  background: transparent;
  color: #212529;
  border-radius: 0px;
  padding: 0px 0px;
  font-size: 10px;
  font-weight: 400;
  border: none;
  cursor: pointer;
}
```

### Filled Button 2

```css
.btn-filled-2 {
  background: #ffffff;
  color: #4d4d4d;
  border-radius: 0px;
  padding: 15px 20px;
  font-size: 16px;
  font-weight: 400;
  border: none;
  cursor: pointer;
}
```

### Ghost Button 3

```css
.btn-ghost-3 {
  background: transparent;
  color: #4d4d4d;
  border-radius: 0px;
  padding: 0px 0px;
  font-size: 30px;
  font-weight: 600;
  border: none;
  cursor: pointer;
}
```

### Card

```css
.card {
  background: #000000;
  border-radius: 101px;
  padding: 15px;
}
```

## 5. Layout Principles

- **Base spacing unit:** `15px` — use multiples (30px, 45px, 60px, etc.)

### Spacing Scale (extracted from real elements)

| Token | Value | Role |
|---|---|---|
| spacing-1 | `15px` | element |
| spacing-2 | `10px` | element |
| spacing-3 | `20px` | element |
| spacing-4 | `5px` | element |
| spacing-5 | `12px` | element |
| spacing-6 | `2px` | element |
| spacing-7 | `1px` | element |
| spacing-8 | `4px` | element |

### Border Radius Scale

| Token | Value | Element |
|---|---|---|
| radius-subtle | `5px` | subtle |
| radius-button | `10px` | button |
| radius-card | `50px` | card |
| radius-subtle | `3px` | subtle |
| radius-button | `7px` | button |
| radius-pill | `101px` | pill |

## 6. Depth & Elevation

| Level | Shadow | Usage |
|---|---|---|
| Deep | `rgba(45, 45, 45, 0.2) 0px 10px 30px 0px` | Hero sections, deep layers |
| High | `rgba(0, 0, 0, 0.1) 9px 11px 14px 0px` | Modals, floating elements |
| Mid | `rgba(0, 0, 0, 0) 0px 0px 10px 0px` | Dropdowns, popovers |
| Mid | `rgb(153, 153, 153) 0px 0px 5px 0px` | Dropdowns, popovers |
| Deep | `rgba(0, 0, 0, 0.15) 0px 10px 25px 0px` | Hero sections, deep layers |

> **Note:** This site uses chromatic (color-tinted) shadows rather than pure black — this is a deliberate brand choice that adds warmth to elevation.

## 7. Do's and Don'ts

### Do
- Use `#ffffff` as the primary background color
- Use `Spartan` for all headings and `Spartan` for body text
- Use `#00a9a3` as the single dominant accent/CTA color
- Maintain `15px` as the base spacing unit — all gaps should be multiples
- Use rounded corners (`5px`+) consistently for all interactive elements
- Apply the shadow system for elevation — use the extracted shadow values

### Don't
- Don't use colors outside the extracted palette without justification
- Don't substitute Spartan/Spartan with generic alternatives
- Don't use irregular spacing — stick to 15px grid
- Don't use dark/black backgrounds — this is a light-themed design
- Don't use sharp corners — they feel hostile in this rounded design language
- Don't use oversized hero text — this brand uses restrained type
- Don't use pure black (#000000) for text — use `#212529` instead
- Don't add decorative elements not present in the original design — no badges, ribbons, banners, or ornaments unless the source site uses them
- Don't invent UI patterns the source site doesn't have — if the original has no NEW badge, don't add one just because a red is in the palette

## 8. Responsive Behavior

| Breakpoint | Width | Notes |
|---|---|---|
| Mobile | < 640px | Single column, stack sections, reduce font sizes ~80% |
| Tablet | 640–1024px | 2-column where appropriate, maintain spacing ratios |
| Desktop | 1024–1440px | Full layout as designed |
| Wide | > 1440px | Max-width container, center content |

- Touch targets: minimum 44×44px on mobile
- Maintain 15px base unit across breakpoints — only scale multipliers

## 9. Agent Prompt Guide

### Quick Color Reference

```
Background:  #ffffff
Text:        #212529
Accent:      #00a9a3
Secondary:   #4169e1
Border:      #020101
```

### Example Prompts

1. "Build a hero section with a `#ffffff` background, `Spartan` heading in `#212529`, and a `#00a9a3` CTA button with 0px radius."
2. "Create a pricing card using background `#ceebec`, border `#020101`, `Spartan` for text, and 45px padding."
3. "Design a navigation bar — `#ffffff` background, `#212529` links, `#00a9a3` for active state."
4. "Build a feature grid with 3 columns, 45px gap, each card using the card component style."
5. "Create a footer with `#212529` background, `#ffffff` text, and 30px padding."

### Iteration Guide

1. Start with layout structure (sections, grid, spacing)
2. Apply colors from the palette — background first, then text, then accents
3. Set typography — font families, sizes from the type scale, weights
4. Add components — buttons, cards, inputs using the specs above
5. Apply border-radius consistently across all elements
6. Add shadows for depth — use the extracted shadow values, not defaults
7. Check responsive behavior — test mobile and tablet layouts
8. Final pass — verify all colors match, spacing is consistent, fonts are correct

## 10. CSS Custom Properties

> 312 custom properties extracted from `:root` / `html` stylesheets.

### Color Variables

| Variable | Value |
|---|---|
| `--wpds-color-background-surface-neutral` | `#fcfcfc` |
| `--wpds-color-background-surface-neutral-strong` | `#fff` |
| `--wpds-color-background-surface-neutral-weak` | `#f4f4f4` |
| `--wpds-color-background-surface-brand` | `#ecf0fa` |
| `--wpds-color-background-surface-success` | `#c6f7cd` |
| `--wpds-color-background-surface-success-weak` | `#ebffed` |
| `--wpds-color-background-surface-info` | `#deebfa` |
| `--wpds-color-background-surface-info-weak` | `#f3f9ff` |
| `--wpds-color-background-surface-warning` | `#fde6be` |
| `--wpds-color-background-surface-warning-weak` | `#fff7e1` |
| `--wpds-color-background-surface-caution` | `#fee995` |
| `--wpds-color-background-surface-caution-weak` | `#fff9ca` |
| `--wpds-color-background-surface-error` | `#f6e6e3` |
| `--wpds-color-background-surface-error-weak` | `#fff6f5` |
| `--wpds-color-background-interactive-neutral-strong` | `#2d2d2d` |
| `--wpds-color-background-interactive-neutral-strong-active` | `#1e1e1e` |
| `--wpds-color-background-interactive-neutral-strong-disabled` | `#e6e6e6` |
| `--wpds-color-background-interactive-neutral-weak` | `#0000` |
| `--wpds-color-background-interactive-neutral-weak-active` | `#ededed` |
| `--wpds-color-background-interactive-neutral-weak-disabled` | `#0000` |
| `--wpds-color-background-interactive-brand-strong` | `#3858e9` |
| `--wpds-color-background-interactive-brand-strong-active` | `#2e49d9` |
| `--wpds-color-background-interactive-brand-strong-disabled` | `#e6e6e6` |
| `--wpds-color-background-interactive-brand-weak` | `#0000` |
| `--wpds-color-background-interactive-brand-weak-active` | `#e6eaf4` |
| `--wpds-color-background-interactive-brand-weak-disabled` | `#0000` |
| `--wpds-color-background-interactive-error` | `#0000` |
| `--wpds-color-background-interactive-error-active` | `#fff6f5` |
| `--wpds-color-background-interactive-error-disabled` | `#0000` |
| `--wpds-color-background-interactive-error-strong` | `#cc1818` |
| ... | *(167 more)* |

### Spacing Variables

| Variable | Value |
|---|---|
| `--wpds-border-radius-xs` | `1px` |
| `--wpds-border-radius-sm` | `2px` |
| `--wpds-border-radius-md` | `4px` |
| `--wpds-border-radius-lg` | `8px` |
| `--wpds-border-radius-xl` | `12px` |
| `--wpds-border-width-xs` | `1px` |
| `--wpds-border-width-sm` | `2px` |
| `--wpds-border-width-md` | `4px` |
| `--wpds-border-width-lg` | `8px` |
| `--wpds-border-width-focus` | `2px` |
| `--wpds-dimension-padding-xs` | `4px` |
| `--wpds-dimension-padding-sm` | `8px` |
| `--wpds-dimension-padding-md` | `12px` |
| `--wpds-dimension-padding-lg` | `16px` |
| `--wpds-dimension-padding-xl` | `20px` |
| `--wpds-dimension-padding-2xl` | `24px` |
| `--wpds-dimension-padding-3xl` | `32px` |
| `--wpds-dimension-gap-xs` | `4px` |
| `--wpds-dimension-gap-sm` | `8px` |
| `--wpds-dimension-gap-md` | `12px` |
| ... | *(34 more)* |

### Typography Variables

| Variable | Value |
|---|---|
| `--wpds-typography-font-family-heading` | `-apple-system,system-ui,"Segoe UI","Roboto","Oxygen-Sans","Ubuntu","Cantarell","Helvetica Neue",sans-serif` |
| `--wpds-typography-font-family-body` | `-apple-system,system-ui,"Segoe UI","Roboto","Oxygen-Sans","Ubuntu","Cantarell","Helvetica Neue",sans-serif` |
| `--wpds-typography-font-family-mono` | `"Menlo","Consolas",monaco,monospace` |
| `--wpds-typography-font-size-xs` | `11px` |
| `--wpds-typography-font-size-sm` | `12px` |
| `--wpds-typography-font-size-md` | `13px` |
| `--wpds-typography-font-size-lg` | `15px` |
| `--wpds-typography-font-size-xl` | `20px` |
| `--wpds-typography-font-size-2xl` | `32px` |
| `--wpds-typography-line-height-xs` | `16px` |
| `--wpds-typography-line-height-sm` | `20px` |
| `--wpds-typography-line-height-md` | `24px` |
| `--wpds-typography-line-height-lg` | `28px` |
| `--wpds-typography-line-height-xl` | `32px` |
| `--wpds-typography-line-height-2xl` | `40px` |
| `--wpds-typography-font-weight-default` | `400` |
| `--wpds-typography-font-weight-emphasis` | `600` |
| `--wp--preset--font-size--small` | `13px` |
| `--wp--preset--font-size--medium` | `20px` |
| `--wp--preset--font-size--large` | `36px` |
| ... | *(8 more)* |

### Other Variables

| Variable | Value |
|---|---|
| `--wpds-cursor-control` | `pointer` |
| `--wpds-motion-duration-xs` | `50ms` |
| `--wpds-motion-duration-sm` | `100ms` |
| `--wpds-motion-duration-md` | `200ms` |
| `--wpds-motion-duration-lg` | `300ms` |
| `--wpds-motion-duration-xl` | `400ms` |
| `--wpds-motion-easing-subtle` | `cubic-bezier(0.15,0,0.15,1)` |
| `--wpds-motion-easing-balanced` | `cubic-bezier(0.4,0,0.2,1)` |
| `--wpds-motion-easing-expressive` | `cubic-bezier(0.25,0,0,1)` |
| `--wp-admin-theme-color--rgb` | `56,88,233` |
| `--wp-admin-theme-color-darker-10--rgb` | `33.0384615385,68.7307692308,230.4615384615` |
| `--wp-admin-theme-color-darker-20--rgb` | `23.6923076923,58.1538461538,214.3076923077` |
| `--wp-block-synced-color--rgb` | `122,0,223` |
| `--wp-bound-block-color` | `var(--wp-block-synced-color)` |
| `--wp--preset--aspect-ratio--4-3` | `4/3` |
| ... | *(18 more)* |
