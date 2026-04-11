# TJT Media Hub — Plan

## Project Goal

Create a dark, futuristic landing page for **tjt-media.online** that acts as a central hub for services, tools, dashboards, and future experiments.

## Core Purpose

* Central launch point for subdomains and self-hosted services
* Clean identity for the overall TJT Media ecosystem
* Easy to expand and update over time
* Mobile-first and suitable for GitHub Pages

---

## Design Direction

### Vibe

* Dark theme
* Bold, futuristic, polished
* Sci-fi / next-gen feel
* Animated, but readable and controlled
* Modular and easy to extend

### Color Palette

#### Core colors

* `--color-bg: #0b0b12`
* `--color-surface: #14141d`
* `--color-surface-2: #1b1b27`
* `--color-text: #f5f7ff`
* `--color-text-muted: #a7abc0`
* `--color-accent: #8b5cf6`
* `--color-accent-soft: rgba(139, 92, 246, 0.18)`
* `--color-border: rgba(255, 255, 255, 0.08)`

### Typography

#### Font stack

* `--font-heading: "Inter", "Segoe UI", system-ui, -apple-system, sans-serif`
* `--font-body: "Inter", "Segoe UI", system-ui, -apple-system, sans-serif`
* `--font-mono: "JetBrains Mono", "Fira Code", monospace`

#### Font sizes

* `--font-size-xs: 0.75rem`
* `--font-size-sm: 0.875rem`
* `--font-size-md: 1rem`
* `--font-size-lg: 1.25rem`
* `--font-size-xl: 1.75rem`
* `--font-size-xxl: 2.5rem`

### Shape / Radius

* `--radius-sm: 0.5rem`
* `--radius-md: 0.75rem`
* `--radius-lg: 1rem`

### Shadows / Depth

* `--shadow-sm: 0 4px 12px rgba(0,0,0,0.25)`
* `--shadow-md: 0 10px 30px rgba(0,0,0,0.35)`
* `--shadow-lg: 0 20px 60px rgba(0,0,0,0.45)`

### Glow System

* `--glow-accent: 0 0 20px rgba(139, 92, 246, 0.35)`
* `--glow-accent-strong: 0 0 40px rgba(139, 92, 246, 0.55)`

### Motion

* `--duration-fast: 120ms`
* `--duration-base: 220ms`
* `--duration-slow: 420ms`
* `--ease-standard: cubic-bezier(0.4, 0, 0.2, 1)`
* `--ease-smooth: cubic-bezier(0.25, 0.1, 0.25, 1)`

---

## Design Tokens

### Spacing scale

* `--space-xs: 0.25rem`
* `--space-sm: 0.5rem`
* `--space-md: 1rem`
* `--space-lg: 1.5rem`
* `--space-xl: 2rem`
* `--space-xxl: 3rem`

### Radius scale

* `--radius-sm: 0.5rem`
* `--radius-md: 0.75rem`
* `--radius-lg: 1rem`

### Shadow tokens

* `--shadow-sm: 0 4px 12px rgba(0,0,0,0.25)`
* `--shadow-md: 0 10px 30px rgba(0,0,0,0.35)`
* `--shadow-lg: 0 20px 60px rgba(0,0,0,0.45)`

### Motion tokens

* `--duration-fast: 120ms`
* `--duration-base: 220ms`
* `--duration-slow: 420ms`
* `--ease-standard: cubic-bezier(0.4, 0, 0.2, 1)`
* `--ease-smooth: cubic-bezier(0.25, 0.1, 0.25, 1)`

### Layout tokens

* `--container-width: 1100px`
* `--container-wide: 1400px`
* `--breakpoint-sm: 640px`
* `--breakpoint-md: 768px`
* `--breakpoint-lg: 1024px`
* `--breakpoint-xl: 1280px`

---

## Site Structure

1. Header
2. Hero / intro
3. Main hub / card grid
4. Future sections as needed
5. Footer

---

## Layout System

### General layout

* Mobile-first
* Spacious hero area
* Tighter, efficient content sections
* Consistent max-width containers
* Clean vertical rhythm between sections

### Grid behavior

* Mobile: 1 column
* Tablet: 2 columns
* Desktop: 3+ columns

### Section structure

Each section should use:

* outer section wrapper
* inner container
* content area

---

## Reusable Components

### Header

Purpose:

* Branding + navigation

Contents:

* site title / wordmark
* nav links
* mobile menu trigger

Behavior:

* non-sticky in v1
* desktop: horizontal nav
* mobile: collapsed menu

### Navigation

Placeholder items:

* Home
* Media Server
* Dashboard
* Tools
* Projects
* About

Desktop:

* horizontal layout
* subtle hover animation

Mobile:

* simple dropdown / collapse menu
* vertical stacked links
* large tap targets

### Hero

Purpose:

* Set tone and identity
* Explain what the site is

Contents:

* bold headline
* short supporting description
* optional quick actions / CTA buttons
* animated visual layer or gradient background

Layout:

* mobile: stacked
* desktop: more spacious, possible split layout

### Card

Purpose:

* Primary unit for services, dashboards, tools, and future content

Required contents:

* title
* short description
* primary action

Optional contents:

* icon or visual
* tag / badge
* secondary action

Behavior:

* mobile: full-width stacked cards
* desktop: grid layout with hover interaction
* subtle lift / glow / border emphasis on hover

Future card data fields:

* title
* description
* url
* icon
* category
* status

### Footer

Purpose:

* reusable bottom section for brand and utility links

Possible contents:

* site name
* short text / tagline
* quick links
* GitHub / social links

---

## Base Styling Categories

* reset / normalization
* body background and text defaults
* typography scale
* link defaults
* container widths
* section spacing
* focus states
* transition conventions

---

## Suggested File Structure

```text
project/
├── index.html
├── plan.md
├── assets/
│   ├── images/
│   ├── icons/
│   └── fonts/
├── css/
│   ├── variables.css
│   ├── base.css
│   ├── layout.css
│   ├── components.css
│   ├── utilities.css
│   └── animations.css
├── js/
│   ├── main.js
│   └── components/
└── data/
    └── services.json
```

## File Definitions

* `variables.css`: colors, spacing, radii, shadows, timing, layout tokens
* `base.css`: reset, body styles, typography, defaults
* `layout.css`: containers, grid, section spacing, structure
* `components.css`: header, nav, hero, cards, footer, buttons
* `utilities.css`: optional helper classes
* `animations.css`: motion and effect rules
* `main.js`: navigation toggle and lightweight interactions
* `services.json`: optional future content source for cards

---

## Build Priorities

1. Set up file structure
2. Define variables and design tokens
3. Build base styles
4. Build layout containers and section system
5. Build header and navigation
6. Build hero
7. Build card grid
8. Add responsive behavior
9. Add animation polish

---

## Notes

* Keep the first version consistent and simple
* Reuse tokens and components everywhere
* Add complexity through polish, not through messy structure
* Build a clean foundation first, then experiment
