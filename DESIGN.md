---
name: Obsidian Telemetry
colors:
  surface: '#051424'
  surface-dim: '#051424'
  surface-bright: '#2c3a4c'
  surface-container-lowest: '#010f1f'
  surface-container-low: '#0d1c2d'
  surface-container: '#122131'
  surface-container-high: '#1c2b3c'
  surface-container-highest: '#273647'
  on-surface: '#d4e4fa'
  on-surface-variant: '#c2c6d6'
  inverse-surface: '#d4e4fa'
  inverse-on-surface: '#233143'
  outline: '#8c909f'
  outline-variant: '#424754'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e6a'
  primary-container: '#4d8eff'
  on-primary-container: '#00285d'
  inverse-primary: '#005ac2'
  secondary: '#4edea3'
  on-secondary: '#003824'
  secondary-container: '#00a572'
  on-secondary-container: '#00311f'
  tertiary: '#4cd7f6'
  on-tertiary: '#003640'
  tertiary-container: '#009eb9'
  on-tertiary-container: '#002f38'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#acedff'
  tertiary-fixed-dim: '#4cd7f6'
  on-tertiary-fixed: '#001f26'
  on-tertiary-fixed-variant: '#004e5c'
  background: '#051424'
  on-background: '#d4e4fa'
  surface-variant: '#273647'
typography:
  headline-xl:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 56px
    letterSpacing: -0.03em
  headline-xl-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.015em
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 26px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 26px
    letterSpacing: -0.005em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 22px
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
    letterSpacing: 0em
  label-lg:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: -0.01em
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '400'
    lineHeight: 14px
    letterSpacing: 0.02em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1.5rem
  gutter-sm: 1rem
  gutter-lg: 2rem
  margin: 1.5rem
  margin-sm: 1rem
  margin-lg: 3rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

## Brand & Style

This design system establishes a high-precision, technical aesthetic tailored for systems engineering, network topology, and cloud infrastructure portfolios. Rooted in structural minimalism and utilitarian discipline, the aesthetic conveys architectural mastery, reliability, and engineering rigor without decorative clutter.

Visual direction centers on:
- **Engineered Restraint:** Elimination of arbitrary visual noise, neon flourishes, or skeuomorphic embellishments. Visual impact is derived through structural hierarchy, hairline borders, and balanced layout.
- **Architectural Density:** Interfaces evoke telemetry dashboards, terminal consoles, and modern enterprise hypervisors—organized, information-dense where required, yet framed with generous whitespace.
- **Precision Micro-Details:** Sharp 1px structural framing, functional monospaced metadata, and live status pulses communicate real-time systems operability.

## Colors

The palette models low-light NOC (Network Operations Center) displays, optimizing legibility, contrast, and cognitive focus:

- **Canvas & Surface Layers:**
  - Base Ground: `#0B0F17` (Canvas background, subterranean depth)
  - Surface Tier 1: `#111827` (Card panels, sidebar, navigation bars)
  - Surface Tier 2: `#1E293B` (Nested containers, code blocks, active hover states)
  - Surface Highlight: `rgba(255, 255, 255, 0.03)` (Subtle surface reflections)

- **Structural Outlines & Rules:**
  - Hairline Primary: `#1E293B` (Subtle boundary dividers)
  - Hairline Interactive: `#334155` (Card borders, table row dividers, inputs)
  - Hairline Focus/Active: `#3B82F6` (Focused controls, active route states)

- **Typography & Content:**
  - Primary Text: `#F8FAFC` (Titles, headers, key metric readouts)
  - Secondary Text: `#94A3B8` (Descriptions, parameter explanations, system notes)
  - Tertiary/Muted: `#64748B` (Metadata keys, timestamps, placeholder text)

- **System Accents & Status Indicators:**
  - Primary Interactive: `#3B82F6` (Electric cobalt for focus targets, primary CTA, active filters)
  - Interactive Hover: `#60A5FA`
  - Interactive Pressed: `#2563EB`
  - Telemetry Normal / Operational: `#10B981` (Emerald green for 200 OK, healthy nodes, uptime)
  - Telemetry Telemetry / Routing: `#06B6D4` (Cyan for ingress/egress, edge traffic, protocol tags)
  - Telemetry Warning / Latency: `#F59E0B` (Amber for degraded links)
  - Telemetry Fault: `#EF4444` (Crimson for outages or drop rates)

## Typography

Typography pairs geometric clarity with monospaced precision:

- **Geist (Display & Headings):** Clean horizontal strokes, tight apexes, and deliberate negative space provide a crisp, modern developer aesthetic. Always apply tight tracking (`-0.01em` to `-0.03em`) on large scales.
- **Inter (Prose & General Interface):** Selected for high legibility at micro-scales, balanced x-height, and neutral editorial tone. Used across all primary descriptions, project case studies, and form elements.
- **JetBrains Mono (Technical Metadata & Telemetry):** Used for code syntax, architectural specs, CLI commands, IP ranges, protocol labels (e.g., `BGP`, `eBPF`, `K8s`), packet latency, and uptime timestamps.

