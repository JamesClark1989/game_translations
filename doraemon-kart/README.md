# Doraemon Kart — English Translation v1.0

An English fan translation of **Doraemon Kart** for the original **Game Boy**, with Super Game Boy support retained.

## About the game

Doraemon Kart is a racing game featuring Doraemon, Nobita, and their friends. It was released by Epoch in Japan on **March 20, 1998**. The story begins with everyone at school getting into Mini 4WD racing—and Nobita wanting a car of his own. The game offers **Story Mode**, **VS Mode**, and **Time Attack**.

Release details: [GameFAQs](https://gamefaqs.gamespot.com/gameboy/570033-doraemon-kart/data). The story and mode descriptions above are based on the game itself.

## How to apply the patch

You need the original Japanese game file and the `.bps` patch. Keep your original file as a backup.

1. If either file is inside a ZIP archive, extract it first.
2. Open [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) in your browser.
3. Beside **ROM file**, choose `Doraemon Kart (Japan) (SGB Enhanced).gb`.
4. Beside **Patch file**, choose `Doraemon Kart (English) v1.0.bps`.
5. Check that the original ROM’s **CRC32 is DD4E588F**. If the patcher reports a mismatch, stop and check your original file. Do not force the patch onto a different version.
6. Click **Apply patch** and save the new `.gb` file. You can name it `Doraemon Kart (English) v1.0.gb` if the patcher chooses a different filename.
7. Open the new file in your Game Boy emulator.

Apply the patch to the **untouched Japanese ROM**, not to an older translation or an already-patched English file. Renaming a file does not change which version it contains. Leave checksum-fixing options off: the patch already produces the correct checksums.

Rom Patcher JS supports BPS patches; its [official project page](https://github.com/marcrobledo/RomPatcher.js/) also provides the tool for people who prefer a local copy.

## What changed in the English version?

- English dialogue, course descriptions, menus, and credits.
- Native English title artwork, race labels, pause text, the GOAL! banner, and the “CONGRATS!” illustration.
- Layout and spacing improvements for clearer text.
- Dialogue lettering appears twice as fast as in the original.

The graphics are changed inside the game itself. They are not emulator overlays.

## File checksums

A checksum is a file’s fingerprint. It helps confirm that you have the right original and that a download has not changed. You do not need to understand the numbers to play. For patching, checking the original’s CRC32 is a useful first step; the longer SHA values identify the files more precisely.

### Original Japanese game — patch input

Japan release, revision 0; 256 KiB; Super Game Boy enhanced.

```
Filename: Doraemon Kart (Japan) (SGB Enhanced).gb
Size:     262,144 bytes
CRC32:    DD4E588F
MD5:      20B436FC3C9621EB4EE82BC3EF3687FB
SHA-1:    F19734B2CB19DE0BE2D9E80297F567806CE4CAD5
SHA-256:  07593E44CFE2D3FACE9779BCB40BCEE4D7F74EE8B3CB0E601ABC3A508AF13FB4
```

### English v1.0 game — patch output

```
Filename: Doraemon Kart (English) v1.0.gb
Size:     262,144 bytes
CRC32:    624829CB
MD5:      BB3101F4C4AA057529F6B8BE8C4B73C1
SHA-1:    E4EAC798BD508B6C5200CB168040C9D7C38EF23D
SHA-256:  8BD25DABE022EC49C4ADA8185B965CB853A8E48EF77163042AD5556FC1C01855
```

### English v1.0 BPS patch

```
Filename: Doraemon Kart (English) v1.0.bps
Size:     17,026 bytes
CRC32:    2144DF1C
MD5:      F42946AF056F89997B255EA1CDFD91F0
SHA-1:    C62A385FACEB6E2B288645B3E27F64EEA392CA85
SHA-256:  B230FE292A9E7D19065B5CAFD81CD854EBB3C348D69D7E74569879D5D817290B
```

## Credits and release notes

The original game is by Epoch and uses the Doraemon characters. This is an unofficial fan translation, not an official English release. Original in-game company attributions are retained.

The project owner contributed artwork edits and playtesting. Translation, graphics, build tools, and validation were developed in this project with Codex assistance.

**Version 1.0 — October 30, 2026:** packaged the playtested English ROM and matching BPS with clean filenames, four dialogue screenshots, and this guide.
