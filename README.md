# spain-electoral-theme

**pkgdown template for the [Spain Electoral Project](https://spainelectoralproject.com/).**

Provides the unified visual identity (colors, typography, component styles) for all R packages in the ecosystem:

- [infoelectoral](https://github.com/rOpenSpain/infoelectoral)
- [opencis](https://github.com/hmeleiro/opencis)
- [eleccionesdb](https://github.com/hmeleiro/eleccionesdb-r)
- [vota](https://github.com/hmeleiro/vota)

## Installation

```r
# install.packages("pak")
pak::pak("hmeleiro/septheme")
## Usage
```r
# install.packages("pak")
In your package's `_pkgdown.yml`:
```

```yaml
template:
  package: spain-electoral-theme
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
  package: septheme
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