## Layout & Spacing

The structural layout utilizes a strict 12-column responsive grid underpinned by an 8px base rhythm (with 4px sub-grid micro steps).

- **Grid Architecture:**
  - Desktop (≥1200px): Max-width canvas of 1280px, 12 columns, `gutter-lg` (2rem), `margin-lg` (3rem).
  - Tablet (768px – 1199px): 8 columns, `gutter` (1.5rem), `margin` (1.5rem). Side rails collapse to an off-canvas drawer or horizontal stack.
  - Mobile (<768px): 4 columns, `gutter-sm` (1rem), `margin-sm` (1rem). Dense technical cards stack vertically.

- **Content Reflow Rules:**
  - Architecture diagrams and topology maps scale horizontally with constrained aspect ratios and pan-enabled viewports on smaller screens.
  - Multi-column telemetry statistics collapse from a 4-column inline metric strip into a 2x2 grid on tablet and a single vertical stack on mobile.

## Elevation & Depth

Visual depth avoids heavy, fuzzy shadows in favor of low-contrast hairline outlines and dark tonal layering:

- **Tier 0 (Base Canvas):** `#0B0F17` — Infinite background plane.
- **Tier 1 (Surface Cards & Structural Sections):** `#111827` enclosed by a 1px solid border of `#1E293B`.
- **Tier 2 (Floating Popovers, Flyouts, Menus):** `#1E293B` framed by a 1px border of `#334155`. Accompanied by a tightly controlled ambient occlusion shadow: `0 8px 24px -4px rgba(0, 0, 0, 0.6)`.
- **Active State Glow:** When focus or selection occurs, cards transition their border from `#1E293B` to `#3B82F6` with a micro-inset outline (`box-shadow: 0 0 0 1px #3B82F6`), eliminating blurry outer dropshadows.
- **Backdrop Filters:** Glassmorphism is restrained to persistent top navigation bars and sticky telemetry bars: `background: rgba(11, 15, 23, 0.8)` with `backdrop-filter: blur(12px)`.

## Shapes

The interface embraces a compact, semi-sharp corner language (`roundedness: 1`):
- Base containers, data cards, modals, and input fields use `0.25rem` (4px) corner radii.
- Medium elements (code snippet containers, preview frames) use `0.5rem` (8px).
- Status indicators, protocol badges, and interactive chip pills override this baseline to use full pill caps (`9999px` / `rounded-full`) to contrast against the sharp rectangular system grid.

## Components

- **Buttons:**
  - *Primary:* Solid `#3B82F6` fill, `#F8FAFC` text, `0.25rem` radius, `JetBrains Mono` 13px medium text. Hover transitions to `#2563EB`. Active scales slightly (`scale(0.99)`).
  - *Secondary / Outline:* `#111827` surface, 1px `#334155` border, `#F8FAFC` text. On hover, background shifts to `#1E293B` and border shifts to `#60A5FA`.
  - *Ghost / Code:* Transparent background, `#94A3B8` text, hover reveals `#1E293B` background.

- **Status Badges & Protocol Chips:**
  - Rendered with full pill styling (`rounded-full`), `space-xs` vertical padding, and `space-sm` horizontal padding.
  - *Operational Status:* Subtle dark emerald background (`rgba(16, 185, 129, 0.1)`), 1px border (`rgba(16, 185, 129, 0.25)`), `#10B981` text, accompanied by a 6px circular green dot with an optional CSS breathing beacon animation.
  - *Protocol Tag:* Dark slate container (`#1E293B`), 1px border (`#334155`), `#94A3B8` `JetBrains Mono` 11px uppercase text.

- **Technical Cards & Topology Nodes:**
  - Background `#111827`, 1px border `#1E293B`, `0.25rem` radius.
  - Hover triggers instantaneous border shift to `#334155` and title color transition from `#F8FAFC` to `#60A5FA`.
  - Header of cards features a split layout: title on left, telemetry/ping metric (`14ms`, `99.98%`) in `JetBrains Mono` on right.

- **Inputs & Search Terminals:**
  - Background `#0B0F17`, 1px border `#334155`, text `#F8FAFC`, placeholder `#64748B`.
  - Prefix icon or prompt glyph (`>`) rendered in `#3B82F6` `JetBrains Mono`.
  - Focus state applies a 1px border of `#3B82F6` and removes standard browser outline.

- **Code Blocks & Telemetry Feeds:**
  - Inset panel `#0B0F17`, hairline top bar containing filename and copy button, border `#1E293B`.
  - Syntax styling uses monochrome tones with `#3B82F6` for keywords, `#06B6D4` for strings, and `#64748B` for comments.

- **Lists & Data Tables:**
  - Striped rows avoided; clean separation via 1px border-b `#1E293B`.
  - Hover over row highlights with `#1E293B` background at 50% opacity.