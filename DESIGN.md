---
name: FlowMood
colors:
  surface: '#0e150f'
  surface-dim: '#0e150f'
  surface-bright: '#333b34'
  surface-container-lowest: '#09100a'
  surface-container-low: '#161d17'
  surface-container: '#1a211b'
  surface-container-high: '#242c25'
  surface-container-highest: '#2f372f'
  on-surface: '#dce5da'
  on-surface-variant: '#bbcbbb'
  inverse-surface: '#dce5da'
  inverse-on-surface: '#2b322b'
  outline: '#869486'
  outline-variant: '#3d4a3e'
  surface-tint: '#4ae183'
  primary: '#54e98a'
  on-primary: '#003919'
  primary-container: '#2ecc71'
  on-primary-container: '#005027'
  inverse-primary: '#006d37'
  secondary: '#ffaaf6'
  on-secondary: '#5b005d'
  secondary-container: '#cd01d1'
  on-secondary-container: '#fffbff'
  tertiary: '#75dcff'
  on-tertiary: '#003543'
  tertiary-container: '#00c3ee'
  on-tertiary-container: '#004c5f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#6bfe9c'
  primary-fixed-dim: '#4ae183'
  on-primary-fixed: '#00210c'
  on-primary-fixed-variant: '#005228'
  secondary-fixed: '#ffd7f6'
  secondary-fixed-dim: '#ffaaf6'
  on-secondary-fixed: '#380039'
  on-secondary-fixed-variant: '#800083'
  tertiary-fixed: '#b7eaff'
  tertiary-fixed-dim: '#4cd6ff'
  on-tertiary-fixed: '#001f28'
  on-tertiary-fixed-variant: '#004e60'
  background: '#0e150f'
  on-background: '#dce5da'
  surface-variant: '#2f372f'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
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
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  container-padding-desktop: 40px
  container-padding-mobile: 20px
  gutter: 24px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

The design system is centered on a "Digital Zen" philosophy, blending high-tech precision with an immersive, calm atmosphere. It is designed for users seeking deep focus, meditation, or creative flow. 

The aesthetic is **Futuristic Minimalism** with a heavy emphasis on **Glassmorphism**. The interface acts as a window into a vast, dark environment where particles and light provide the only sense of depth. Interactions are meant to feel light and frictionless, utilizing soft blurs and glowing accents to guide the user's eye without breaking their concentration. The emotional response should be one of tranquility, safety, and sophisticated technological empowerment.

## Colors

The palette is anchored by a "Deep Space" background to minimize eye strain and maximize the perceived depth of the glass layers.

- **Primary (Aurora Green):** #2ECC71. Used for active flow states and positive feedback.
- **Secondary (Cyberpink):** #FF4DFF. Used for creative energy and highlights.
- **Tertiary (Deep Sea Blue):** #00D1FF. Used for deep focus and navigational cues.
- **Healing Gold:** #FFD700. Reserved for premium features, achievements, or warm lighting transitions.
- **Neutral/Surface:** The background is a strict #0D0D11. Interactive surfaces use a semi-transparent white alpha (`rgba(255, 255, 255, 0.04)`) to create the glass effect.

## Typography

This design system utilizes **Inter** for its neutral, systematic clarity, ensuring high readability against dark, translucent backgrounds. **Geist** is introduced for labels and technical data to reinforce the "developer-grade" precision of the futuristic theme.

Typography should be kept mostly white (#FFFFFF) with varying opacity levels:
- **Primary Text:** 90% opacity for high contrast.
- **Secondary Text:** 60% opacity for metadata and descriptions.
- **Disabled/Hint:** 35% opacity.

## Layout & Spacing

The layout follows a **Fluid Grid** model with generous whitespace to prevent the UI from feeling "cluttered." 

- **Desktop:** 12-column grid with 24px gutters. Elements typically float in the center of the screen within a 1200px max-width container.
- **Mobile:** 4-column grid. Controls are shifted to the bottom of the screen (the "thumb zone") to accommodate one-handed immersive use.
- **Spacing Rhythm:** Based on a 4px baseline. Most components should use 16px (stack-md) or 32px (stack-lg) margins to maintain a sense of openness.

## Elevation & Depth

Depth is not communicated through traditional shadows, but through **Backdrop Blurs** and **Rim Lighting**.

- **Level 1 (Base):** The Deep Space background.
- **Level 2 (Panels):** 20px - 40px Backdrop Blur with a 1px border of `rgba(255, 255, 255, 0.1)`. This creates the "frosted glass" look.
- **Level 3 (Active/Hover):** A subtle outer glow using the primary or secondary accent color (0px 0px 15px color at 30% opacity).
- **Z-Index Strategy:** Floating elements should appear as if they are suspended in liquid, with very soft transitions between states.

## Shapes

The design system uses a **Rounded** (Level 2) shape language. This softens the "technical" feel of the dark theme, making it feel more organic and approachable.

- **Standard Elements:** 0.5rem (8px) radius for buttons and small inputs.
- **Main Glass Containers:** 1.5rem (24px) radius to emphasize the "pod" or "capsule" feeling of the control panels.
- **Interactive Points:** Circles or highly rounded pills are preferred for toggles and sliders.

## Components

### Control Panels (Glass)
The signature component. Must use `backdrop-filter: blur(20px)` and a subtle linear gradient border (top-left to bottom-right) to simulate light catching the edge of the glass.

### Buttons
- **Primary:** Solid Aurora Green with black text for maximum contrast.
- **Ghost/Glass:** Transparent background with a 1px white border (20% opacity). On hover, the border becomes 60% opaque and the background blurs slightly.

### Inputs & Sliders
Sliders are critical for "mood" adjustments. Use a thick track with a glowing thumb indicator. Inputs should be "bottom-line only" or fully transparent glass containers to minimize visual noise.

### Chips & Tags
Small, pill-shaped elements with 10% opacity fills of the accent colors (e.g., 10% Deep Sea Blue fill with 100% Blue text).

### Immersive Particles
Though not a standard UI component, a background particle system is required. Particles should drift slowly and react to cursor proximity, using the four accent colors at low opacities.