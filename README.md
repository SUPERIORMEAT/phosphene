# Phosphene

A music visualizer for accretion.tv. One HTML file, WebGL2 and Web Audio, no dependencies.

The song's key becomes the colour of the field, on the circle of fifths. Two FFTs run at
once: a long window for key and a 256-band log spectrum, a short window for hits. A beat
tracker locks the pulse and flips the spin every bar. Build, drop and breakdown are detected
from sixteen seconds of energy history. Nothing strobes.

**Seven modes** — Afterimage, Haze, Bloom, Lattice, Hyperspace, Aurora, Event Horizon.
**Ten dials** — depth, drift, react, bass, spiral, zoom, twist, bulge, ripple, model.
**Shapes** — the field folds onto a circle, triangle, square, pentagon, hexagon, star or flower.
**A 3D deformer** — it opens on the accretion "a", built as real geometry from the logo's own
vector measurements. The mesh is drawn off screen every frame and the field is refracted
through its surface normals and depth. Load your own `.obj` or `.stl` with **Load 3D**.
Scroll to **dolly**: the camera physically moves toward the object, so perspective opens up
as you approach. It is a dolly, not a zoom, and the focal length never changes.
**Anchor** slows everything to a warm, steady mandala with a breath pacer, for when it is too much.

## Objects

The second row under the modes is the 3D deformer. A mesh is drawn off screen every frame
into a surface-normal and depth buffer, and the field is refracted through it, so the picture
bends around a real object rather than a flat mask. Eleven are built in:

| object | what it is |
|---|---|
| Text | anything you type, rastered then domed into a rounded solid. Eight typefaces, and a slider for how soft the edges are |
| accretion a | the accretion.tv letterform, generated from the logo's own vector measurements |
| Knot | a trefoil, swept as a tube |
| Infinity | a lemniscate of Gerono, so both lobes stay round rather than pinching to points |
| Concentric | six nested rings, each tipped further over, like an armillary |
| Mobius | a Mobius strip: one surface, one edge |
| Harmonic | a spherical-harmonic surface, the standing waves of a vibrating sphere |
| Klein | the figure-eight immersion of a Klein bottle, a surface with no inside |
| Supershape | the Gielis superformula, the one equation behind many natural outlines |
| Torus | the plain case |
| Load .OBJ / .STL | your own model. Wavefront `.obj` and `.stl`, binary or ASCII |

**Drag to spin it.** Press and drag anywhere to orbit the object; it keeps turning when you
let go. **Scroll to dolly**: the camera physically moves toward it, so perspective opens up as
you approach. It is a dolly, not a zoom, and the focal length never changes.

The flat shape row above is a separate control. It folds the 2D field onto a circle, triangle,
square, pentagon, hexagon, star or flower, and works with or without an object loaded.

Feed it a song by dropping the file, the microphone, one Chrome tab, or MIDI.

Built with Claude Code.
