# Agent guide: Team Aqua's Asset Repo (Kanto City's fork)

This repository is a **library** of free Gen 3 decomp assets: tilesets, sprites, music, UI and more.
It's kept here as a source for the **Kanto City** ROM hack (the `Kanto-City` repository, whose
`KANTO_CITY.md` explains the project). Nothing here is built or run.

- **Don't browse or search this repository's folders.** There are around 16,000 files. Read
  [`CATALOGUE.md`](CATALOGUE.md) instead. It has one row per pack, and one per tileset with its
  format. Open a folder only when you're choosing an asset from it.
- ⭐ in the catalogue marks assets Kanto City uses. They're listed in `tools/kanto_city_usage.json`.
  When Kanto City starts using another asset, add it there.
- After adding or changing assets, regenerate the catalogue with `python3 tools/build_catalogue.py`.
  `--check` reports whether it's stale.
- **Using a tileset in Kanto City:**
  - Kanto City's metatiles are **triple-layer**. Convert a dual-layer tileset with Kanto-City's
    `dev_scripts/kanto_city/convert_metatiles_to_triple_layer.py`.
  - An Emerald-format tileset can only go on a layout marked `"include_in_firered": true`, and it
    can't share a map connection with FRLG-format maps. See "Tilesets" in `KANTO_CITY.md`.
- **Credits:** every pack's README names who to credit. Carry the credits over to `KANTO_CITY.md`
  when an asset is used.
