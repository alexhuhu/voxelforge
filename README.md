# VoxelForge

Convert 3D models (`.obj`) into Minecraft schematics (`.schem`) right in the browser. Load a model, set the resolution and block palette, preview the voxelized result on a grid, and export a Sponge v2 `.schem` that loads into WorldEdit (`//schem load`) or Litematica.

Everything runs client-side. There is no server and nothing is uploaded.

## Usage

Open `index.html` in a browser, or visit the hosted page. Then:

1. Drop an `.obj` file onto the panel (add its `.mtl` alongside for material colors).
2. Set the size, constraint axis, and block palette.
3. Click **Voxelize** to preview.
4. Click **Export .schem** to download.

## Features

- In-browser voxelization of `.obj` meshes
- Color matching to real Minecraft block colors (perceptual or RGB)
- Palettes: all blocks, schematic-friendly, colourful, concrete, wool, greyscale
- Selectable export data version (1.19.4 through 1.21.11)
- Verified Sponge Schematic v2 output

## Hosting

This is a single static file. It works on GitHub Pages, Cloudflare Pages, Netlify, or any static host with no build step.

## Credits and attribution

This project is inspired by and partially derived from
[ObjToSchematic](https://github.com/LucasDower/ObjToSchematic) by Lucas Dower,
licensed under BSD 3-Clause. The block average colors and palette lists in this
tool are derived from that project's resource files. See
[`THIRD_PARTY_LICENSES.md`](THIRD_PARTY_LICENSES.md) for the full notice.

Third-party libraries loaded at runtime via CDN: [three.js](https://threejs.org/)
and [pako](https://github.com/nodeca/pako).
