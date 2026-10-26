---
name: Signal / Noise
version: 2.0 (redesign)
themes: [light (default), dark]
fonts: [Space Grotesk, JetBrains Mono]
---

# Signal / Noise — design system

Portfolio of **Andreas Tri Dewa Putra** (Computer Science, BINUS University — Network Technology).

Direction: a bold, monochrome, neo-brutalist layout (oversized uppercase type, thick ink
borders, hard offset shadows, alternating paper/ink sections) with a network-engineering voice:
mono "CLI" labels, a single **signal-green** accent reserved for live status and focus.

Rule of thumb: *everything is ink or paper; green means "live".*

## Colors

Tokens live as RGB triplets in CSS custom properties (`:root` = light, `.dark` = dark) and are
exposed to Tailwind as `rgb(var(--c-*) / <alpha-value>)`, so opacity modifiers (`bg-ink/80`) work.

| Token | Light | Dark | Use |
|---|---|---|---|
| `ink` | `#0A0A0A` | `#0A0A0A` | Borders, shadows, inverted sections |
| `paper` | `#FAFAF7` | `#FAFAF7` | Page ground, text on ink |
| `signal` | `#15803D` | `#22C55E` | Status dots, focus ring, active state only |
| `surface` | `#FAFAF7` | `#0A0A0A` | Page background |
| `surface-container-low` | `#F2F2EE` | `#141414` | Cards |
| `surface-container` | `#EAEAE5` | `#1C1C1C` | Chips, nested blocks |
| `surface-container-high` | `#DEDED8` | `#262626` | Hover states |
| `on-surface` | `#0A0A0A` | `#FAFAF7` | Primary text |
| `on-surface-variant` | `#404040` | `#B5B5B0` | Body / secondary text |
| `outline` | `#6B6B6B` | `#8A8A85` | Muted metadata |
| `outline-variant` | `#C8C8C2` | `#3A3A3A` | Hairlines |
| `primary` / `on-primary` | ink / paper | paper / ink | Primary buttons |
| `secondary` | = signal | = signal | Legacy alias (status text) |
| `tertiary` | `#525252` | `#A3A3A3` | Legacy alias (neutral accent) |

Light-mode signal is darkened to `#15803D` so green text keeps ≥ 4.5:1 contrast on paper.

## Typography

- **Space Grotesk** — display, headings and body.
  - Hero name: uppercase, 700, `clamp(48px, 11vw, 140px)`, tracking `-0.04em`, line-height ~0.9.
  - Section titles: uppercase, 700, `clamp(40px, 7vw, 88px)`, tracking `-0.04em`.
  - Card titles: 24–40px, 700. Body: 15–16px / 1.6.
- **JetBrains Mono** — labels, chips, metadata, section indices (`01 // SELECTED WORKS`),
  11–13px, uppercase, tracking `0.04–0.06em`.

## Shape, borders & depth

- Radius: `sm` 4px, `DEFAULT` 6px, `lg` 8px, `xl` 20px (cards), `2xl` 24px, `full` (pills).
- Borders: 2px ink on cards/buttons (1.5px on pills); hairlines use `outline-variant`.
- Shadows are hard, never blurred: `shadow-hard-sm` 3px, `shadow-hard` 6px, `shadow-hard-lg` 9px
  (ink in light mode, paper in dark mode via `--shadow-ink`).
- Hover: translate `-2px,-2px` and step the shadow up one size. Press: translate back, shadow down.

## Spacing & layout

- 8px base unit. Max content width 1280px.
- Section padding: 96–128px desktop, 64px mobile. Gutter 16px mobile / 24px tablet / 32px desktop.
- Breakpoints: mobile < 768, tablet 768–1199, desktop ≥ 1200.
- Sections alternate paper / ink backgrounds (Hero & About paper → Works ink → Journey paper → Contact ink).

## Components (planned)

- **Nav** — fixed, paper/95 + blur, 1px bottom hairline; logo, anchors, EN/ID + theme toggles, CV button; mobile menu.
- **Pill** — mono label, rounded-full, 1.5px ink border, `shadow-hard-sm`.
- **Button** — solid ink or outline; mono uppercase label; hard shadow.
- **Bento card** — 2px ink border, radius xl, `shadow-hard`; About grid: bio, photo, education (big GPA), stack, focus.
- **Status strip** — row of bordered cells: live dot + "Open to internship", BINUS · Network Technology, North Jakarta, ID, today's date.
- **Project row** — category pill, huge title, description, spec row (type · domain · repo), tech chips; terminal-style panel instead of screenshots.
- **Timeline** — center line (left line on mobile), outlined year numerals, alternating cards.

## Motion

Vanilla IntersectionObserver + CSS only: reveal-on-scroll, hero name line rise, timeline line draw,
card hover lift, live clock. Everything is disabled under `prefers-reduced-motion`.

## Accessibility

- Focus ring: 2px signal, 3px offset, on every interactive element.
- Native scrollbar is kept.
- Heading order h1 → h2 → h3; text contrast ≥ 4.5:1 in both themes.

## Language (EN / ID)

- All copy lives in the `I18N` dictionary inside `<script id="site-ui">` (`en` and `id` keys must match).
- Mark elements with `data-i18n` (text), `data-i18n-html` (allows `<br>`), `data-i18n-aria` (aria-label)
  or `data-i18n-alt` (img alt). The English text in the HTML is the fallback.
- The choice is stored in `localStorage.lang`; default is English. Title, meta description, dates
  (status strip, repo cards) and copy feedback follow the selected language.
- Proper nouns, project/course names and tool names stay in their original language.
