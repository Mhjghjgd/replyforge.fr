---
name: forgeui
description: "WebGL-powered animated React components: shader backgrounds (Cloudscape, Lumadrift, Velora, Auralis...), animated cards, security UIs, text effects, OTP inputs. Copy-paste via shadcn registry. Use for SaaS landing pages with premium animated backgrounds and interactive components."
---

# ForgeUI

Animation-first React component library. Components are added via the shadcn registry from forgeui.in.

## Installation (per component)
```bash
npx shadcn@latest add "https://forgeui.in/r/<component-name>"
```

## WebGL Backgrounds (les plus impressionnants)

| Component | Effect |
|-----------|--------|
| `cloudscape` | Nuages animés, ciel doux |
| `lumadrift` | Lumière fluide, patterns procéduraux |
| `cosmicrift` | Espace, étoiles scintillantes, nébuleuse |
| `chromatic-fluid` | Fluide chromatique, grain cinématographique |
| `velora` | Traînées lumineuses radiales, 3D noise |
| `velaris` | Simplex noise multicouches, vignette |
| `auralis` | Aurora dramatique, bloom lumineux |
| `nebulore` | Rubans aurora, domain-warped noise |
| `noctylis` | Lueur nocturne, violet, grain cinéma |

```bash
# Exemple : fond cosmique pour hero
npx shadcn@latest add "https://forgeui.in/r/cosmicrift"
```

## UI Components

| Component | Description |
|-----------|-------------|
| `animated-form` | Formulaire avec checkmarks progressifs |
| `animated-tabs` | Tabs avec underline animé |
| `animated-otp` | OTP glowing, simulation auth |
| `bot-detection` | Radar animé, détection en temps réel |
| `security-card` | Carte identité sécurisée, character scramble |
| `vault-lock` | Coffre-fort interactif au hover |
| `fraud-card` | Alerte sécurité style Clerk |
| `notification-center` | Centre de notifs mobile animé |
| `text-shimmer` | Effet shimmer sur texte |
| `text-morph` | Rotation de mots animés |
| `text-reveal` | Apparition séquentielle de texte |
| `spectrum-switcher` | Sélecteur de thème avec gradients |
| `stats-card` | Comparaison stats avec graphe animé |
| `stack-ripple` | Notifications empilées en ripple |

## Best Practices
- Les fonds WebGL remplacent avantageusement ShaderGradient pour des effets cinématiques
- Utiliser sur fond noir (`bg-black`) ou très sombre
- Pair avec `text-shimmer` ou `text-reveal` pour les titres hero
- `lazy import` obligatoire pour les WebGL components (code splitting)
