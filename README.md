# LW Map Multi Tool

A map-development multi-tool for Arma Reforger (Enfusion) terrains. Current version: **v3.0 "Silverlake"**.
(Earlier versions were called GalloDevelopment Tool / Fake Terrain Maker.)

Pick a map once, then use:

- **Real world**: put a box anywhere on Earth on a world map, pick a scale (1:1 up to 1:100) and make a new Reforger
  world from the real heights (free Copernicus elevation data, up to 20 km, with a live relief preview).
- **Fake Terrain**: turns a block of terrain into a mesh object (FBX with 3 LODs + a collider with the right surface
  materials), with the terrain's own textures, hole cut-outs, tunnel cut-outs (pick which of your placed prefabs are
  tunnels), splitting into pieces, satmap colour and optional automatic import into Workbench.
- **Satmap**: export the current satmap, generate a new one from the painted surfaces, or fix tile seams in any
  satmap image.
- **Convert roads**: road `.layer` files or GIS data (`.shp`, GeoJSON, `.osm`) turned into Reforger road generators.
- **Paint terrain**: repaint a terrain's surfaces in place, by rules (height, slope, shore), along roads or under trees.
- **In-game map**: set a paper map or satmap image as the world's map background.

Works with the terrain (`.terr`) of your own mod. Real world needs no map at all.

## Download

Get `LWMapMultiTool.exe` from the [Releases](../../releases) page. This is the only official download. Please link
here instead of re-uploading it.

Windows may show "Windows protected your PC" because the exe is not signed: click **More info -> Run anyway**.

## Requirements

- Windows 10 / 11 with the Microsoft Edge WebView2 Runtime (built into Windows 11; on Windows 10 get it from
  Microsoft if the window stays blank)
- Blender 4.2 or newer (Fake Terrain builds the mesh with it in the background; tested with 4.5)
- Arma Reforger installed (to read the vanilla terrain surfaces and textures)
- The map's terrain files on disk (not needed for Real world)
- An internet connection for Real world (it downloads the elevation tiles it needs and keeps them cached)
- Arma Reforger Tools / Workbench, only for "Register in Workbench"

Settings and caches: `%LOCALAPPDATA%\FakeTerrainMaker`. Default output: `Documents\LW Map Multi Tool`.

## Updates

The tool keeps itself up to date. Every time it starts, it checks this repository; if there is a newer release, it
downloads and installs it automatically and restarts. This can't be turned off. Updates are signed, so only releases
from the author are ever installed. Without an internet connection, the tool simply runs the version you have.
The check only contacts GitHub, and nothing about you or your projects is sent (see section 12 of the licence).

## Licence

Free to use, credit required, closed source. In short (the full terms are in [LICENSE.txt](LICENSE.txt)):

You need the rights to whatever maps you load into it. This is an unofficial tool, not affiliated with Bohemia
Interactive. Third-party components: [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

## Data credits

Real world uses these open datasets (downloaded when you use it, never shipped inside the exe). Every world it makes
gets a `CREDITS.txt` with the Copernicus line - please keep it with the world.

- Elevation: Produced using Copernicus WorldDEM-30 © DLR e.V. 2010-2014 and © Airbus Defence and Space GmbH 2014-2018
  provided under COPERNICUS by the European Union and ESA; all rights reserved.
- World map outlines: [Natural Earth](https://www.naturalearthdata.com/), public domain.
