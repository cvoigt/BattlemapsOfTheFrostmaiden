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
bm_rotf_<chapter>_<location>_<version>_<variation>_<dimension>_<PPI>_<level or flat>_<grid>_<lights>_<noprops>_<propx>.extension
```

Examples:
```
bm_rotf_c1_targos_mountain-climb_v1.dungeondraft_map
bm_rotf_c1_targos_mountain-climb_v1_30x30_100ppi_flat.png
bm_rotf_c1_targos_mountain-climb_v1_30x30_100ppi_flat_grid_lights.png
bm_rotf_c1_targos_mountain-climb_v1_var1_30x30_100ppi_L0_prop1.png
bm_rotf_c1_targos_mountain-climb_v1_var1_30x30_100ppi_L0_prop2.png
```

## Indicators
> ℹ️ This only applies to `.png` and `.webp` exports.
>
> The original Dungeondraft source files don't have filename indicators
- `v` version of the Dungeondraft source file
- `varX` multiple variations of the same map
- `dimensions` tile dimensions, e.g.: `30x30`
- `PPI` grid PPI, e.g.: `100ppi`
- `Lx` if a map consists of multiple layers this will indicate which layer the file belongs to.
  - `L1` = Level 1
  - `L0` = Level 0 (default)
  - `L-1` = Basement Level 1
  - `L-2` = Basement Level 2
- `flat` if all layers are flattened into a single image
- `grid` contains a standard grid within the exported image
- `lights` contains the lighting baked into the export
- `noprops` no optional props are on the scene
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

# Dungeondraft Configuration 
## New Map Settings
- Width & Height: *depending on the source book recommendation* or `30x30` tiles
- 💎 Edit Asset Pack Selection -> Disable Default Assets **`ON`**
- [x] Disable Building Wear
- [x] Disable Wall Shadow
- [x] Disable Object Shadow

> ℹ️ Common sizes for maps include:
> - 20×20 small encounter map / single room
> - 25×25 compact dungeon section
> - 30×30 common size that fits most uses
> - 40×30 medium-large tactical encounters
> - 50×50 large dungeon level or outdoor areas

## Map Settgins - Grid Style
For baked in grids in exports the `Narrow Line` provides the best compromise between visibility and artefacting when compressed.

| Dark Backgrounds | Light Backgrounds |
|----------|----------|
| Grid Style: `Narrow Line` | Grid Style: `Narrow Line` |
| Grid Color: `7fcccccc`  | Grid Color: `7f333333` |
| ![grid style dark background](/supporting%20files/asset%20samples/grid%20style%20dark%20background%207fcccccc.png) | ![grid style light background](/supporting%20files/asset%20samples/grid%20style%20light%20background%207f333333.png) |


## Levels
The name of Levels in Dungeondraft should reflect the naming for the Levels in [Indicators](/README.md#indicators)

## Layers
> ⚠️ Do not add roofs or overhangs that creatures/objects could hide under to a layer on the same *Level*.
> 
> 👍🏼 Always create a **new Level** for Roofs.

## Export Options
### **Export Mode:** `PNG`
- Grid: `ON` ⚙️ (*depending on `<grid>` indicator*)
- Lighting `OFF` ⚙️ (*depending on `<light>` indicator*)
- Brightness & Focus `100%`
- Camera Filter: `None`
- Grid Presets: `Commercial Print` (Grid PPI `300 Pixels`)

### **Export Mode:** `Universal VTT (WebP)`
- Quality: `90%`
- Grid: `ON` ⚙️ (*depending on `<grid>` indicator*)
- Lighting `OFF` ⚙️ (*depending on `<light>` indicator*)
- Brightness & Focus `100%`
- Camera Filter: `None`
- Grid Presets: `Custom` (Grid PPI `100 Pixels`)


# Art Direction
## Lights
Physical representation of lights (torches, campfires, lamps etc) should be displayed in an "off" state to allow VTTs to supplement the effects.

The `<light>` indicator can be used in exports to explicitly bake lights and lighting effects into the resulting image.

## Terrain Brushes
For a unified artstyle the following Terrain Brushes
### Ocean / Sea / Lakes
> ⚠️ The **Water Brush** should be avoided as it breaks the goal of a unified, realistic artstyle

![FA_Textures_A - Arctic Ocean A1](supporting%20files/asset%20samples/FA_Textures_A%20-%20Arctic%20Ocean%20A1.png)

`FA_Textures_A - Arctic Ocean A1`

![FA_Textures_A - Arctic Ocean A2](supporting%20files/asset%20samples/FA_Textures_A%20-%20Arctic%20Ocean%20A2.png)

`FA_Textures_A - Arctic Ocean A2`

![FA_Textures_A - Arctic Ocean B1](supporting%20files/asset%20samples/FA_Textures_A%20-%20Arctic%20Ocean%20B1.png)

`FA_Textures_A - Arctic Ocean B1`