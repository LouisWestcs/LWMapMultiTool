# LW Map Multi Tool

A map-development multi-tool for Arma Reforger (Enfusion) terrains. Current version: **v3.0 "Silverlake"**.
(Earlier versions were called GalloDevelopment Tool / Fake Terrain Maker.)

Pick a map once, then use:

- **Fake Terrain**: turns a block of terrain into a mesh object (FBX with 3 LODs + a collider with the right surface
  materials), with the terrain's own textures, hole cut-outs, splitting into pieces, satmap colour and optional automatic
  import into Workbench.
- **Satmap**: export the current satmap, generate a new one from the painted surfaces, or fix tile seams in any
  satmap image.
- **Convert roads**: road lines from an Arma 3 map, road `.layer` files or GIS data (`.shp`, GeoJSON, `.osm`) turned
  into Reforger road generators.
- **Paint terrain**: repaint a terrain's surfaces in place, by rules (height, slope, shore), along roads or under trees.
- **In-game map**: set a paper map or satmap image as the world's map background.

Works with vanilla maps, mod terrains and Arma 3 map PBOs.

## Download

Get `LWMapMultiTool.exe` from the [Releases](../../releases) page. This is the only official download. Please link
here instead of re-uploading it.

Windows may show "Windows protected your PC" because the exe is not signed: click **More info -> Run anyway**.

## Requirements

- Windows 10 / 11 with the Microsoft Edge WebView2 Runtime (built into Windows 11; on Windows 10 get it from
  Microsoft if the window stays blank)
- Blender 4.2 or newer (Fake Terrain builds the mesh with it in the background; tested with 4.5)
- Arma Reforger installed (to read the vanilla terrain surfaces and textures)
- The map's terrain files on disk
- Arma Reforger Tools / Workbench, only for "Register in Workbench"

Settings and caches: `%LOCALAPPDATA%\FakeTerrainMaker`. Default output: `Documents\LW Map Multi Tool`.

## Licence

Free to use, closed source. In short (the full terms are in [LICENSE.txt](LICENSE.txt)):

- Free to use for personal and commercial projects, and you can publish what you make with it.
- **Credit required** when you publish something made with it: `Made with LW Map Multi Tool by LW`.
- **No selling** the tool, no paywalls, **no re-uploading**, and no claiming it as your own.
- **No modifying** the tool, and no decompiling or unpacking the exe.
- **Not licensed** to Narcos Roleplay or to any server owned or staffed by Discord user ID `527293059008823307`
  (see section 4 of the licence).

You need the rights to whatever maps you load into it. This is an unofficial tool, not affiliated with Bohemia
Interactive. Third-party components: [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).
