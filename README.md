# Cobblemon PC Icons

A client-side Fabric mod for **Minecraft 1.21.1 / Cobblemon 1.7.3** that replaces Pokémon 3D models in the Cobblemon PC storage screen with 2D icons when matching resources are available, while preserving Cobblemon's normal 3D fallback when no icon is found.

## Preview

![Cobblemon PC Icons v2.0.6.4 preview](Screenshot%202026-09-04%20102106.png)

## Author / Maintainer

**mcneilcusi20-byte**

GitHub: https://github.com/mcneilcusi20-byte

The mod metadata in `fabric.mod.json` also points to this GitHub account as the author.

## Current build

- Mod: [`cobblemon-pc-icons-2.0.6.4.jar`](cobblemon-pc-icons-2.0.6.4.jar)
- Resource pack: [`PC_Icons v2.0.6.4_3.zip`](PC_Icons%20v2.0.6.4_3.zip)
- Minecraft: 1.21.1
- Cobblemon: 1.7.3
- Baby Legends: 2.4 support

## Features

- 2D Pokémon icons in Cobblemon PC storage
- Hybrid fallback to Cobblemon's normal 3D model
- Form, shiny, and gender-aware icon lookup
- Cached texture lookup for better performance
- Runtime scale/position configuration
- Mega Showdown form aliases
- Zygarde runtime-form fixes
- Baby Legends 2.4 icon aliases
- Latot gender mapping: male → Latios, female → Latias
- Courpup gender mapping: male → Zamazenta, female → Zacian

## Configuration

After launching the game once with the mod installed, the mod automatically creates:

`config/cobblemon-pc-icons.properties`

Open this file with any text editor to change the PC icon size, position, fallback icon, and debug logging.

```properties
# 1.0 = normal size; range 0.10 to 3.00
scale=1.3

# Base icon size in logical PC-slot pixels
base_size=10

# Positive X = right, positive Y = down
offset_x=0
offset_y=6

# Show built-in diagnostic icon when no custom sprite exists
fallback_icon=true

# Log the exact sprite path chosen/attempted once per Pokemon variant
debug=true
```

### Quick guide

- `scale` — changes the overall icon size.
- `base_size` — changes the base rendered icon size.
- `offset_x` — moves icons left (`-`) or right (`+`).
- `offset_y` — moves icons up (`-`) or down (`+`).
- `fallback_icon` — set to `false` to hide the diagnostic fallback icon when a custom sprite is missing.
- `debug` — set to `false` to disable sprite lookup logging.

The config is checked while the game is running, so saved changes can be picked up without manually recreating the file.

## Baby Legends 2.4 compatibility

Version **2.0.6.4** includes built-in Baby Legends 2.4 icon support, including normal/shiny variants and special mappings such as **Latot male → Latios**, **Latot female → Latias**, **Courpup male → Zamazenta**, **Courpup female → Zacian**, and **Royal Carbink → Diancie**. The matching resource pack is recommended for the complete icon library.

## Resource-pack attribution

The PC icon resource pack is a conversion/compatibility pack based on **E19 Cobblemon Minimap Icons** artwork and naming data. Original artwork and third-party assets remain attributable to their respective creators; this repository does not claim ownership of those upstream assets.

## Installation

1. Download [`cobblemon-pc-icons-2.0.6.4.jar`](cobblemon-pc-icons-2.0.6.4.jar) and place it in your Fabric `mods` folder.
2. Download [`PC_Icons v2.0.6.4_3.zip`](PC_Icons%20v2.0.6.4_3.zip) and enable it in Minecraft's Resource Packs menu.
3. Fully restart Minecraft after changing the resource pack because the mod caches icon lookups for the current game session.
