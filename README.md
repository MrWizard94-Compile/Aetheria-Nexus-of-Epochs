# Aetheria: Nexus of Epochs

> Kitchen-sink-meets-expert. Ancient magic, industrial steampunk, and quantum tech bleed into one timeline — and KubeJS scripts force them to talk to each other so no mod makes another obsolete.

**Minecraft 1.20.1 · Forge 47.x · CurseForge-format modpack**

## Overview

| Spec | Detail |
|------|--------|
| Title | Aetheria: Nexus of Epochs |
| Version | Minecraft 1.20.1 |
| Loader | Forge 47.x |
| Primary focus | Kitchen-sink with expert-style woven progression |
| Difficulty | Action-RPG combat; scaling threat |
| Pack version | 0.1.0 (foundation) |

The differentiator is the **KubeJS "secret sauce"**: early game leans on Create + Botania; mid game gates AE2 behind Alex's Caves resources + Ars Nouveau enchanting; end game gates Mekanism fusion behind Cataclysm boss drops processed in Botania-powered factories.

## Repository layout

| Path | Purpose |
|------|---------|
| `manifest/manifest.json` | CurseForge manifest (Forge 1.20.1). `files[]` resolved at packaging time. |
| `overrides/config/` | Pack configs (committed) |
| `overrides/mods/` | Local mod jars (gitignored; `.gitkeep` tracked) |
| `docs/CONCEPT.md` | Original design vision |
| `docs/MODLIST.md` | Curated, categorized mod roster + Forge 1.20.1 availability notes |

## Status

🌱 **Foundation scaffolded.** Structure, manifest, and curated roster in place. Mod `files[]` not yet resolved to CurseForge IDs — see `docs/MODLIST.md`. The KubeJS integration scripts live under `overrides/kubejs/` once authored.

## Building / CurseForge export

1. Drop mod jars into `overrides/mods/` to test in a local Forge 1.20.1 instance.
2. Resolve each mod's `projectID` / `fileID` into `manifest/manifest.json` `files[]`.
3. Zip `manifest.json` + `overrides/` per the CurseForge modpack spec; publish via the CurseForge author dashboard.

## Related

- [JanusPrime orchestration](https://github.com/MrWizard94-Compile/JanusPrime)
- Sibling concept packs: Aethelgard, Aetherial Convergence, Chronicles of the Shattered Cosmos, Omniverse Odyssey
