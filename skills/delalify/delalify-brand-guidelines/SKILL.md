---
name: delalify-brand-guidelines
description: Applies Delalify's official brand colors, typography, and design tokens to any artifact that benefits from Delalify's look-and-feel. Use this skill when creating presentations, documents, charts, posters, web pages, or any visual output for Delalify. Trigger whenever the user mentions Delalify branding, Delalify colors, Delalify style, or asks for output styled "like the Delalify site," even if they don't say "brand guidelines" explicitly.
---

# Delalify Brand Identity

Delalify's visual identity is built around a bold blue primary color, gold secondary accent, and clean modern typography. The brand feels professional yet approachable, with generous whitespace and rounded corners throughout.

## Colors

### Brand Colors

| Role | Hex | RGB | Usage |
| ------ | ----- | ----- | ------- |
| Primary Blue | `#1C7EDA` | `rgb(28, 126, 218)` | Buttons, links, primary actions, brand identity |
| Primary Blue (bright) | `#2196F3` | `rgb(33, 150, 243)` | Accent foreground, chart primary, theme color |
| Secondary Gold | `#FFBB00` | `rgb(255, 187, 0)` | Secondary buttons, badges, highlights |
| Brand Active | `#1664AF` | `rgb(22, 100, 175)` | Hover/pressed states on primary elements |
| Highlight Yellow | `#FFDD33` | `rgb(255, 221, 51)` | Callouts, selected text, emphasis |
| Focus Ring | `#1DA1F2` | `rgb(29, 161, 242)` | Focus indicators, interactive outlines |

### Logo Palette

The Delalify logo is a stylized geometric "D" constructed from five colored shapes:

| Color | Hex | RGB | Logo element |
| ------- | ----- | ----- | -------------- |
| Blue | `#2196F3` | `rgb(33, 150, 243)` | Main letter body and wordmark |
| Gold | `#FDD835` | `rgb(253, 216, 53)` | Center accent strip |
| Pink | `#F50057` | `rgb(245, 0, 87)` | Lower curve accent |
| Green | `#4CAF50` | `rgb(76, 175, 80)` | Upper curve accent |
| Ice Blue | `#E3F2FD` | `rgb(227, 242, 253)` | Inner highlight |

When using accent colors in non-text shapes (charts, diagrams, decorative elements), cycle through these five logo colors to maintain brand cohesion.

### Surface Colors

**Light mode:**

| Role | Hex | RGB |
| ------ | ----- | ----- |
| Background | `#FFFFFF` | `rgb(255, 255, 255)` |
| Foreground | `#0F1419` | `rgb(15, 20, 25)` |
| Card | `#FCFCFC` | `rgb(252, 252, 252)` |
| Muted | `#F0F0F0` | `rgb(240, 240, 240)` |
| Muted Foreground | `#646E78` | `rgb(100, 110, 120)` |
| Accent | `#E3ECF6` | `rgb(227, 236, 246)` |
| Border | `#E3E9ED` | `rgb(227, 233, 237)` |
| Input | `#F7F9FA` | `rgb(247, 249, 250)` |
| Destructive | `#F4212E` | `rgb(244, 33, 46)` |

**Dark mode:**

| Role | Hex | RGB |
| ------ | ----- | ----- |
| Background | `#000000` | `rgb(0, 0, 0)` |
| Foreground | `#E7E9EA` | `rgb(231, 233, 234)` |
| Card | `#17181C` | `rgb(23, 24, 28)` |
| Muted | `#181818` | `rgb(24, 24, 24)` |
| Muted Foreground | `#727678` | `rgb(114, 118, 122)` |
| Accent | `#061622` | `rgb(6, 22, 34)` |
| Border | `#242628` | `rgb(36, 38, 40)` |
| Input | `#22303C` | `rgb(34, 48, 60)` |

Primary Blue (`#1C7EDA`), Secondary Gold (`#FFBB00`), and Destructive (`#F4212E`) stay the same across both modes.

### Chart Colors

Use these in order for data visualization:

1. `#2196F3` - Blue
2. `#4CAF50` - Green
3. `#F7B928` - Amber
4. `#17BF63` - Teal green
5. `#E91E63` - Pink

