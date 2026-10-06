# KLYC-Box engine components

Copies of the files [KLYC-Box](https://github.com/ernklyc/klyc-box)'s Windows engine is assembled from, so the app does not depend on anyone else's download servers. Each file is exactly what was published upstream: the app checks its SHA-256 (listed in `mirror-manifest.json`) before using it.

**Where the files are:** the [Releases](https://github.com/ernklyc/klyc-engine/releases) of this repository. **What each one is, and under which license:** [SOURCES.md](SOURCES.md).

## Source code

These are free-software binaries (Wine, DXVK, DXMT, MoltenVK and friends). Their sources are at the projects:

- Wine: https://gitlab.winehq.org/wine/wine (Sikarugir's builds: https://github.com/Sikarugir-App/Engines)
- DXMT: https://github.com/3Shain/dxmt, DXVK: https://github.com/doitsujin/dxvk, MoltenVK: https://github.com/KhronosGroup/MoltenVK
- Winetricks: https://github.com/Winetricks/winetricks

The changes KLYC-Box's engine adds to them, and the scripts that build them, are in [`source/`](source): `source/patches` and `source/build-scripts`. Originally written for the [Highball](https://github.com/gauthierpiarrette/highball) project, by Gauthier Piarrette and its contributors, whose work this is built on.

## What is not here

Apple's Game Porting Toolkit / D3DMetal. Its license does not allow redistribution, so it is not in these releases; KLYC-Box asks you to accept Apple's license and downloads it from where it is already published.

## License

Each file keeps the license of its project (see SOURCES.md); the license texts are in [`licenses/`](licenses):

| Text | Applies to |
|---|---|
| [LGPL-2.1](licenses/LGPL-2.1.txt) | Wine (and Sikarugir's Wine builds), the Wine patches, Winetricks |
| [MIT](licenses/MIT-DXMT.txt) | DXMT (and KLYC-Box's own small components: the D3DMetal timestamp shim, the audio buffer fix) |
| [zlib](licenses/zlib-DXVK.txt) | DXVK (Direct3D 9) |
| [Apache-2.0](licenses/Apache-2.0.txt) | MoltenVK (with the patches in `source/patches`) |

This repository is free and non-commercial.
