# GameCheats Library

Free standalone trainers and the **GameCheats Loader**, by **KeenAsGreen**.

## Download

- **[Download GameCheats Loader for Windows](https://github.com/daleeb/gamecheats-library/releases/tag/loader-v0.1.0)** — extract the entire ZIP and run `GameCheats-Loader.exe` inside the folder.
- **[Download the HOMM: Olden Era trainer](https://github.com/daleeb/gamecheats-library/releases/tag/homm-olden-era-v1.3.0)** — standalone EXE, no loader required.
- **[All releases](https://github.com/daleeb/gamecheats-library/releases)**

The loader browses this catalog, downloads trainers, checks their signature-backed
SHA-256 hashes, and launches their separate windows. It includes search,
favourites, installed status, updates, and a saved catalog for offline use.
No GitHub account or Python installation is required to use the packaged loader.

## Available trainers

| Game | Supported build | Trainer | Features |
|---|---|---|---|
| Heroes of Might and Magic: Olden Era | v0.82.08 | 1.3.0 | Resource tools, movement, mana, reveal map, army editor |

Launch the game, load a single-player save, then launch its trainer. All cheats
start disabled. The HOMM trainer refuses incompatible build fingerprints.
F1/F2 toggle resource patches, F3/F4 movement and mana, and F5 reveals the map once.
Select a hero to edit occupied troop stacks. Closing the trainer restores code
patches; changed gameplay values and revealed tiles are not automatically undone.

## Catalog

`catalog.json` is an Ed25519-signed manifest. `catalog-public-key.json` contains
the public verification key; the loader pins that key in its own resources.
Trainer binaries are attached to releases, not committed to this repository.
`definitions/` contains the associated trainer definitions.

Downloads are portable Windows x64 builds. Windows code signing is separate from
catalog signing: these initial executables do not have an Authenticode signature.

Updates and discussion: [r/GameCheats](https://www.reddit.com/r/GameCheats/).
For a bug report, include the game build, trainer version, and what happened.
