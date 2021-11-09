# Enhanced Lighting for ENB Synthesis patcher

## Description

Carries over changes from [Enhanced Lighting for ENB](https://www.nexusmods.com/skyrimspecialedition/mods/1377) when reverted. Also patches some modded locations to use ELE's lighting templates & image spaces, and adjusts some modded imagespaces & lights.

### Supported mods

The number after the mod indicates the version the "mod support patch" was made for. You can safely use it for other versions too, might just not be quite right if there were cell changes or some such.

- [Beyond Skyrim - Bruma SE](https://www.nexusmods.com/skyrimspecialedition/mods/10917) (1.4.2)
- [Cutting Room Floor - SSE](https://www.nexusmods.com/skyrimspecialedition/mods/276) (3.1.9)
- [Darkend](https://www.nexusmods.com/skyrimspecialedition/mods/10423) (1.4)
- [Falskaar](https://www.nexusmods.com/skyrimspecialedition/mods/2057) (2.2)
- [Helgen Reborn](https://www.nexusmods.com/skyrimspecialedition/mods/5673) (V106.SSE)
- [Lanterns of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/2429) (any version)
- [Legacy of the Dragonborn SSE](https://www.nexusmods.com/skyrimspecialedition/mods/11802) (5.5.2, 4.1.1 support included)
- [Medieval Lanterns of Skyrim](https://www.nexusmods.com/skyrimspecialedition/mods/27622) (any version)
- [Ravengate](https://www.nexusmods.com/skyrimspecialedition/mods/12617) (0.06BTASSE)

### Details for the curious

- [Technical details](docs/Technical.md)
- [Mod support details](docs/ModSupportDetails.md)

## Installation & usage

### Note about load order

The first part of the patcher won't do much if ELE is late in your load order. The majority of people are probably only after the mod support part of the patcher so that's fine.

If, however, you wish to merge ELE's changes with another mod you use, place `ELE_SSE.esp` before the mod you'd like to merge its changes with.

For example, to merge Atlas Map Markers' Blackreach map data & ELE's Blackreach interior lighting, place `ELE_SSE.esp` before `Atlas Map Markers.esp` before running the patcher.

### Synthesis (Match or 0.20.5+ required)

If you have Synthesis, there are 2 options:
- In Synthesis, click on Git repository, and choose ELE Patcher from the list of patchers
- [Grab the exe](https://github.com/Benna96-Synthesis/ELE_patcher/releases/latest/download/ELE_Patcher.exe), then in Synthesis, click on External Program, and browse for the exe
  - Not recommended

### Standalone

The patcher does run without Synthesis as well. Just [grab the exe](https://github.com/Benna96-Synthesis/ELE_patcher/releases/latest/download/ELE_Patcher.exe) and run it. The generated plugin is called `Synthesis ELE patch.esp`.

If you're an MO2 user, as with all things, remember to run through MO2!