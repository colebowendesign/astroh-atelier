---
name: Astroh Cinematic Minimal
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#cdc3d0'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#968e9a'
  outline-variant: '#4a454f'
  surface-tint: '#dbb8ff'
  primary: '#ecd7ff'
  on-primary: '#3f2160'
  primary-container: '#d8b4fe'
  on-primary-container: '#604283'
  inverse-primary: '#6f5092'
  secondary: '#bdc2ff'
  on-secondary: '#131e8c'
  secondary-container: '#2f3aa3'
  on-secondary-container: '#a8afff'
  tertiary: '#cfe0fa'
  on-tertiary: '#213145'
  tertiary-container: '#b4c4de'
  on-tertiary-container: '#415167'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#efdbff'
  primary-fixed-dim: '#dbb8ff'
  on-primary-fixed: '#29074a'
  on-primary-fixed-variant: '#573878'
  secondary-fixed: '#e0e0ff'
  secondary-fixed-dim: '#bdc2ff'
  on-secondary-fixed: '#000767'
  on-secondary-fixed-variant: '#2f3aa3'
  tertiary-fixed: '#d3e4fe'
  tertiary-fixed-dim: '#b7c8e1'
  on-tertiary-fixed: '#0b1c30'
  on-tertiary-fixed-variant: '#38485d'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display:
    fontFamily: Plus Jakarta Sans
    fontSize: 64px
    fontWeight: '300'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  h1:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '400'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  h2:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.3'
    letterSpacing: 0.01em
  h3:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.02em
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0.015em
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0.015em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.08em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  container-max: 1280px
---

## Brand & Style

The brand personality is high-end, artistic, and evocative, targeting the luxury tech and creative services sector. It evokes an emotional response of "deep focus" and "quiet confidence" through a design style that blends **Minimalism** with **Glassmorphism**.

The visual direction uses cinematic interaction design—leveraging motion, transparency, and subtle glows—to create a digital environment that feels premium and immersive. The aesthetic intelligence is reflected in the spaciousness, precision typography, and a "dark mode" first approach that prioritizes content and atmospheric depth over traditional interface chrome.

## Colors

The palette is anchored in a "Deep Space" neutral (#080808) with a primary "Soft Lavender" (#D8B4FE) used for high-intent actions and focal points.

- **Primary:** Lavender provides a soft, luminous contrast against dark backgrounds. It is used for buttons, active indicators, and text glows.
- **Surface Strategy:** We avoid solid greys in favor of semi-transparent blacks with heavy backdrop blurs.
- **Accents:** Secondary indigo and tertiary slate are used sparingly for depth in gradients and lower-hierarchy UI elements.
- **Semantic Feedback:** Success states should utilize the primary lavender's glow properties rather than traditional green to maintain the specialized brand palette.

## Typography

The system uses **Plus Jakarta Sans** across all levels to maintain a cohesive, modern, and slightly geometric feel. 

- **Display & Headlines:** Use light weights (300-400) for large sizes to convey elegance. Apply a subtle `text-glow` (primary color at 30% opacity) to Display text to simulate light emission.
- **Body:** Maintains a generous line height (1.6) for readability. Body text should often be slightly de-emphasized using `on-surface-variant` colors to keep the focus on headlines.
- **Labels:** Small labels use uppercase styling with increased letter spacing (0.08em) for a "technical" or "gallery" metadata look.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy for desktop, centering content within a 1280px container, while transitioning to a fluid model for mobile devices.

- **Rhythm:** An 8px base unit drives all spacing.
- **Margins:** Desktop views utilize wide 48px margins to emphasize the "atelier" (studio) feel, providing plenty of negative space.
- **Verticality:** Use large sections of vertical padding (80px - 120px) between major content blocks to allow the background visuals to breathe.

## Elevation & Depth

Depth is created through **Glassmorphism** and light manipulation rather than traditional drop shadows.

- **Surfaces:** Use `glass-panel` effects: 70% opacity backgrounds combined with 24px backdrop blurs. This allows background video or gradients to bleed through softly.
- **Borders:** "Ghost borders" (1px solid white at 10% opacity) define edges without creating heavy visual weight.
- **Atmosphere:** Use radial gradients in the background (vignettes) to draw the eye toward the center of the screen. 
- **Active Elevation:** When elements are hovered, use inner glows or outer primary-tinted shadows (`rgba(236, 215, 255, 0.3)`) to simulate a physical light source being activated.

## Shapes

The shape language is primarily **Pill-shaped** for interactive elements and **Rounded** for containers.

- **Buttons & Chips:** Always use `rounded-full` (pill) to create a soft, inviting interaction point that contrasts with the structured grid.
- **Panels:** Larger content panels or cards use a consistent 0.5rem (8px) base radius, stepping up to 0.75rem (12px) for high-level containers.
- **Interactive Feedback:** Use scale transforms (e.g., `scale-95`) on click to reinforce the tactile nature of the UI.

## Components

### Buttons
- **Primary:** Gradient fill (Primary to Primary-Container), pill-shaped, with a leading or trailing icon. On hover, apply a soft primary glow shadow.
- **Secondary/Ghost:** Transparent background with the 10% white border. Subtle background fill change on hover.

### Chips / Status Indicators
- Used for "Available for projects" or category tags. Small pill-shaped glass panels.
- Include a 2x2 unit pulsing dot (Primary color) to indicate "live" or "available" status.

### Navigation
- **Docked Bar:** Full-width, top-positioned with a strong backdrop blur and bottom border.
- **Links:** Uppercase `label-sm` typography. Hover states should include a subtle background highlight (`white/5`) and a smooth transition.

### Input Fields
- Dark backgrounds, 10% white border, with 16px horizontal padding. Focus states should transition the border to the Primary color with a subtle outer glow.

### Cards & Panels
- Utilize the `glass-panel` class. Content should be padded with at least 32px (4 units) to maintain the airy, minimalist aesthetic.