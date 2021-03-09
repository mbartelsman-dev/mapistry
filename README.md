# Mapistry

Inspired by [Fractal Terrains][ft3], [Wilbur][wilbur], and [Martin O'Leary's Generating Fantasy Map Generator][mapgen], Mapistry aims to be a global and local map generation tool capable of creating realistic terrain for the globe or a region of it, while leveraging modern technologies.

Wilbur and Fractal Terrains are powerful tools, but they are extremely slow due to the lack of paralelization. GPU computing libraries could be leveraged to perform the most intensive calculations, such as erosion. In this regard, using the threading facilities provided by modern programming languages should already provide a noticeable improvement. And using technologies such as OpenCL for GPU computing should make the process orders of magnitude faster.

[ft3]: https://www.profantasy.com/products/ft.asp
[wilbur]: http://www.fracterra.com/wilbur.html
[mapgen]: http://mewo2.com/notes/terrain/


## Requirements

### Overview

- Must haves
  - World loading
  - World saving
  - World erosion

- Should haves
  - Live world visualization

- Could haves
  - Processing world visualization

- Would haves

### World Erosion

**Resources**:
- https://github.com/dandrino/terrain-erosion-3-ways
- https://hal.inria.fr/hal-01262376/document
- https://hal.inria.fr/inria-00402079/document
