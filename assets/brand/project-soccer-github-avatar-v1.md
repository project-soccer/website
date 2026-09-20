# Project Soccer — GitHub Avatar v1 (Format Revision)

Asset: [project-soccer-github-avatar-v1.png](project-soccer-github-avatar-v1.png)

Created on 2026-09-20 using the built-in image generation tool through the imagegen skill. No CLI/API fallback was used. The final generated PNG was copied into this workspace without modification. The asset is included in the public website repository. Applying it as the GitHub organization avatar is a separate action.

The founder approved the monochrome football emblem with integrated PS initials and requested a transparent exterior, opaque interior, and tight framing. The current 1254 × 1254 RGBA PNG replaces the earlier padded, black-background asset at the same path. It was edited with the built-in image generator and copied without pixel processing. The raster file is not a vector asset.

Validation found transparent corners and near-edge-to-edge framing. The generator still leaves interior alpha values of 252–254 rather than exactly 255, with minor edge residue. The founder was informed and explicitly chose to keep the generator output instead of deterministic pixel cleanup. This file therefore does not meet strict full-opacity requirements; a very small background contribution remains possible. No claim of exact binary transparency is made.

## Initial generation prompt

```text
Use case: logo-brand
Asset type: GitHub organization avatar for Project Soccer, a browser-based 3D multiplayer football game.
Primary request: Create one polished, original logo symbol for Project Soccer.
Subject: A bold, compact football emblem with a clever, subtle integration of the initials "PS" into simplified soccer-ball panel geometry. Football should be immediately recognizable; the monogram is secondary. Make it distinctive and intentional, not a generic stock soccer ball.
Style/medium: Minimal flat vector-like brand design rendered as a crisp raster image, strong silhouette, carefully balanced negative space, very few substantial shapes.
Composition/framing: Square 1:1 canvas, preferably 1024 by 1024. One centered emblem occupying about 70 percent of the canvas. Generous consistent padding so the complete mark remains intact in circular avatar crops. Must remain legible at small avatar sizes.
Scene/backdrop: A clean solid opaque background, strong contrast between symbol and background. Restrained visual treatment.
Text: No full wordmark, captions, or slogan. Only the initials "PS" may be integrated into the emblem.
Constraints: Deliver the actual standalone logo image, not a presentation board, not a mockup, not multiple alternatives. No gradients, shadows, glow, 3D extrusion, texture, fine decorative lines, watermarks, cryptocurrency symbols, existing football club badges, or GitHub mascots.
```

## Original flat-rendering refinement prompt

Input: the initial generated emblem.

```text
Use case: logo-brand
Asset type: Final GitHub organization avatar for Project Soccer.
Input image: edit target, the existing monochrome soccer ball with integrated PS initials.
Change only the rendering finish: remove all glow, haze, halos, gradients, lighting, and soft shading. Make the same logo a completely flat clean white mark on a solid opaque black background. Use crisp antialiased edges, with every shape interior uniformly white and every negative-space/background region uniformly black.
Preserve the existing PS letter geometry, soccer-ball panel layout, circle silhouette, centered placement, proportions, square canvas, and generous outer padding exactly. Do not redesign or add elements. No new text. The result must look like a precise flat brand mark, never illuminated.
```

## Transparency and framing edit prompt

Input: the approved padded emblem.

```text
Use case: background-extraction
Asset type: Project Soccer GitHub avatar, PNG with true alpha transparency.
Input image: edit target, the approved white-and-black soccer-ball logo containing the PS monogram.
Primary request: Change only the background transparency and canvas framing. Preserve the approved design, panel geometry, PS letterforms, circular silhouette, monochrome colors and flat crisp finish.
Transparency: Treat the entire circular football as ONE SOLID OPAQUE DISC. Every pixel inside its outer circumference, INCLUDING ALL BLACK PANELS, ALL BLACK GAPS, THE BLACK CENTER PENTAGON, THE COUNTER INSIDE P, AND THE DARK AREAS AROUND PS, must remain opaque solid black or opaque solid white (alpha 255). ONLY the area OUTSIDE the outer circular football outline is truly transparent (alpha 0). Partial alpha is allowed only on the outer antialiased silhouette edge. Do not remove black areas from inside the football. If placed over pink, nothing inside the football may turn pink.
Framing: Remove the existing large margins. Tightly crop the square canvas to the circular football's bounding box: top, bottom, left and right extremes of the circle should reach the canvas edges, allowing at most 1-2 pixels to preserve antialiasing. No extra padding, and no clipping of the outer white rim. Enlarge/reframe the original emblem as necessary without changing its geometry.
Output: One tightly framed square transparent PNG, preferably 1024x1024. Actual alpha channel, never a baked checkerboard. No shadow, glow, background color, added text, mockup, or redesign.
```

## Final alpha refinement prompt

Input: the first tightly framed transparent edit. The generator output was retained by explicit founder choice despite the validation limitation above.

```text
Use case: background-extraction
Edit target: the provided tightly framed Project Soccer football PS logo.
Preserve EXACTLY its design, letterforms, monochrome palette and near-edge-to-edge framing.
Correct its alpha mask and clean circular outline. The last export has alpha 254 throughout its interior and dirty speckles outside its edge. This is wrong. The entire disc must be fully OPAQUE with alpha EXACTLY 255, including every black area and white panel; pure solid black #000000 and white #FFFFFF interiors. Only the area OUTSIDE the football circle must have alpha 0. Partial alpha only within the 1-pixel outer antialiased edge. Remove every speckle/halo outside the smooth clean circle. No texture or translucent interior.
Square PNG with real alpha, tightly crop to circle with at most 1-2 pixels padding, no clipping. Deliver the standalone corrected PNG, no mockup or checkerboard.
```
