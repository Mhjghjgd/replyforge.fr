---
name: shadergradient
description: "3D animated shader gradients using Three.js/WebGL. Use when adding animated gradient backgrounds, hero sections, or visual effects. Package @shadergradient/react is already installed."
---

# ShaderGradient

Animated 3D gradients powered by Three.js/WebGL shaders. Already installed: `@shadergradient/react`.

## Installation (already done)
```bash
npm i @shadergradient/react @react-three/fiber three three-stdlib camera-controls
```

## Basic Usage

```tsx
import { ShaderGradient, ShaderGradientCanvas } from '@shadergradient/react'

export function GradientBackground() {
  return (
    <ShaderGradientCanvas style={{ position: 'absolute', inset: 0 }}>
      <ShaderGradient
        type="waterPlane"
        animate="on"
        uTime={0.2}
        uSpeed={0.3}
        uStrength={1.5}
        uDensity={1.5}
        uFrequency={5.5}
        uAmplitude={1}
        positionX={0}
        positionY={0}
        positionZ={0}
        rotationX={50}
        rotationY={0}
        rotationZ={-60}
        color1="#ff5ca0"
        color2="#3b82f6"
        color3="#000000"
        reflection={0.1}
        wireframe={false}
        shader="defaults"
        envPreset="city"
        lightType="3d"
        brightness={1.2}
        grain="off"
        cAzimuthAngle={180}
        cPolarAngle={80}
        cDistance={2.8}
        cameraZoom={9.1}
      />
    </ShaderGradientCanvas>
  )
}
```

## Key Props

| Prop | Values | Description |
|------|--------|-------------|
| `type` | `plane`, `sphere`, `waterPlane` | Mesh geometry |
| `animate` | `on`, `off` | Toggle animation |
| `color1/2/3` | hex string | Gradient colors |
| `uSpeed` | 0–1 | Animation speed |
| `uStrength` | 0–4 | Distortion strength |
| `grain` | `on`, `off` | Film grain effect |
| `envPreset` | `city`, `dawn`, `lobby` | Lighting environment |

## From URL (shadergradient.co configurator)
```tsx
<ShaderGradient urlString="https://www.shadergradient.co/customize?animate=on&type=waterPlane&..." />
```

Use the configurator at shadergradient.co to visually design and get a URL.

## Best Practices
- Wrap in a `position: relative` container, set canvas to `position: absolute; inset: 0`
- Set `pointer-events: none` on the canvas for hero sections behind content
- Use `grain="on"` for a more organic feel
- Keep `uSpeed` under 0.5 for subtle backgrounds
