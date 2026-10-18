# Doraemon 3 — Nobita and the Jewels of Time

## English translation v1.0

An unofficial English localization of **Doraemon 3: Nobita to Toki no Hougyoku** (ドラえもん3 のび太と時の宝玉) for the Super Famicom / SNES.

Join Doraemon, Nobita and their friends in a time-travel adventure combining side-scrolling action, exploration, gadgets, shops and passwords. Visit places including prehistoric villages, Western towns and the future, using Doraemon's gadgets along the way.

The original game was developed by **AIM**, published by **EPOCH**, and released in Japan on **16 December 1994**. Historical release details: [GameFAQs](https://gamefaqs.gamespot.com/snes/565224-doraemon-3-nobita-to-toki-no-hougyoku/data), [SuperFamicom.org](https://superfamicom.org/info/doraemon-3-nobita-to-toki-no-hougyoku). The English subtitle above is this project's localization title.

## Required original ROM

Apply the patch to a clean, **unheadered Japanese ROM**, revision **00**.

| Property | Required value |
| --- | --- |
| Original filename | `Doraemon 3 - Nobita to Toki no Hougyoku (Japan).sfc` |
| Size | **1,572,864 bytes** — 1.5 MiB / `0x180000` |
| Copier header | **None** — 0 bytes |
| Mapping | FastROM HiROM, mapping byte `31` |
| Internal revision | `00` |
| CRC32 | `560C5EAB` |
| SHA-1 | `34680c83d64bbff58aaab4b6d7029aef8a1cd558` |
| SHA-256 | `1fd2c69c6e0598ea288a32a7a5f7571e074c653a60cea75d99d8834baf9c7339` |

The filename is a reference; **the file's checksums determine compatibility**. Renaming a different ROM will not make it compatible. A ROM with a 512-byte copier header will have a different size and checksum.

## Patch instructions

1. Keep your original Japanese ROM unchanged and work from a copy.
2. Extract the ROM and patch from any ZIP archives.
3. Verify that the original ROM matches the size and checksums above.
4. Open a BPS-compatible patcher, such as [Floating IPS / Flips](https://github.com/Sir-Walrus/Flips).
5. Choose **Apply Patch** and select:
   `Doraemon 3 - Nobita and the Jewels of Time (English v1.0).bps`
6. When asked for the source file, select the clean Japanese ROM.
7. Save the output as:
   `Doraemon 3 - Nobita and the Jewels of Time (English v1.0).sfc`
8. Verify the output against the checksums below, then open it in your SNES emulator.

Apply this patch **once, to the original Japanese ROM**. Do not apply it over another English build or another patch. If the patcher reports a source mismatch, check the source ROM rather than forcing the patch.

For the complete project workspace, `launch_game.sh` opens the identical current ROM in `LATEST_BUILD` with the project's existing Mednafen settings and stable save filenames. The English-named file in this directory has identical ROM bytes.

## Patched ROM checksums

| Property | English v1.0 |
| --- | --- |
| Filename | `Doraemon 3 - Nobita and the Jewels of Time (English v1.0).sfc` |
| Size | **1,572,864 bytes** |
| CRC32 | `AB5CA36D` |
| SHA-1 | `1ba9d82d744a5185410787768bbca122058fa7d0` |
| SHA-256 | `3bed8019457c26c235457b8116e39105250929729ece4a6014357fddb331c144` |

**BPS SHA-256:**

```text
6bd073c3559e656dd5a25cca26be1b173c566518fb671c4352f514250786d27a
```

The BPS has been applied to the verified original ROM and checked to reproduce the final English ROM **byte for byte**. The ROM retains its original size and mapping.

## Translation features

- Natural English dialogue using Doraemon, Nobita, Shizuka, Gian, Suneo and Dorami's names.
- English menus, item descriptions, destination labels and passwords.
- Translated title artwork, credits, identified scenery lettering and interface graphics.
- The approved Storybook Balanced dialogue font and English Doraemon logo.
- Adjusted dialogue reveal speed, retaining native scripted waits and pauses.
- Menu layout, selection-box and shop-layering fixes, including the travel menu's expanded English labels.

Passwords use a **case-sensitive English alphabet**, including upper- and lowercase letters, digits, `+` and `-`. Copy them exactly. The underlying native password values and checksum logic are retained.

## Included files

| File | Contents |
| --- | --- |
| `Doraemon 3 - Nobita and the Jewels of Time (English v1.0).bps` | Translation patch |
| `Doraemon 3 - Nobita and the Jewels of Time (English v1.0).sfc` | Requested private local patched ROM |
| `title-screen.png` | Fresh translated title-screen capture |
| `in-game-01.png` through `in-game-04.png` | Four fresh captures of translated opening dialogue |
| `RELEASE.json` | Release version, filenames, hashes and screenshot provenance |
| `metadata.json` | Detailed engineering build and validation record |
| `README.md` | This guide |

All five images are actual Mednafen screenshots from this exact ROM, captured during normal startup and the opening. They are not reconstructions or edited mockups.

## Testing and known limitations

Version **1.0** packages engineering **build 57**. Source-hash, checksum, BPS roundtrip, text insertion, menu geometry and review-editor checks pass. Bounded emulator checks include travel-menu selection and destination loading with two-, three- and four-destination test profiles.

All **764 currently identified original dialogue pages** have English translations. The whole-game text/graphics census remains provisional; this is not a claim that every possible event has been seen in a complete manual playthrough.

Back up your progress before changing builds. Emulator save states may depend on the exact build and emulator; native passwords are useful for carrying progress without relying on a save state. The project's existing local Mednafen slots were preserved and updated for this build where necessary. That work does not establish compatibility for arbitrary external states.

FXPAK Pro save-state instability was reported during this project. Its cause remains unresolved, and v1.0 does not claim to fix it. Full-game completion and SNES/FXPAK Pro hardware compatibility have not been certified.

## Sharing

Share the **BPS patch and documentation**, not the ROM or save states. The patched ROM here is the private local copy requested for this workspace. Original game and character credits remain with their respective creators and rights holders.
