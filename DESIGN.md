---
name: Apex Broadcast
colors:
  surface: '#101415'
  surface-dim: '#101415'
  surface-bright: '#363a3b'
  surface-container-lowest: '#0b0f10'
  surface-container-low: '#191c1e'
  surface-container: '#1d2022'
  surface-container-high: '#272a2c'
  surface-container-highest: '#323537'
  on-surface: '#e0e3e5'
  on-surface-variant: '#c6c6cd'
  inverse-surface: '#e0e3e5'
  inverse-on-surface: '#2d3133'
  outline: '#909097'
  outline-variant: '#45464d'
  surface-tint: '#bec6e0'
  primary: '#bec6e0'
  on-primary: '#283044'
  primary-container: '#0f172a'
  on-primary-container: '#798098'
  inverse-primary: '#565e74'
  secondary: '#4ae176'
  on-secondary: '#003915'
  secondary-container: '#00b954'
  on-secondary-container: '#004119'
  tertiary: '#b9c7e0'
  on-tertiary: '#233144'
  tertiary-container: '#09182a'
  on-tertiary-container: '#738298'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#6bff8f'
  secondary-fixed-dim: '#4ae176'
  on-secondary-fixed: '#002109'
  on-secondary-fixed-variant: '#005321'
  tertiary-fixed: '#d5e3fd'
  tertiary-fixed-dim: '#b9c7e0'
  on-tertiary-fixed: '#0d1c2f'
  on-tertiary-fixed-variant: '#3a485c'
  background: '#101415'
  on-background: '#e0e3e5'
  surface-variant: '#323537'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-bold:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 20px
    letterSpacing: 0.05em
  stats-number:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
---

## Brand & Style
The design system is engineered for high-stakes, real-time sports broadcasting and data visualization. It prioritizes rapid information processing, legibility under varying lighting conditions, and a premium "live" aesthetic.

The style is **Corporate Modern with High-Contrast accents**. It utilizes a dark-mode-first approach to reduce eye strain during extended viewing and to allow vibrant action colors to pop. UI elements are structured as clean, flat cards with surgical precision, ensuring the system feels authoritative and technologically advanced. For broadcast overlays, the system maintains high transparency compatibility, using solid color blocks and clear strokes to ensure visibility against motion-heavy video backgrounds.

## Colors
This design system utilizes a high-contrast dark palette optimized for digital screens and broadcast overlays.

- **Primary (#0f172a):** The "Deep Navy" foundation. Used for core backgrounds, sidebars, and heavy UI containers. It provides a stable, professional anchor.
- **Secondary (#22c55e):** The "Neon Live" green. Reserved exclusively for active states, "Live" indicators, primary action buttons, and positive momentum data (e.g., run rate increasing).
- **Tertiary (#334155):** The "Subtle Slate." Used for borders, divider lines, and secondary card backgrounds to create internal hierarchy without high visual noise.
- **Neutral (#f8fafc):** "Clean White." Used for primary body text and headlines to ensure maximum readability against dark backgrounds.

## Typography
The system relies on **Inter** for its exceptional legibility and systematic feel. In a sports context, "tabular num" (tnum) settings are mandatory for scoreboards to prevent horizontal jumping when numbers update.

- **Headlines:** Use Bold or Extra Bold weights to create a strong information hierarchy. 
- **Stats:** Use the `stats-number` role for scoreboards and data grids; it ensures vertical alignment across rows of data.
- **Labels:** Small, uppercase labels with increased letter spacing are used for metadata (e.g., "OVER", "WICKETS", "TARGET") to distinguish them from dynamic data.

## Layout & Spacing
The layout follows a **Fluid Grid** model based on a 4px baseline shift, ensuring all elements align mathematically.

- **Desktop:** 12-column grid with 24px gutters. Use wide margins (32px+) to maintain a "broadcast safe" area.
- **Mobile:** 4-column grid with 16px gutters. Elements should stretch to full width where possible to maximize the size of touch targets and data points.
- **Broadcast Overlays:** Use a "Safe Zone" padding of 48px from all edges to ensure the UI is not cut off by various screen aspect ratios or hardware scaling.

## Elevation & Depth
The system uses **Tonal Layering** supplemented by extremely subtle shadows to maintain a "flat but layered" feel.

- **Level 0 (Base):** Deep Navy (#0f172a). Used for the main background.
- **Level 1 (Card):** Slate tint (#1e293b). Used for surface containers.
- **Level 2 (Active/Hover):** Subtle Slate (#334155). Used for elevated elements.
- **Shadows:** Use a single, tight shadow for cards: `0 4px 6px -1px rgba(0, 0, 0, 0.3)`. Shadows should be neutral and dark to avoid "glow" effects unless it's a specific live indicator.
- **Overlays:** For OBS integration, use 90% opacity on card backgrounds to allow a hint of the video feed to pass through while maintaining text contrast.

## Shapes
The design system utilizes **Rounded** (8px) geometry. This radius is applied to cards, buttons, and input fields. 

- **Standard Radius:** 8px (`rounded-md`) for most UI containers.
- **Large Radius:** 16px (`rounded-xl`) for main dashboard widgets.
- **Indicator Radius:** 2px for small "live" tags or status bars to keep them looking sharp and professional.

## Components
Consistent implementation of components is critical for the "Broadcast" look:

- **Buttons:** Primary buttons use the Neon Green (#22c55e) background with dark text. Secondary buttons use an outline of Subtle Slate with white text.
- **Live Indicator:** A small Neon Green dot paired with "LIVE" in `label-bold`. This component should have a subtle pulse animation.
- **Scorecards:** Flat cards using Level 1 background. Use a vertical 4px Neon Green accent bar on the left side to indicate the currently batting team or active event.
- **Data Tables:** Use alternating row stripes (Level 0 and Level 1) instead of borders for a cleaner look. Headers must be in `label-bold`.
- **Inputs:** Dark background (#1e293b) with a 1px border of Subtle Slate. On focus, the border transitions to Neon Green.
- **Chips/Badges:** Small capsules with a 1px border. Use Neon Green for positive stats (e.g., "Free Hit") and Red for alerts (e.g., "Out").