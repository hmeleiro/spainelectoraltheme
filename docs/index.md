# Spain Electoral Project UI

**pkgdown template for the [Spain Electoral
Project](https://spainelectoralproject.com/).**

Provides the unified visual identity (colors, typography, component
styles) for all R packages in the ecosystem:

## Ejemplos de componentes visuales

Ejemplo de componentes y estilo global del proyecto.

## Botones

Primario Secundario

## Badges

Dataset Paquete Metodología API

## Card

``` R
<h3 style="margin-top:0; font-size:1.25rem;">Título de Card</h3>
<p style="color:#5a5a7a; margin-bottom:0.5rem;">Descripción breve de la card, siguiendo el estilo minimalista y profesional.</p>
<button style="background:#2d5bff; color:#fff; border:none; border-radius:0.5rem; padding:0.5rem 1.25rem; font-size:1rem; font-family:var(--font-sans); font-weight:600;">Acción</button>
```

## Input

# spainelectoraltheme

**pkgdown template for the [Spain Electoral
Project](https://spainelectoralproject.com/).**

Provides the unified visual identity (colors, typography, component
styles) for all R packages in the ecosystem:

- [infoelectoral](https://github.com/rOpenSpain/infoelectoral)
- [opencis](https://github.com/hmeleiro/opencis)
- [eleccionesdb](https://github.com/hmeleiro/eleccionesdb-r)
- [vota](https://github.com/hmeleiro/vota)

## Installation

``` r
# install.packages("pak")
pak::pak("hmeleiro/spainelectoraltheme")
## Usage
```r
# install.packages("pak")
In your package's `_pkgdown.yml`:
```

``` yaml
template:
  package: spainelectoraltheme
  bootstrap: 5
```

That’s it. The template provides:

- **Design tokens**: colors (`#2d5bff` accent), backgrounds, borders
- **Typography**: Inter (sans) + JetBrains Mono (code) via Google Fonts
- **Navbar**: white background, `◆` diamond branding, clean navigation
- **Code blocks**: light background with syntax highlighting for downlit
  tokens
- **Components**: cards, sidebar, buttons, footer — all styled
  consistently

## Customization

Override any bslib variable in your package’s `_pkgdown.yml`:

``` yaml
template:
  package: spainelectoraltheme
  bootstrap: 5
  bslib:
    primary: "#0066cc"  # Override accent color
```

## Design System

The template mirrors the design tokens from
[spainelectoralproject.com](https://spainelectoralproject.com/):

| Token            | Value          |
|------------------|----------------|
| Primary / Accent | `#2d5bff`      |
| Background       | `#fafbfc`      |
| Text             | `#1a1a2e`      |
| Text secondary   | `#5a5a7a`      |
| Border           | `#e5e7eb`      |
| Font (body)      | Inter          |
| Font (code)      | JetBrains Mono |
