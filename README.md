# Phosphene

A music visualizer for accretion.tv. One HTML file, WebGL2 and Web Audio, no dependencies.

The song's key becomes the colour of the field, on the circle of fifths. Two FFTs run at
once: a long window for key and a 256-band log spectrum, a short window for hits. A beat
tracker locks the pulse and flips the spin every bar. Build, drop and breakdown are detected
from sixteen seconds of energy history. Nothing strobes.

**Seven modes** — Afterimage, Haze, Bloom, Lattice, Hyperspace, Aurora, Event Horizon.
**Six dials** — depth, drift, react, bass, spiral, zoom.
**Anchor** slows everything to a warm, steady mandala with a breath pacer, for when it is too much.

Feed it a song by dropping the file, the microphone, one Chrome tab, or MIDI.

Built with Claude Code.
