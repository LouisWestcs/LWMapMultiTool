# LW Map Multi Tool

A map-development multi-tool for Arma Reforger (Enfusion) terrains, formerly **GalloDevelopment Tool**.
Pick a map once, then use:

- **Fake Terrain**: turns a block of terrain into a mesh object (FBX with 3 LODs + a collider with the right surface
  materials), with the terrain's own textures, cut-outs, splitting into pieces, satmap colour and optional automatic
  import into Workbench.
- **Satmap**: export the current satmap, generate a new one from the painted surfaces, or fix tile seams in any
  satmap image.
- **Terrain**: copy a map (or an area of it, resized / resampled) into a new world + `.terr` in your mod, including
  its roads, buildings, trees and other objects. It can also make an import kit (heightmap, masks, satmap).
  Works with vanilla maps, mod terrains and Arma 3 map PBOs.

## Download

Get the latest `.exe` from the [Releases](../../releases) page. This is the only official download. Please link
here instead of re-uploading it.

Windows may show "Windows protected your PC" because the exe is not signed: click **More info -> Run anyway**.

## Requirements

- Windows 10 / 11
- Blender 4.2 or newer (Fake Terrain builds the mesh with it in the background; tested with 4.5)
- Arma Reforger installed (to read the vanilla terrain surfaces and textures)
- The map's terrain files on disk
- Arma Reforger Tools / Workbench, only for "Register in Workbench"

Settings and caches: `%LOCALAPPDATA%\FakeTerrainMaker`. Default output: `Documents\GalloDevelopmentTool`.

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
