# Vantage — Design System Reference

This project follows the **Vantage** design system: a technical, dark-mode
design language for a consumer product. Blue / gray / black palette,
Open Sans typeface, instrument-grade precision.

The full token reference and live component examples live in
`design-system.html` in this project. **Always check that file before
building or styling a component.**

## Hard rules

- **Never invent new colors, fonts, spacing values, or radii.** Only use
  the tokens defined below (or in `design-system.html`).
- **Never swap in a different font.** Open Sans only, for both display and
  body text. JetBrains Mono only for data, timestamps, and labels — never
  for regular UI copy.
- **Every component needs its states**: default, hover, focus, disabled,
  and (where relevant) error — matching the patterns already shown in
  `design-system.html`.
- **Match the existing component patterns** (buttons, inputs, badges, cards,
  tabs, toggles) rather than designing a new visual style for the same kind
  of element.
- If a new component type is needed that isn't in `design-system.html`,
  build it **from the same tokens** and ask before introducing anything new
  visually (new color, new font weight, new shadow style, etc.).

## Color tokens

| Name | Hex | Usage |
|---|---|---|
| Ink | `#101418` | Base background |
| Surface | `#171C21` | Cards, panels |
| Surface 2 | `#1D232A` | Nested surfaces |
| Line | `#2B333B` | Borders, dividers |
| Steel | `#6E7F91` | Labels, icons |
| Fog | `#8A96A3` | Secondary text |
| Paper | `#E8ECF0` | Primary text |
| Blue | `#4C8DFF` | Primary action, focus |
| Mint | `#3ECF8E` | Success / positive |
| Amber | `#F2A33D` | Caution / monitoring |
| Error | `#F2545B` | Errors, destructive |

> **Eyebrow labels** (`.eyebrow`, e.g. "VANTAGE · DASHBOARD") use **Fog**
> (`#8A96A3`), not Steel — Steel is too low-contrast for this size/weight.
> Steel stays reserved for icons and larger structural labels
> (e.g. `.group-label`).

## Typography

- **Display / headings:** Open Sans, weight 700
- **Body:** Open Sans, weight 400–600
- **Data / labels / timestamps:** JetBrains Mono, weight 400–600
- Type scale reference: 40px (primary heading), 24px (section heading),
  16px (body), 13px (secondary/caption), 14px mono (data)

## Spacing scale

4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 px — always use this scale for padding,
margin, and gap. Never use an arbitrary pixel value outside this list.

## Radius

- Small (`6px`): buttons, inputs, tags
- Medium (`10px`): metric cards, tab containers
- Large (`16px`): panels, larger cards

## Components already defined (see `design-system.html`)

Buttons (primary / secondary / ghost / danger / disabled), Inputs
(default / focus / error), Badges (mint / blue / error), Metric card,
Tabs, Toggle switch.

## Language & direction

All UI copy is in **English**, layout is **LTR**.
