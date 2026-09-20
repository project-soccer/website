# Project Soccer — Vector Brand Master

- Master: [project-soccer-logo.svg](project-soccer-logo.svg)
- PNG export: [project-soccer-logo.png](project-soccer-logo.png), 1024 × 1024 RGBA
- Historical generated reference: [avatar v1 in Git history](https://github.com/project-soccer/website/blob/b0dbb66e1189645457290f6a4f7e2c1e8089747b/assets/brand/project-soccer-github-avatar-v1.png)
- Decision: ADR 0013 in the game repository.

Created on 2026-09-20 at the founder's request as native vector geometry. The approved generated football/PS emblem was manually reconstructed with circles and editable paths; small geometric irregularities were regularized. This is not an embedded bitmap, automatic noisy trace, or a new image-generator output. It contains no external fonts, scripts, or linked resources.

A fully opaque black disc underlies the white panels and PS monogram. Letter counters and dark gaps therefore remain black on any background. The exterior alone is transparent, with normal raster edge antialiasing on export. The master has a 1254-square viewBox and approximately two units of outer padding.

The PNG was rasterized directly from the SVG with Sharp. The SVG is the source of truth; regenerate exports from it rather than editing PNG pixels. The earlier generator output is retained in Git history and is no longer the canonical logo.

The SVG and PNG were checked over pink and for interior alpha. General brand/software licensing is not selected here. Storing these assets does not apply the organization avatar on GitHub.
