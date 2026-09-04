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

## Resource-pack attribution

The PC icon resource pack is a conversion/compatibility pack based on **E19 Cobblemon Minimap Icons** artwork and naming data. Original artwork and third-party assets remain attributable to their respective creators; this repository does not claim ownership of those upstream assets.

## Installation

Place the mod JAR in your Fabric `mods` folder and enable the ZIP in Minecraft's Resource Packs menu. Fully restart Minecraft after changing the resource pack because the mod caches icon lookups for the current game session.
