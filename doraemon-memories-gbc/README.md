# Doraemon Memories — English v1.0

## About the game

**Doraemon Memories: Nobita no Omoide Daibouken** is a Japanese Game Boy Color action-platforming game. Join Doraemon and his friends on an adventure through Nobita’s memories. Choose from Doraemon, Nobita, Shizuka, Suneo and Gian, tackle stages, collect dorayaki, and explore the Memory Album’s illustrations and stories.

This unofficial English translation covers the inventoried dialogue, menus, title and startup text, credits, and Japanese lettering found in the reviewed artwork. The original characters, illustrations and visual style are retained wherever possible.

## Files

- **English game:** `Doraemon Memories - English v1.0.gbc`
- **English patch:** `Doraemon Memories - English v1.0.ips`
- **Required original game:** `Doraemon Memories - Nobita no Omoide Daibouken (Japan).gbc`

If you already have the English `.gbc` file supplied with this release, it is ready to play. **Do not apply the patch to it again.** Open it in a Game Boy Color emulator, or use `launch_game.sh` from the project folder to play in Mednafen at 4× size.

## How to apply the patch

You need your own unmodified Japanese game file and the English `.ips` patch. Extract them first if they are inside a ZIP file. Keep a spare copy of the original game.

1. Open [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) in your browser.
2. Next to **ROM file**, choose `Doraemon Memories - Nobita no Omoide Daibouken (Japan).gbc`.
3. Next to **Patch file**, choose `Doraemon Memories - English v1.0.ips`.
4. Click **Apply patch** and save the new game file.
5. Rename the new file to `Doraemon Memories - English v1.0.gbc` if needed, then open it in your Game Boy Color emulator.

Use the original Japanese game each time you apply this patch. Renaming a different game file will not make it compatible. The file checks below let you confirm you have the right version. Rom Patcher JS can show the original file’s CRC32: it should be **D187CEC4**. The patcher’s [official project page](https://github.com/marcrobledo/RomPatcher.js/) documents its supported patch formats.

## File checks

CRC32 and SHA-256 are file fingerprints. Matching values mean the file contains exactly the expected data, even if its filename has changed.

| File | Size (bytes) | CRC32 |
| --- | ---: | --- |
| `Doraemon Memories - Nobita no Omoide Daibouken (Japan).gbc` | 1,048,576 | `D187CEC4` |
| `Doraemon Memories - English v1.0.gbc` | 1,048,576 | `0159B5E4` |
| `Doraemon Memories - English v1.0.ips` | 267,793 | `071EF900` |

### SHA-256

**Doraemon Memories - Nobita no Omoide Daibouken (Japan).gbc**

```text
78e3c25f8b4dc3eed1a0c4c5cf17243b276d34e4b7315b63931c3816e1f1f386
```

**Doraemon Memories - English v1.0.gbc**

```text
af63b815f1bbf9dc301e5fd304c7349dc925a1b6b3ea3b7f36cfeab6bcee8270
```

**Doraemon Memories - English v1.0.ips**

```text
fb2c7fc2b721699f1d238a68192f4ffdfa0522548b44f3e35bdfda41e24d93fa
```

## Screenshots

The `Screenshots` folder contains actual emulator captures at the Game Boy Color’s native **160 × 144** resolution: English title, two dialogue scenes, player selection, first-stage gameplay, and the original Japanese title for comparison. Dialogue images use isolated native scene previews. Images have not been enlarged or retouched.

## Verification and saves

The IPS patch has been checked to reproduce the supplied English ROM exactly. Automated checks cover translated script insertion, original commands, graphics boundaries, checksums, and selected native screens.

Complete manual playthroughs, every story route and physical infrared transfer have not been verified. Some preview entries depend on the debugger’s clean starting context.

Keep a backup of your saves. Older emulator save states can retain old text pointers or screen data; a new session is preferable when checking this release. The project’s save-state helper repairs Mednafen filename matching, but cannot guarantee compatibility of every old state.

This is an unofficial fan translation, not an official Doraemon or EPOCH release.
