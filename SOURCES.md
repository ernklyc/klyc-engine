# Engine components (x64-sikarugir10.0_6-r19)

Copies of the files KLYC-Box's engine is assembled from, byte for byte as published upstream (their sha256 is in the manifest and is checked before the app uses them).

| Component | File | License | Upstream | Size |
|---|---|---|---|---|
| wine | `WS12WineSikarugir10.0_6.tar.xz` | LGPL-2.1+ | https://github.com/Sikarugir-App/Engines/releases/download/v1.0/WS12WineSikarugir10.0_6.tar.xz | 158 MB |
| dxmt | `dxmt-highball-20260930T161516Z-a444716.tar.gz` | MIT (KLYC-Box branch of DXMT: SwapDeviceContextState, cross-process opt-in) | https://github.com/gauthierpiarrette/highball-engine/releases/download/dxmt-highball-20260930T161516Z-a444716/dxmt-highball-20260930T161516Z-a444716.tar.gz | 18 MB |
| d3dmetal-tsshim | `d3dmetal-tsshim-20260915.tar.xz` | MIT | https://github.com/gauthierpiarrette/highball-engine/releases/download/d3dmetal-tsshim-20260915/d3dmetal-tsshim-20260915.tar.xz | 0 MB |
| winetricks | `winetricks` | LGPL-2.1 | https://raw.githubusercontent.com/Winetricks/winetricks/5a59ea07513b24093bd90fad943ecf9543cf05bc/src/winetricks | 0 MB |
| moltenvk | `moltenvk-1.4.1-shadow-import-1-x86_64.tar.gz` | Apache-2.0 | https://github.com/gauthierpiarrette/highball/releases/download/engine-components/moltenvk-1.4.1-shadow-import-1-x86_64.tar.gz | 1 MB |
| d9vk-modern | `d9vk-dxvk-macos-3.1-20260916.tar.xz` | zlib | https://github.com/gauthierpiarrette/highball-engine/releases/download/d9vk-dxvk-macos-3.1-20260916/d9vk-dxvk-macos-3.1-20260916.tar.xz | 9 MB |
| winemac | `winemac-focus-20260930.tar.xz` | LGPL-2.1+ (Wine; the change in source form is spike/patches/winemac-sikarugir10.0-focus.patch) | https://github.com/gauthierpiarrette/highball-engine/releases/download/winemac-focus-20260930/winemac-focus-20260930.tar.xz | 0 MB |
| wineserver | `wine10-msync-20261001.tar.xz` | LGPL-2.1+ (Wine; the same change in source form, for the CrossOver tree, is klyc-engine's patches/0014-msync-unregister-early-return.patch) | https://github.com/gauthierpiarrette/highball-engine/releases/download/wine10-msync-20261001/wine10-msync-20261001.tar.xz | 0 MB |
| audiobuf | `audiobuf-20261001.tar.xz` | MIT (KLYC-Box's own, source spike/audiobuf/audiobuf.c) | https://github.com/gauthierpiarrette/highball-engine/releases/download/audiobuf-20261001/audiobuf-20261001.tar.xz | 0 MB |

Not included: `Template-1.0.11.tar.xz` (runtime). It contains Apple's Game Porting Toolkit / D3DMetal, whose license does not allow us to redistribute it; KLYC-Box downloads it from https://github.com/Sikarugir-App/Wrapper/releases/download/v1.0/Template-1.0.11.tar.xz.

Wine, DXVK, DXMT, MoltenVK and the others are free software; their source code is available from the projects linked in the README, and the patches and build scripts KLYC-Box's engine carries are in `source/` of this repository. Apple's D3DMetal is not part of this release.
