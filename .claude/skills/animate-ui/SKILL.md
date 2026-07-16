---
name: animate-ui
description: "Fully animated open-source component library built with React, TypeScript, Tailwind CSS, and Motion. Registry-based (like shadcn). Use when adding pre-built animated components to a React/Next.js project."
---

# Animate UI

Animated component distribution built with React, TypeScript, Tailwind CSS, and Motion (Framer Motion).

## Registry Model (like shadcn/ui)

Components are added via the shadcn CLI pointing to the animate-ui registry:

```bash
npx shadcn@latest add "https://animate-ui.com/r/<component-name>"
```

## Prerequisites
```bash
npm i motion tailwindcss
```

## Available Components

Browse the full list at: https://animate-ui.com/docs

Key categories:
- **Animated text** — typewriter, char-by-char, word reveal, blur-in
- **Transitions** — page transitions, route animations
- **Loaders** — spinners, skeleton, progress bars
- **Interactive** — animated buttons, toggles, inputs
- **Layout** — animated accordions, tabs, modals
- **Numbers** — animated counters, odometers

## Example: Add a component
```bash
# Add typewriter text effect
npx shadcn@latest add "https://animate-ui.com/r/typewriter"

# Add animated counter
npx shadcn@latest add "https://animate-ui.com/r/number-flow"
```

## Usage After Adding
```tsx
import { Typewriter } from '@/components/ui/typewriter'

export function Hero() {
  return (
    <Typewriter
      words={['Beautiful', 'Animated', 'Components']}
      loop
      cursor
    />
  )
}
```

## Integration with Other Skills
- Pair with **shadergradient** for animated backgrounds + animated text
- Pair with **vengenceui** for layout components + animate-ui for micro-interactions
- Pair with **ui-ux-pro-max** for design system guidance

## Docs
https://animate-ui.com/docs
