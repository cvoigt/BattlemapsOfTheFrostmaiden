# Battlemaps Of The Frostmaiden
Welcome to my small selection of hand-crafted battlemaps for ```Icewind Dale: Rime of the Frostmaiden```.

My goal is to workthrough the whole Adventure and provide battle maps that provide a consistent look & feel for use in any VTT platform while also providing some complementary maps that can slot in anywhere in the adventure and provide a reusable backdrop for random encounters or homebrew ideations.

> ℹ️ All chapter-related battle maps follow the original layouts from the source book although distances might be adjusted to provide a more realistic scale or account for larger engagement/party sizes.

## Folder Structure
The folder structure and naming conventions in this repository follow the order and organization of the source book ```Icewind Dale: Rime of the Frostmaiden```

```
└───Chapter 1 - Ten-Towns
    └───Targos - Mountain Climb
```

## File Formats
All battlemaps are provided in several variations:
- `*.png` for lossless high-quality suitable for printing
- `*.webp` for optimized file size for usage in Virtual Table Top (VTT) systems like Roll20, FoundryVTT or OwlBear Rodeo
- `*.dungeondraft_map` for import into Dungeondraft

# Filenames
All files follow the following naming convention:

```
bm_rotf_<chapter>_<location>_<version>_<variation>_<level or flat>_<grid>.extension bm_rotf_c1_targos_mountain-climb_v1_var1_L0_grid.png
```

Examples:
```
bm_rotf_c1_targos_mountain-climb_v1.dungeondraft_map
bm_rotf_c1_targos_mountain-climb_v1_var1_flat_grid.png
bm_rotf_c1_targos_mountain-climb_v1_var1_flat.png
bm_rotf_c1_targos_mountain-climb_v1_var1_L0_prop1.png
bm_rotf_c1_targos_mountain-climb_v1_var1_L0_prop2.png
```



## Indicators
> ℹ️ This only applies to `.png` and `.webp` exports.
>
> The original Dungeondraft source files don't have filename indicators
- `v` version of the Dungeondraft source file
- `varX` multiple variations of the same map
- `_Lx` if a map consists of multiple layers this will indicate which layer the file belongs to.
  - `L1` = Level 1
  - `L0` = Level 0 (default)
  - `L-1` = Basement Level 1
  - `L-2` = Basement Level 2
- `flat` if all layers are flattened into a single image
- `grid` contains a standard grid within the exported image
- `propx` this can be used as an optional hide/show prop in the scene. It shares dimensions with the scene itself so alignment on the main scene is easiest.

## Prerequisites
All source files ar built with **Dungeondraft** and exclusively utilize the Forgotten Adventures Asset Packs. The minimum requirements are:
- Dungeondraft 1.2.0.1 *opulent kirin*
- Required Dungeondraft Mods:
  - [ColourObjectsAndPaths 1.1.1](https://cartographyassets.com/assets/92440/colour-and-modify-things/) by *uchideshi34*
  - [Convert Object Into Pattern 1.0.3](https://cartographyassets.com/assets/87173/convert-object-to-pattern/) by *uchideshi34*
  - [Dropshadower 1.2.0](https://cartographyassets.com/assets/45436/dropshadower/) by *MBMM*
  - [EdgeBlurPattern 1.1.2](https://cartographyassets.com/assets/57470/blurred-edge-patterns/) by *uchideshi34*
  - [EssentialUtils 1.3.5](https://cartographyassets.com/assets/32902/essentialutils/) by *MBMM*
  - [Item and path opacity 1.1.2](https://cartographyassets.com/assets/42112/item-and-path-opacity/) by *cheetodust*
- Recommended Dungeondraft Mods:
  - [Additional Search Options 1.2.6](https://cartographyassets.com/assets/48648/additional-search-options/) by *uchideshi34*
  - [Layers Panel 1.0.0](https://cartographyassets.com/assets/89773/layers-panel-mod-updated/) by *uchideshi34*
  - [ScatterBrush 1.0.3](https://cartographyassets.com/assets/87314/scatter-brush/) by *uchideshi34*
  - [Universal VTT WebP Exporter 1.0.0](https://cartographyassets.com/assets/41839/universal-vtt-webp-exporter/) by *insteadofnothing*
- [Forgotten Adventures Asset Packs](https://www.forgotten-adventures.net/product/map-making/assets/dungeondraft-integration/) (*requires one-time Patreon membership at the Adventurer Level to gain access to the Dungeondraft packs on pCloud.*)
  - FA_Objects_A_v3.52
  - FA_Objects_B_v3.84
  - FA_Textures_A_v3.59
  - FA_Textures_B_v3.54