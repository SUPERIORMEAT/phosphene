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

Feed it a song by dropping the file, the microphone, one Chrome tab, or MIDI.

Built with Claude Code.
