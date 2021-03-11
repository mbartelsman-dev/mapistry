# Mapistry

Inspired by [Fractal Terrains][ft3], [Wilbur][wilbur], and [Martin O'Leary's Generating Fantasy Map Generator][mapgen], Mapistry aims to be a global and local map generation tool capable of creating realistic terrain for the globe or a region of it, while leveraging modern technologies.

Wilbur and Fractal Terrains are powerful tools, but they are extremely slow due to the lack of paralelization. GPU computing libraries could be leveraged to perform the most intensive calculations, such as erosion. In this regard, using the threading facilities provided by modern programming languages should already provide a noticeable improvement. And using technologies such as OpenCL for GPU computing should make the process orders of magnitude faster.

[ft3]: https://www.profantasy.com/products/ft.asp
[wilbur]: http://www.fracterra.com/wilbur.html
[mapgen]: http://mewo2.com/notes/terrain/


## Requirements

### Overview

Note: World in this context is used to refer to the region of interest being mapped.

- Must haves
  - World generation: User must be able to generate a world that they can use as a starting point in the program
  - World erosion: User must be able to perform erosion operations on the current world
  - World visualization: User must be able to visualize the current state of the world
  - World loading: User must be able to load world data that's been stored in the filesystem or (potentially) online
  - World saving: User must be able to save their generated world into their filesystem or (potentially) online

- Should haves
  - Parameterized erosion: User should be able to fine-tune the erosion process to achieve desired results
  - Dynamic visualization: User should be able to pan, zoom, and rotate their world-view
  - Cultural feature generation: Users should be able to proceduraly generate a set of cities based on desirability parameters

- Could haves
  - Parameter mask: User should be able to load bitmap masks and tie them to their parameters
  - Sample visualization: User could be able to see a small rendered sample of the world prior to confirming any changes
  - Undo/Redo: User could have the option to undo or redo the last few states of the world
  - Climate generation: Users should be able to procedurally generate the climate of their world given a set of parameters

- Would haves
  - Processing world visualization: User would able to see the effects of different processess as they are generated

### World Erosion

**Resources**:
- https://github.com/dandrino/terrain-erosion-3-ways
- https://hal.inria.fr/hal-01262376/document
- https://hal.inria.fr/inria-00402079/document
