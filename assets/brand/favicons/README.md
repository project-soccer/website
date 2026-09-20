# Favicon Exports

Derived from the unchanged [SVG brand master](../project-soccer-logo.svg) on 2026-09-20. This directory is the canonical export set; the game repository carries deployment copies in `client/public/` so it builds independently.

| File | Use |
|---|---|
| `favicon.svg` | Scalable browser tab icon; exact copy of the master |
| `favicon.ico` | Browser fallback with 16 × 16 and 32 × 32 PNG frames |
| `favicon-16.png`, `favicon-32.png` | Standalone raster exports |
| `apple-touch-icon.png` | 180 × 180 opaque touch icon, emblem inset on the game's dark background |

The SVG/ICO/PNG tab icons retain transparent exteriors and opaque football interiors. The touch icon intentionally has an opaque background. PNGs were rasterized directly from the SVG with Sharp; the ICO container embeds those PNG exports. Regenerate from the master instead of editing raster pixels. Copy updated exports into the game client when changing the canonical set.

The game HTML declares the SVG, ICO fallback and touch icon. No website has been deployed, and no installable/offline web-app behavior is implied.
