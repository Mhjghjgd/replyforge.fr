---
name: vengenceui
description: "Animated landing page UI components (copy-paste model). Built with React, TypeScript, Tailwind CSS, Framer Motion, GSAP, and Three.js. Use when building landing pages, SaaS pages, portfolios with premium animations."
---

# VengenceUI

Modern animated UI components for landing pages. Copy-paste model (like shadcn/ui) — no npm install needed, just copy components into your project.

## Tech Stack Required
- React + TypeScript
- Tailwind CSS
- Framer Motion (`npm i framer-motion`)
- GSAP (`npm i gsap`)
- Lucide React (`npm i lucide-react`)
- Radix UI primitives (`npm i @radix-ui/react-*`)

## How to Use

1. Browse components at: https://github.com/Ashutoshx7/VengenceUI
2. Copy the component source code into your project (e.g. `src/components/ui/`)
3. Install any missing peer dependencies

## Component Categories

- **Hero sections** — animated headline, gradient text, particle effects
- **Navigation** — floating nav, blur-on-scroll navbar
- **Buttons** — magnetic, ripple, glow, shimmer effects
- **Cards** — tilt, glassmorphism, border-glow, hover-lift
- **Text effects** — typewriter, word-by-word reveal, scramble
- **Backgrounds** — aurora, mesh gradient, dot grid, beam
- **Sections** — bento grid, feature grid, testimonials, pricing
- **3D elements** — using Three.js/React Three Fiber

## Example: Glassmorphism Card
```tsx
// Copy from VengenceUI repo and adapt:
<div className="relative backdrop-blur-md bg-white/10 border border-white/20 rounded-2xl p-6 shadow-xl">
  {children}
</div>
```

## Best Practices
- Components are designed for dark backgrounds — use `bg-black` or deep gradient as base
- Pair with ShaderGradient for animated gradient backgrounds
- Use `will-change: transform` on animated elements for performance
- Lazy-load heavy 3D components with `next/dynamic` or React.lazy
