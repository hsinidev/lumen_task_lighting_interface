---
name: Lumen-Task
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
  on-surface-variant: '#c6c6cc'
  inverse-surface: '#d4e4fa'
  inverse-on-surface: '#233143'
  outline: '#909096'
  outline-variant: '#46464c'
  surface-tint: '#c3c6d6'
  primary: '#c3c6d6'
  on-primary: '#2c303c'
  primary-container: '#0d111c'
  on-primary-container: '#797c8b'
  inverse-primary: '#5a5e6b'
  secondary: '#ffd393'
  on-secondary: '#432c00'
  secondary-container: '#fdaf00'
  on-secondary-container: '#694600'
  tertiary: '#c1c6da'
  on-tertiary: '#2b3040'
  tertiary-container: '#0c111f'
  on-tertiary-container: '#787c8f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dfe2f2'
  primary-fixed-dim: '#c3c6d6'
  on-primary-fixed: '#171b27'
  on-primary-fixed-variant: '#434653'
  secondary-fixed: '#ffddaf'
  secondary-fixed-dim: '#ffba43'
  on-secondary-fixed: '#281800'
  on-secondary-fixed-variant: '#614000'
  tertiary-fixed: '#dee2f7'
  tertiary-fixed-dim: '#c1c6da'
  on-tertiary-fixed: '#161b2a'
  on-tertiary-fixed-variant: '#414657'
  background: '#051424'
  on-background: '#d4e4fa'
  surface-variant: '#273647'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  body-base:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  data-label:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
  data-value:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1'
    letterSpacing: '0'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  container-margin: 20px
  gutter: 12px
---

## Brand & Style
The brand personality of this design system is rooted in optical precision and professional-grade utility. It is designed for creators, cinematographers, and architects who view light as a technical instrument rather than just a utility. The UI should evoke the feeling of a high-end physical lighting console—cool to the touch, responsive, and incredibly accurate.

The aesthetic utilizes a **Technical Glassmorphism** style. It combines deep, immersive surfaces with razor-sharp "light-leak" borders and subtle glow effects that simulate the behavior of light hitting a lens. The interface prioritizes clarity and functional density, ensuring that complex lighting setups feel manageable through a sophisticated, dark-mode-first environment.

## Colors
This design system operates on a primary palette of **Deep Indigo** and **Crisp White**, punctuated by a functional **Amber Glow**. 

- **Primary Background:** A deep, desaturated indigo (#0D111C) provides a high-contrast canvas that minimizes eye strain in dark studio environments.
- **Primary Text & Icons:** Pure white (#FFFFFF) is used for maximum legibility, with secondary information rendered in a muted slate (#94A3B8).
- **Interaction Accent:** Amber (#FFB000) is used exclusively for active states, warnings, and light-intensity indicators. It should feel like a warm filament glowing against the cool background.
- **Glass Surfaces:** Translucent layers use the Surface Glass variable with a background blur of 12px to 20px to create depth without clutter.

## Typography
Typography in this design system emphasizes technical accuracy. **Geist** is used for all primary UI elements and headings due to its clean, geometric precision. For technical data—such as Kelvin temperatures, lumen counts, and percentages—**JetBrains Mono** is employed to provide a "read-out" aesthetic that feels machine-generated and accurate.

Letter spacing is tightened for large displays to maintain a premium feel, while data labels are set in uppercase monospaced type with increased tracking to ensure they are glanceable in low-light conditions.

## Layout & Spacing
The layout follows a strict **8pt grid system** adapted for mobile density. As a professional tool, the design system allows for a higher information density than typical consumer apps, but maintains "safe zones" for thumb-driven interaction.

Components are organized within a contextual layout that uses 20px side margins. Gauges and control sliders should span the full width of the container-margin to provide maximum travel for precise adjustments. Vertical rhythm is maintained through consistent 16px and 24px gaps between functional blocks.

## Elevation & Depth
Depth is conveyed through **Optical Layering** rather than traditional drop shadows. Surfaces are stacked using varying levels of transparency and background blurs.

1.  **Base Layer:** Solid Deep Indigo.
2.  **Surface Layer:** Semi-transparent Indigo with a 1px "Inner Stroke" (White at 10% opacity) on the top and left edges to simulate light hitting a bezel.
3.  **Active Elevation:** Elements that are "turned on" or active do not rise physically; instead, they emit an **Amber Glow**. This is achieved using a subtle outer shadow with a large blur radius (20px+) and low opacity, paired with an amber hairline border.
4.  **Overlays:** High-blur glassmorphism is used for modals and dropdowns to keep the user grounded in the studio environment.

## Shapes
The shape language is "Soft-Technical." Elements use a **4px base corner radius** (Soft) for primary buttons and containers. This creates a profile that is precise and architectural, avoiding the playfulness of hyper-rounded corners.

- **Primary Containers:** 4px (rounded-sm).
- **Secondary Cards/Modals:** 8px (rounded-lg).
- **Control Sliders:** Pill-shaped ends are only used for the "thumb" of a slider to indicate "touchability," while the track remains rectangular with slight rounding.

## Components
- **Buttons:** Primary buttons are dark with a 1px Amber border. Upon interaction, the border glows. Text is always uppercase JetBrains Mono for a technical feel.
- **Control Sliders:** The "Lumen Slider" features a gradient track from Deep Indigo to Amber. The thumb is a crisp white circle that glows when held.
- **Status Chips:** Small, rectangular tags with a monospaced font. They use a subtle "Pulse" glow effect when a light is currently "Live."
- **Optical Cards:** These host individual light controls. They feature a 0.5px border and a very subtle vertical gradient (lighter at the top) to simulate a glass panel.
- **Input Fields:** Minimalist lines rather than boxes. When focused, the line transitions from Slate to Amber with a small glow emanating from the cursor point.
- **Toggle Switches:** Designed to look like physical toggle switches found on studio gear—stark white on a deep indigo track, using amber to denote the 'on' state.
- **Gauges:** Circular or linear read-outs for battery and temperature, utilizing hairline strokes and monospaced percentage indicators.