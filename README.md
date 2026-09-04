# Cobblemon PC Icons

A client-side Fabric mod for **Minecraft 1.21.1 / Cobblemon 1.7.3** that replaces Pokémon 3D models in the Cobblemon PC storage screen with 2D icons when matching resources are available, while preserving Cobblemon's normal 3D fallback when no icon is found.

## Author / Maintainer

**mcneilcusi20-byte**

GitHub: https://github.com/mcneilcusi20-byte

The mod metadata in `fabric.mod.json` also points to this GitHub account as the author.

## Current build

- Mod: `cobblemon-pc-icons-2.0.6.4-baby-legends.jar`
- Resource pack: `E19_PC_Icons_All_Forms_Fix_v5_Baby_Legends.zip`
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

## Baby Legends 2.4 compatibility

Version **2.0.6.4** includes built-in compatibility aliases for the Baby Legends 2.4 addon. Baby Pokémon use the corresponding adult legendary icon artwork, matching the behavior used by the E19 minimap icon pack rather than introducing newly drawn baby sprites.

Supported Baby Legends species and their PC icon mappings:

| Baby Legends species | PC icon used |
| --- | --- |
| Articoo | Articuno |
| Beta | Arceus |
| Courpup (male) | Zamazenta |
| Courpup (female) | Zacian |
| Creslume | Cresselia |
| Delcalf | Kyogre |
| Foreroar | Suicune |
| Fulguroar | Raikou |
| Giragrub | Giratina |
| Haidon | Koraidon |
| Kaidon | Miraidon |
| Karfoal | Keldeo |
| Latot (male) | Latios |
| Latot (female) | Latias |
| Myu | Mew |
| Myutu | Mewtwo |
| Neonite | Necrozma |
| Ohho | Ho-Oh |
| Raygul | Rayquaza |
| Regiclay | Regigigas |
| Rotisikree | Moltres |
| Saladune | Groudon |
| Statchic | Zapdos |
| Temga | Dialga |
| Vertrice | Virizion |
| Volcaroar | Entei |
| Xerfawn | Xerneas |
| Yangram | Kyurem |
| Yivpip | Yveltal |
| Zerpint | Zygarde |
| Royal Carbink | Diancie |

Normal and shiny variants are supported. Gender-specific aliases are included for **Latot** and **Courpup**, including common full-aspect combinations used by Cobblemon so their male/female and shiny appearances resolve correctly in the PC UI.

Because **Regiclay** and **Yangram** can evolve into multiple legendary Pokémon, this compatibility pack uses a single neutral representative icon for each branching line: Regiclay uses **Regigigas**, while Yangram uses **Kyurem**.

The Royal Carbink form added by Baby Legends is mapped to **Diancie**, including its shiny variant.

The compatibility aliases are bundled directly inside the 2.0.6.4 mod JAR and are also included in the matching v5 resource pack. This means Baby Legends support is available even if only the mod's bundled aliases are used, while the resource pack remains the recommended way to provide the complete E19 icon library.

## Resource-pack attribution

The PC icon resource pack is a conversion/compatibility pack based on **E19 Cobblemon Minimap Icons** artwork and naming data. Original artwork and third-party assets remain attributable to their respective creators; this repository does not claim ownership of those upstream assets.

## Installation

Place the mod JAR in your Fabric `mods` folder and enable the ZIP in Minecraft's Resource Packs menu. Fully restart Minecraft after changing the resource pack because the mod caches icon lookups for the current game session.
