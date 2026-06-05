---
name: High-Velocity Automation
colors:
  surface: '#131315'
  surface-dim: '#131315'
  surface-bright: '#39393b'
  surface-container-lowest: '#0e0e10'
  surface-container-low: '#1b1b1d'
  surface-container: '#1f1f21'
  surface-container-high: '#2a2a2c'
  surface-container-highest: '#343536'
  on-surface: '#e4e2e4'
  on-surface-variant: '#c5c6cd'
  inverse-surface: '#e4e2e4'
  inverse-on-surface: '#303032'
  outline: '#8f9097'
  outline-variant: '#44474d'
  surface-tint: '#b9c7e4'
  primary: '#b9c7e4'
  on-primary: '#233148'
  primary-container: '#0a192f'
  on-primary-container: '#74829d'
  inverse-primary: '#515f78'
  secondary: '#b6c6ed'
  on-secondary: '#20304f'
  secondary-container: '#374767'
  on-secondary-container: '#a5b5db'
  tertiary: '#e7bf99'
  on-tertiary: '#432b10'
  tertiary-container: '#281400'
  on-tertiary-container: '#9d7b5a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d6e3ff'
  primary-fixed-dim: '#b9c7e4'
  on-primary-fixed: '#0d1c32'
  on-primary-fixed-variant: '#39475f'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#b6c6ed'
  on-secondary-fixed: '#091b39'
  on-secondary-fixed-variant: '#374767'
  tertiary-fixed: '#ffdcbd'
  tertiary-fixed-dim: '#e7bf99'
  on-tertiary-fixed: '#2b1701'
  on-tertiary-fixed-variant: '#5d4124'
  background: '#131315'
  on-background: '#e4e2e4'
  surface-variant: '#343536'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-table:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 40px
  xl: 64px
  gutter: 24px
  margin: 32px
---

## Brand & Style

This design system is engineered for professional automation and high-stakes data management. The brand personality is rooted in **precision, speed, and reliability**, catering to technical operators who require clarity in complex workflows.

The visual style is **Technological Minimalism** infused with **Glassmorphism**. It utilizes a sophisticated dark mode foundation to reduce eye strain during long sessions, while employing vibrant, high-energy accents to denote activity and status. The aesthetic balances the density of a data-rich dashboard with the breathable elegance of modern SaaS, ensuring that critical information is never obscured by visual clutter.

## Colors

The palette is optimized for a technical environment, using depth and luminance to establish hierarchy:

- **Primary & Secondary Backgrounds:** Use the deep navy (#0A192F) for the global canvas and charcoal grey (#112240) for elevated containers like cards and sidebars.
- **Electric Blue (#64FFDA):** Reserved for primary actions, success states, and active automation glows. It provides a "high-tech" feel and high contrast against the dark base.
- **Bright Orange (#FF8C00):** Used for attention-seeking elements, warnings, and secondary CTAs to ensure they stand out without competing with the primary action color.
- **Neutral Tones:** Use a range of desaturated blues and silvers for typography to maintain a soft but legible contrast, avoiding pure white to prevent "halation" effects on dark backgrounds.

## Typography

The system relies on **Inter** for its exceptional legibility in UI environments and high x-height, making it ideal for dense data tables. **JetBrains Mono** is introduced as a secondary label font for technical metadata, status codes, and monospaced values, reinforcing the "automation" aesthetic.

- **Headlines:** Should use tighter letter-spacing to appear more structural and impactful.
- **Labels:** Always uppercase when using the monospaced font to differentiate from standard body copy.
- **Data Tables:** Use a slightly reduced font size with generous line-height to ensure readability across massive datasets.

## Layout & Spacing

This design system utilizes a **12-column fluid grid** for dashboard views, allowing widgets to reflow based on screen real estate. 

- **Desktop (1440px+):** 12 columns, 24px gutters, 40px side margins.
- **Tablet (768px - 1439px):** 8 columns, 16px gutters, 24px side margins.
- **Mobile (<768px):** 4 columns, 12px gutters, 16px side margins.

Spacing follows an 8px base unit. Internal card padding should be a minimum of 24px (`md`) to maintain a premium, spacious feel despite the dark, technical nature of the content. Layouts should prioritize "Top-Down" hierarchy, placing global KPIs at the header and granular logs at the footer.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and **Tonal Layering**. 

1. **Base Layer:** The global background (#0A192F).
2. **Container Layer:** Cards use the charcoal grey (#112240) with a 60% opacity background-blur (20px) to create a frosted glass effect.
3. **Accent Elevation:** Active automation tasks or "focused" widgets use a 1px solid border of Electric Blue (#64FFDA) with a soft outer glow (`box-shadow: 0 0 15px rgba(100, 255, 218, 0.3)`).
4. **Interactive Elements:** Buttons and clickable cards should shift up by 2px on hover, increasing the blur radius of the shadow to simulate physical lifting.

## Shapes

The system uses a **Rounded** (Level 2) language to soften the technical edge of the platform. 

- **Standard Components:** 8px (0.5rem) radius for buttons and input fields.
- **Dashboard Cards:** 16px (1rem) radius for primary containers.
- **Task 'Tick' Cards:** 12px radius to strike a balance between the two.

Avoid sharp corners to maintain an approachable "SaaS" feel, but do not use fully pill-shaped elements for structural containers to ensure they still feel professional and stable.

## Components

### Data Upload Zones
Use a dashed border (`2px dashed #233554`) with a centered icon. Upon dragging a file over the zone, the border and background should transition to Electric Blue at 10% opacity.

### Automation Task Cards (Multi-select)
These cards feature a checkbox in the top-right corner. When selected, the entire card gains the "active glow" border. The "tick" should be the Electric Blue accent color.

### Pricing Tables
- **Free Tier:** Simple charcoal background, no glow, outlined primary button.
- **Premium Tier:** Features a subtle gradient border and the Electric Blue glowing effect to denote "Recommended" or "High Value." Use the Bright Orange for the "Upgrade" CTA.

### Admin Dashboard Widgets
Widgets should contain a header with monospaced labels for technical data points. Graphs and visualizations should use high-contrast Electric Blue for lines and Bright Orange for outliers/alerts.

### Ad Banner Placeholders
Integrate AdSense banners within standard card containers to maintain visual consistency. Use a subtle label "Sponsored Content" in the monospaced label font at the top-right.

### Payment & Brand Assets
- **Payment Icons:** GPay, PhonePe, and PayPal should be housed in white or light-grey rounded-rect containers to ensure brand colors are legible against the dark UI.
- **Status Indicators:** Use small, pulsing circular pips next to text to show "Live" or "Running" status in Electric Blue.