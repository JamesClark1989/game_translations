# Doraemon 3: Nobita's Town SOS! — English v1.0

An unofficial English translation of **Doraemon 3: Nobita no Machi SOS!** for the **Nintendo 64**.

## About the game

Join Doraemon, Nobita and their friends in a 3D adventure filled with strange towns, forests, lakes and towers. Talk to the people you meet, collect clues and items, and use Doraemon's gadgets to solve problems and move the story forward. There are also minigames alongside the main adventure.

The original game is in Japanese. This release translates dialogue, menus, item descriptions, hints and many graphics into English, including the title screen. The original game's artwork and gameplay are retained wherever possible.

## Ready to play?

If you already have **Doraemon 3 - Nobita's Town SOS! (English) v1.0.z64**, it is already patched. Open that file in your Nintendo 64 emulator. You do not need to apply the patch again.

In this project folder, run **launch_game.sh** to start it in Mupen64Plus at 4× window size. That launcher also uses the project's save folder and game identification data.

## How to apply the patch

You need two files:

- Your untouched Japanese game ROM: **Doraemon 3 - Nobita no Machi SOS! (Japan).z64**.
- **Doraemon 3 - Nobita's Town SOS! (English) v1.0.bps**, the English patch.

The patch is a set of changes, so it cannot be played by itself.

1. Open [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) in your browser.
2. Beside **ROM file**, choose your original Japanese `.z64` file.
3. Beside **Patch file**, choose the English v1.0 `.bps` file.
4. Click **Apply patch** and save the new game file.
5. Open the new `.z64` file in your Nintendo 64 emulator. Keep the Japanese original as a backup.

If the patcher says the ROM does not match, check that you chose the original Japanese game, not an already translated copy. This patch expects the `.z64` version listed below. Renaming a `.n64` or `.v64` file to `.z64` does not convert it. Do not bypass a mismatch warning.

## Saves

This v1.0 release has the same game data as the final pre-release build. Existing saves in this project keep their original identity and remain usable through the supplied launcher. They do not need to be renamed to match the new release filename.

For future project updates, **update_save_states.sh** carries states forward only along supported conversion paths and keeps backups. It does not convert arbitrary saves from other emulators. Keep your normal in-game saves too.

## What has been checked?

The patch has been applied to the exact original and verified to reproduce the released English ROM byte for byte. The Nintendo 64 checksum also passes.

Translation coverage is estimated at **98%**, with a **95–99% uncertainty range**. Identified content includes 1,826 text records and 79 native graphics replacements. These counts are not proof that every scene has been seen in play. Testing has been limited; some wording or display issues may remain. A few tiny paper and book inscriptions were deliberately left unchanged.

Existing review screenshots come from earlier builds and are labelled accordingly. Open **launch_review.sh** to view the local review page; it does not need a web server.

## File information

The long codes below are file fingerprints. You do not need to type them to play. They help confirm that your original ROM and the released files are the correct copies. CRC32 here means the checksum of the entire file, not the two checksum values inside an N64 ROM header.

Original format: **Japanese release, revision 0, big-endian .z64**. The English ROM is larger because the translation uses extra storage.

### Original Japanese ROM

- Filename: `Doraemon 3 - Nobita no Machi SOS! (Japan).z64`
- Size: **16,777,216 bytes**
- CRC32: `D3B68BE4`
- SHA-1: `dd9ba0f6cfc10c3b78401cc55d06ad534f39d5b1`
- SHA-256: `410f99bdd58795639da272c9be9d1ab8c35b61f24f7c1fb92f7e83e1069a2602`

### English v1.0 ROM

- Filename: `Doraemon 3 - Nobita's Town SOS! (English) v1.0.z64`
- Size: **33,554,432 bytes**
- CRC32: `6EA0BD99`
- SHA-1: `8097f3d3c8fafc4fa39a29b04c10090474191c61`
- SHA-256: `c78c28408491a94c6764cf7bf31827efa7f1d87a0fcfa7729e1907d8f0d2052a`

### English v1.0 patch

- Filename: `Doraemon 3 - Nobita's Town SOS! (English) v1.0.bps`
- Size: **9,561,228 bytes**
- CRC32: `2144DF1C`
- SHA-1: `3a06762d9705d7461e407034dbfdf84a3913bdf5`
- SHA-256: `97536788ea98fc7e5680995c0df544a6da1cdc2ea3c621156862a7134c016cef`

## Credits and support

Doraemon and the original game belong to their respective creators and rights holders. This is an unofficial fan translation, not an official English release.

Patching instructions use [Rom Patcher JS by Marc Robledo](https://github.com/marcrobledo/RomPatcher.js/), which supports BPS patches.

If you find an issue, note the location, character and exact text. Include the version number and, if available, a screenshot or save state near the problem. This helps distinguish translation issues from emulator display problems.
