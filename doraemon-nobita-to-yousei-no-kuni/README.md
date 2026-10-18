# Doraemon: Nobita and the Land of Fairies

**English translation — Version 1.0**

An English localization of *Doraemon - Nobita to Yousei no Kuni*, a Japanese Super Famicom / Super Nintendo family adventure from 1993. Join Doraemon and his friends on a journey to help the fairies and rescue their imprisoned queen.

## Translation features

- English dialogue, scrolling introduction, item descriptions and menu text.
- Storybook Balanced font, refined for readability at the original resolution.
- English Doraemon title logo, subtitle and romanized copyright names.
- Faster normal dialogue reveal; scripted pauses and event commands are preserved.
- Latin password symbols that preserve the game's original numeric password values.

Original Japanese character names are retained: Doraemon, Nobita, Shizuka, Gian and Suneo. The title keeps the original yellow/purple PUSH START and blue/purple copyright colours. The original Game Over prompt alignment is also retained.

## Required original Japanese ROM

Apply the patch to the **unmodified, unheadered Japanese revision 0 ROM** below.

| Property | Required value |
| --- | --- |
| Original filename | `Doraemon - Nobita to Yousei no Kuni (Japan).sfc` |
| Region / language | Japan / Japanese |
| Revision | 0 |
| Size | 524,288 bytes (512 KiB) |
| Copier header | None |
| CRC32 | `51BC2909` |
| SHA-1 | `11cd5e49b6907b6fa6f524ec7b216805712eeaf6` |
| SHA-256 | `6501d12f6615cdff9622d56445156789b156333579ff6e94492449605b48b8db` |

The filename is a reference; the file's contents and hashes determine compatibility. A headered ROM, another revision or a previously patched ROM will not match. Keep your original ROM unchanged.

## Applying the BPS patch

1. Make a backup of your original Japanese ROM and verify its size and hash against the table above.
2. Open a ROM patcher that supports **BPS**. Select `Doraemon - Nobita and the Land of Fairies (English) v1.0.bps` as the patch and the untouched Japanese ROM as the source.
3. Save the result as `Doraemon - Nobita and the Land of Fairies (English) v1.0.sfc`, using a separate output file.
4. Verify the output against the table below, then open it in your SNES emulator or use it with your compatible SNES flash cartridge.

Apply the BPS directly to the original Japanese ROM. Do not apply the Torvus IPS first, patch an older English build, or disable source-checksum validation. If the patcher reports a source mismatch, recheck the source ROM's revision, header and hashes.

The local project folder includes the already-patched SFC for the project owner's use. It does not need patching again. When sharing this translation, distribute the **BPS and documentation**, without a ROM.

## Expected English ROM

| Property | Value |
| --- | --- |
| Filename | `Doraemon - Nobita and the Land of Fairies (English) v1.0.sfc` |
| Size | 1,048,576 bytes (1 MiB) |
| CRC32 | `4B9E953F` |
| SHA-256 | `1e67a2a39ab10dc86bb9d3ef0c76587cac9e7878a45a1a13ca25f519dc211c19` |

Patch SHA-256: `f371252c5dea5f44c5f29964c9e15b237c0074e4164124f26331840cda9fae39`.

`SHA256SUMS.txt` contains checksums for the ROM, patch, this README and the five screenshots. `release-manifest.json` records the source requirements and screenshot provenance.

## Playing and progress

The game uses a password system for continuing progress. Record your password carefully and enter it through **Password** on the title menu. This translation displays password values using Latin letters and symbols; Japanese password characters cannot be copied directly without the corresponding symbol mapping.

The Options menu includes difficulty, automatic/manual gadget use, sound and button assignments. Emulator or flash-cartridge save states are separate from the game's password system and depend on the device/software being used.

## Screenshots

These are actual emulator captures from the exact ROM identified above, at native 256 × 224 resolution:

- `01-title.png` — English title screen.
- `02-nobita.png` — Gian calls to Nobita.
- `03-the-fairy.png` — The fairy asks the group for help.
- `04-doraemon.png` — Doraemon plans the rescue.
- `05-town-dialogue.png` — Town earthquake dialogue with Doraemon's portrait.

## Testing and release notes

The project owner reported completing the game on a real Super Nintendo with no issues before the later title-logo revisions. The final title revision has emulator checks covering the logo, caption colours and Options rendering. The five supplied screenshots use the final ROM. BPS reconstruction, source hashes and output checksums have been verified. A separate full hardware playthrough of the final title revision has not been reported.

Version **1.0** is the final release label requested on 18 October 2026. Its ROM bytes are unchanged from the previously approved v1.4 / internal v0.17 build. The cancelled Game Over centering change is excluded.

The Torvus English IPS was used as a technical reference, not as the translation authority. This patch applies independently to the original Japanese ROM. Doraemon and the original game belong to their respective rights holders; this is an unofficial fan translation.
