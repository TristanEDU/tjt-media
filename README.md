# TJT Media Hub

A dark, futuristic landing page serving as the central hub for the TJT Media domain ecosystem.

## Project Overview

**TJT Media Hub** is a polished, modular landing page designed to act as a central access point for services, dashboards, tools, and self-hosted applications under the `tjt-media.online` domain. Built with a focus on clean design, responsive behavior, and future extensibility.

### Core Purpose

- Central launch point for subdomains and self-hosted services
- Clean, consistent brand identity for the TJT Media ecosystem
- Mobile-first and GitHub Pages–ready
- Easy to expand with new sections and components

## Design Direction

### Vibe

- **Dark theme** with bold, futuristic aesthetics
- **Sci-fi / next-gen feel** with controlled, readable animations
- **Polished and modular** — simple to extend and maintain

### Color Palette

- **Background**: `#0b0b12`
- **Surfaces**: `#14141d`, `#1b1b27`
- **Text**: `#f5f7ff` (primary), `#a7abc0` (muted)
- **Accent**: `#8b5cf6` (purple) with soft variant
- **Border**: `rgba(255, 255, 255, 0.08)`

### Typography

- **Font Stack**: Inter, Segoe UI, system-ui
- **Mono Stack**: JetBrains Mono, Fira Code
- **Scale**: Fluid responsive, from xs (0.5em) to xxl (2.5em)
  - Body root scales via `clamp(1.5em, 2.5vw, 3em)`, flowing from ~24px on small screens to ~48px on large screens
  - All font-size tokens use em units, scaling proportionally with the root body size

## File Structure

```
project/
├── index.html              # Main page
├── plan.md                 # Design & build plan
├── README.md               # This file
├── assets/
│   ├── fonts/
│   ├── icons/
│   └── images/
├── css/
│   ├── variables.css       # Design tokens (colors, spacing, typography)
│   ├── base.css            # Base styles & defaults
│   ├── layout.css          # Structure, grid, spacing, responsive
│   ├── components.css      # Visual styling for components
│   ├── utilities.css       # Helper classes (optional)
│   └── animations.css      # Motion and effects
├── js/
│   ├── main.js             # Entry point
│   └── components/         # Component logic
└── data/
    └── services.json       # Service data (optional)
```

## CSS Organization

### variables.css

Centralized design tokens: colors, typography, spacing, shadows, motion, layout constraints.

### base.css

Body defaults, typography scale, normalization, link styles, focus states.

### layout.css

Container widths, grid systems, section spacing, flexbox layouts, responsive breakpoints.

### components.css

Visual styling for UI components: headers, hero, cards, buttons, footer. Includes colors, borders, shadows, hover states.

### utilities.css

Optional helper classes for common patterns (e.g., `.flex-center`, `.text-muted`).

### animations.css

Keyframes and animation definitions. Currently includes header zoom effect.

## Page Structure

1. **Header** (`pg-header`) — 15vh branding area with optional hero background
2. **Hero** — Full-viewport intro section with headline, description, and CTA buttons
3. **Content Cards** — Grid-based card system showcasing services and portals
4. **Footer** — Brand info, links, and social icons

## Design Tokens

### Typography Scale

The typography system uses **fluid responsive scaling**:

1. **Body Root**: `clamp(1.5em, 2.5vw, 3em)`
   - Minimum: 1.5em (locks at small viewports)
   - Preferred: 2.5vw (grows with viewport width)
   - Maximum: 3em (locks at large viewports)
   - Result: Base font smoothly scales from ~24px (small) → ~48px (large)

2. **Font-Size Variables** (all em-based, relative to body):
   - xs: 0.5em (12px–24px depending on viewport)
   - sm: 0.75em (18px–36px)
   - md: 1em (24px–48px, equals body size)
   - lg: 1.25em (30px–60px)
   - xl: 1.75em (42px–84px)
   - xxl: 2.5em (60px–120px)

**Why em units?** Because they scale *with* the body clamp, creating a proportional, fluid type scale. Every element grows and shrinks together, maintaining visual hierarchy across all viewport sizes without explicit media queries.

### Spacing Scale

- xs: 0.25rem
- sm: 0.5rem
- md: 1rem
- lg: 1.5rem
- xl: 2rem
- xxl: 3rem

### Radius Scale

- sm: 0.5rem
- md: 0.75rem
- lg: 1rem
- xl: 3rem

### Shadows

- sm, md, lg variants with accent-tinted glow effects

### Motion

- **Durations**: fast (120ms), base (220ms), slow (420ms)
- **Easing**: standard, smooth cubic-bezier curves

### Responsive Breakpoints

- sm: 640px
- md: 768px
- lg: 1024px
- xl: 1280px

## Components

### Hero

- Status indicator badge
- Bold headline with accent span
- Supporting description
- Dual-action CTA buttons
- Radial gradient background

### Card Grid

- Auto-fill responsive grid (min 320px columns)
- Individual card styling with hover effects
- Status indicator in top-right
- Icon, title, description, action button
- Text truncation on description (2 lines)

### Footer

- Branded layout with icon, text, and social links
- Responsive stacking on mobile

## Development

### Getting Started

1. Clone or download the project
2. Open `index.html` in a browser or serve locally
3. Edit CSS variables in `variables.css` to customize colors and spacing
4. Add content by duplicating card templates in `index.html`

### Customization

- **Colors**: Update CSS variables in `variables.css`
- **Typography**: Adjust `--font-size-*` variables
- **Layout**: Modify container widths and breakpoints in `layout.css`
- **Components**: Style overrides in `components.css`

### Future Enhancements

- Load card data from `services.json` via JavaScript
- Navigation menu toggle (HTML template included)
- Additional animation effects
- Dark/light mode toggle
- Search or filter functionality

## Browser Support

Modern browsers supporting CSS Custom Properties, Flexbox, and CSS Grid (all major browsers).

## Notes

- Keep the design consistent and simple
- Reuse tokens and components everywhere
- Add complexity through polish, not messy structure
- Mobile-first approach throughout

---

Built with attention to design system consistency, accessibility, and maintainability.