## Typography

### Font Families

| Role | Font | Fallback | CSS Variable |
| ------ | ------ | ---------- | -------------- |
| Body / UI | **Figtree** | `ui-sans-serif, sans-serif, system-ui` | `--font-figtree` |
| Headings / Branding | **EB Garamond** | `serif` (light) / `Georgia, serif` (dark) | `--font-eb-garamond` |
| Code | System mono | `monospace` (light) / `Menlo, monospace` (dark) | `--font-mono` |

### How fonts are applied

- **Figtree** is the workhorse; it handles body text, labels, navigation, and all general UI.
- **EB Garamond** is reserved for display headings, hero text, and moments where the brand wants an elegant serif voice. Use it for `h1`/`h2` headings and branded callouts.
- Headings use semi-bold to bold weight with tight letter spacing (`tracking-tight`).
- Body text uses regular weight with relaxed line height (`leading-relaxed`).

### For non-web artifacts

When creating presentations, documents, or other outputs:

- Use **Figtree** for body text. If unavailable, fall back to **Arial** or **Helvetica**.
- Use **EB Garamond** for headings. If unavailable, fall back to **Georgia**.
- For python-pptx: apply EB Garamond to titles/headings (24pt+), Figtree to body text.

## Layout and Spacing

### Border Radius

Delalify uses generous rounding. The base radius is `1rem` (16px):

| Token | Value | Typical usage |
| ------- | ------- | --------------- |
| `radius-sm` | 12px | Small chips, tags |
| `radius-md` | 14px | Buttons, inputs |
| `radius-lg` | 16px | Cards, dialogs |
| `radius-xl` | 20px | Feature cards, hero sections |
| Full round | `rounded-full` | Avatars, icon badges |
| Extra large | `rounded-3xl` (48px) | Showcase/feature cards |

### Spacing

Built on a 4px grid (`--spacing: 0.25rem`):

- Compact elements: `px-3 py-1`
- Standard buttons: `px-4 py-2`
- Card padding: `px-6 py-6`
- Section vertical rhythm: `py-16` for major sections, `py-6` to `py-12` for subsections
- Container horizontal padding: `px-4` (mobile), `px-8` to `px-16` (desktop)

### Shadows

The brand avoids heavy drop shadows in favor of subtle border-based separation.

## Callout / Status Colors

These are ready-made palettes for informational UI:

| Type | Light BG | Light Border | Light Text | Icon |
| ------ | ---------- | ------------- | ------------ | ------ |
| Note | `#EFF6FF` | `#93C5FD` | `#1E3A8A` | `#3B82F6` |
| Info | `#F0F9FF` | `#7DD3FC` | `#0C4A6E` | `#0EA5E9` |
| Tip | `#F0FDF4` | `#86EFAC` | `#14532D` | `#22C55E` |
| Warning | `#FEFCE8` | `#FDE047` | `#713F12` | `#EAB308` |
| Danger | `#FEF2F2` | `#FCA5A5` | `#7F1D1D` | `#EF4444` |
| Check | `#ECFDF5` | `#6EE7B3` | `#064E3B` | `#10B981` |

Dark mode variants shift to darker backgrounds with brighter text; the border and icon colors remain close to their light-mode counterparts for consistency.

## Applying the Brand

### Presentations (python-pptx)

Apply colors using `RGBColor`:

```python
from pptx.util import RGBColor

DELALIFY_BLUE = RGBColor(28, 126, 218)
DELALIFY_GOLD = RGBColor(255, 187, 0)
DELALIFY_PINK = RGBColor(245, 0, 87)
DELALIFY_GREEN = RGBColor(76, 175, 80)
DELALIFY_ICE = RGBColor(227, 242, 253)
DELALIFY_DARK = RGBColor(15, 20, 25)
DELALIFY_LIGHT = RGBColor(255, 255, 255)
```

Use EB Garamond for slide titles (24pt+) and Figtree for body text. Cycle through the logo palette for shape fills and chart series.

### Documents and other formats

Follow the same color and typography rules. Primary Blue for headings and links, dark foreground for body text, gold for secondary highlights. Keep the generous whitespace and rounded aesthetic wherever the format allows.
