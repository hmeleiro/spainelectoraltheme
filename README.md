**pkgdown template for the [Spain Electoral Project](https://spainelectoralproject.com/).**

Provides the unified visual identity (colors, typography, component styles) for all R packages in the ecosystem:

## Ejemplos de componentes visuales

<div style="max-width: 720px; margin: 2rem auto;">
  <h1 style="font-size:2.25rem; font-weight:700; margin-bottom:0.5rem;">Spain Electoral Project UI</h1>
  <p style="color:var(--color-text-secondary); font-size:1.125rem; margin-bottom:2rem;">Ejemplo de componentes y estilo global del proyecto.</p>

  <!-- Botones -->
  <h2 style="font-size:1.25rem; margin-top:2rem;">Botones</h2>
  <button style="background:#2d5bff; color:#fff; border:none; border-radius:0.5rem; padding:0.75rem 1.5rem; font-size:1rem; font-family:var(--font-sans); font-weight:600; margin-right:1rem; box-shadow:var(--shadow-sm); transition:background 150ms;">Primario</button>
  <button style="background:#fff; color:#1a1a2e; border:1px solid #e5e7eb; border-radius:0.5rem; padding:0.75rem 1.5rem; font-size:1rem; font-family:var(--font-sans); font-weight:600;">Secundario</button>

  <!-- Badges -->
  <h2 style="font-size:1.25rem; margin-top:2rem;">Badges</h2>
  <span style="display:inline-block; background:#ecfdf5; color:#0d9488; border-radius:9999px; padding:0.25rem 1rem; font-size:0.875rem; font-weight:600; margin-right:0.5rem;">Dataset</span>
  <span style="display:inline-block; background:#f3e8ff; color:#7c3aed; border-radius:9999px; padding:0.25rem 1rem; font-size:0.875rem; font-weight:600; margin-right:0.5rem;">Paquete</span>
  <span style="display:inline-block; background:#fef3c7; color:#d97706; border-radius:9999px; padding:0.25rem 1rem; font-size:0.875rem; font-weight:600; margin-right:0.5rem;">Metodología</span>
  <span style="display:inline-block; background:#dbeafe; color:#2563eb; border-radius:9999px; padding:0.25rem 1rem; font-size:0.875rem; font-weight:600;">API</span>

  <!-- Card ejemplo -->
  <h2 style="font-size:1.25rem; margin-top:2rem;">Card</h2>
  <div style="background:#fff; border:1px solid #e5e7eb; border-radius:0.75rem; box-shadow:0 2px 8px rgba(0,0,0,0.06); padding:2rem; margin-bottom:2rem; max-width:420px;">
    <h3 style="margin-top:0; font-size:1.25rem;">Título de Card</h3>
    <p style="color:#5a5a7a; margin-bottom:0.5rem;">Descripción breve de la card, siguiendo el estilo minimalista y profesional.</p>
    <button style="background:#2d5bff; color:#fff; border:none; border-radius:0.5rem; padding:0.5rem 1.25rem; font-size:1rem; font-family:var(--font-sans); font-weight:600;">Acción</button>
  </div>

  <!-- Input ejemplo -->
  <h2 style="font-size:1.25rem; margin-top:2rem;">Input</h2>
  <input type="text" placeholder="Introduce texto..." style="width:100%; max-width:320px; padding:0.75rem 1rem; border:1px solid #e5e7eb; border-radius:0.5rem; font-size:1rem; font-family:var(--font-sans); background:#fff; color:#1a1a2e; margin-bottom:2rem;">
</div>
# spainelectoraltheme

**pkgdown template for the [Spain Electoral Project](https://spainelectoralproject.com/).**

Provides the unified visual identity (colors, typography, component styles) for all R packages in the ecosystem:

- [infoelectoral](https://github.com/rOpenSpain/infoelectoral)
- [opencis](https://github.com/hmeleiro/opencis)
- [eleccionesdb](https://github.com/hmeleiro/eleccionesdb-r)
- [vota](https://github.com/hmeleiro/vota)

## Installation

```r
# install.packages("pak")
pak::pak("hmeleiro/spainelectoraltheme")
## Usage
```r
# install.packages("pak")
In your package's `_pkgdown.yml`:
```

```yaml
template:
  package: spainelectoraltheme
  bootstrap: 5
```

That's it. The template provides:

- **Design tokens**: colors (`#2d5bff` accent), backgrounds, borders
- **Typography**: Inter (sans) + JetBrains Mono (code) via Google Fonts
- **Navbar**: white background, `◆` diamond branding, clean navigation
- **Code blocks**: light background with syntax highlighting for downlit tokens
- **Components**: cards, sidebar, buttons, footer — all styled consistently

## Customization

Override any bslib variable in your package's `_pkgdown.yml`:

```yaml
template:
  package: spainelectoraltheme
  bootstrap: 5
  bslib:
    primary: "#0066cc"  # Override accent color
```

## Design System

The template mirrors the design tokens from [spainelectoralproject.com](https://spainelectoralproject.com/):

| Token | Value |
|---|---|
| Primary / Accent | `#2d5bff` |
| Background | `#fafbfc` |
| Text | `#1a1a2e` |
| Text secondary | `#5a5a7a` |
| Border | `#e5e7eb` |
| Font (body) | Inter |
| Font (code) | JetBrains Mono |
