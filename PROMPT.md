# Flora — Interactive 3D Flower Garden

## What to build
A single-file HTML game (index.html) — an interactive 3D relaxing flower garden using Three.js (loaded from CDN). No build step, no npm, no server needed — just open index.html in a browser.

## Design requirements
- **Relaxing, meditative atmosphere** — soft ambient lighting, gentle camera movement, calming color palette (warm beiges, soft pastels, deep greens)
- **Professional, design-forward aesthetic** — this should impress someone with a design background. Think: art installation, not generic web game
- **Flowers**: orchids (phalaenopsis style), roses, tulips, lilies, cherry blossoms, daisies — each procedurally generated with realistic petal geometry, not simple cones or spheres
- **Interaction**: 
  - Click/tap on the ground to plant a flower
  - Select flower type from an elegant UI panel (glassmorphism style)
  - Flowers gently grow with smooth animation when planted (scale + rotate)
  - Flowers sway gently in a breeze (vertex shader or bone animation)
  - Camera orbits slowly; user can drag to look around, scroll to zoom
  - Particles: floating pollen/spores drifting through the scene
  - Day/night cycle toggle with smooth transition (warm sunset → starry night)
- **Visual polish**:
  - Soft shadows (PCF or contact shadows)
  - Subtle fog for depth
  3  - Bloom post-processing for glow on flowers
  - Ground: subtle terrain with grass-like particles or texture
  - Sky: gradient shader (not flat color)
- **Audio**: gentle ambient wind sound (Web Audio API generated, no external files), soft chime when planting a flower

## Technical constraints
- Single file: everything in index.html (HTML + CSS + JS inline)
- Three.js from CDN: `https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js`
- No external assets, no images, no model files — everything procedural
- Must work in modern Chrome/Safari on macOS
- Performance: should run smoothly at 60fps on M4 Mac mini

## UI/UX
- Minimal, elegant control panel (bottom-left, glassmorphism)
- Flower type selector with small icon/thumbnail of each flower
- Day/night toggle button
- "Clear garden" button
- Flower count display
- Title "Flora" in a refined serif font (Google Fonts: Cormorant Garamond)
- Subtle instructions that fade after first interaction

## Flower construction guidelines
- **Orchid**: 5 broad petals arranged in characteristic phalaenopsis shape, central lip/column, soft pink/white gradient
- **Rose**: layered spiral of curved petals, tight center, deep red or coral
- **Tulip**: cup-shaped, 6 petals, smooth curved form, vibrant colors
- **Lily**: trumpet shape, 6 elongated curved petals, stamens visible, white/orange
- **Cherry blossom**: 5 notched petals, delicate pink, small clustered
- **Daisy**: ring of flat petals, yellow center, white/colored
- Each flower on a stem with leaves, slight bend for natural look

## What to output
Write the complete index.html file. Make it beautiful. This is a portfolio-quality piece.