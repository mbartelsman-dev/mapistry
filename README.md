# Mapistry

Inspired by [Fractal Terrains][ft3], [Wilbur][wilbur], and [Martin O'Leary's Generating Fantasy Map Generator][mapgen], Mapistry aims to be a global and local map generation tool capable of creating realistic terrain for the globe or a region of it, while leveraging modern technologies.

## Goals

### Speed

Wilbur and Fractal Terrains are powerful tools, but they are extremely slow due to the lack of paralelization. GPU computing libraries could be leveraged to perform the most intensive calculations, such as erosion. In this regard, using the threading facilities provided by modern programming languages should already provide a noticeable improvement. And using technologies such as OpenCL for GPU computing should make the process orders of magnitude faster.

- Integration. Use of open formats that can be reused with external tools. Particularly integration with GIS.
- Scalability. Mapistry should be capable of handling maps at large and small scales while remaining mini

- [ ] World visualization  
The first step is to make a tool capable of visualizing the world

[ft3]: https://www.profantasy.com/products/ft.asp
[wilbur]: http://www.fracterra.com/wilbur.html
[mapgen]: http://mewo2.com/notes/terrain/
