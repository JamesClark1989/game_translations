# Doraemon: Gadget Showdown — English translation

An English translation of **Doraemon: Taiketsu Himitsu Dougu!!** (ドラえもん 対決ひみつ道具!!), originally released in Japan for the Nintendo Game Boy.

## Game details

| Item | Details |
| --- | --- |
| Original title | Doraemon: Taiketsu Himitsu Dougu!! |
| English title | Doraemon: Gadget Showdown |
| Platform | Nintendo Game Boy |
| Developer | SAS Sakata |
| Publisher | Epoch |
| Original release | 1 March 1991, Japan |
| Genre | Action |
| ROM size | 131,072 bytes (128 KiB) |

Guide Doraemon through maze-like stages, using his futuristic gadgets to overcome enemies and obstacles. The subtitle is a shortened English adaptation of “Secret Gadget Showdown!!”. Game publication details: [GameFAQs](https://gamefaqs.gamespot.com/gameboy/569687-doraemon-taiketsu-himitsu-dogu/data).

## Files

The latest build is in `_final/`:

- `Doraemon - Gadget Showdown (English).ips` — translation patch.
- `Doraemon - Gadget Showdown (English).gb` — patched English ROM.
- `Title.png`, `Dialogue-1.png` through `Dialogue-4.png`, and `Action-1.png` through `Action-4.png` — screenshots at the native 160 × 144 resolution.

The patch format is **IPS**, not BPS. The `.ips` file must be applied to the original Japanese ROM; it cannot be played directly.

## How to patch

1. Make a copy of your original Japanese ROM, named `Doraemon - Taiketsu HimitsuDougu!! (Japan).gb` in this project.
2. Check that the ROM is exactly **131,072 bytes** and matches the **Original Japanese ROM** checksums below. A matching filename alone is not sufficient. Use the unmodified `.gb` file, not a ZIP archive or an earlier English build.
3. Open an IPS-compatible patcher such as [Floating IPS (Flips)](https://github.com/Alcaro/Flips).
4. Choose **Apply Patch**, select `Doraemon - Gadget Showdown (English).ips`, then select the original Japanese ROM.
5. Save the result separately as `Doraemon - Gadget Showdown (English).gb`.
6. Check the output against the **Patched English ROM** checksums below, then open it in your Game Boy emulator.

The original ROM is not overwritten by this project's builder. Applying the patch once to the correct source reproduces the included English ROM exactly. IPS does not contain a source-ROM checksum, so check the source hashes before applying it.

On Linux, calculate checksums with:

```bash
sha256sum 'Doraemon - Taiketsu HimitsuDougu!! (Japan).gb'
sha1sum 'Doraemon - Taiketsu HimitsuDougu!! (Japan).gb'
md5sum 'Doraemon - Taiketsu HimitsuDougu!! (Japan).gb'
```

On Windows PowerShell, use `Get-FileHash -Algorithm SHA256 'path\to\game.gb'`.

## ROM and patch checksums

These checksums describe the actual uncompressed files in this build. CRC32 uses the standard ZIP/IEEE CRC-32 algorithm.

<!-- BUILD-HASHES:START -->

### Original Japanese ROM

```text
File    Doraemon - Taiketsu HimitsuDougu!! (Japan).gb
Size    131,072 bytes
CRC32   A42524A3
MD5     E01F6FCB9BACCA86642744FA4003B349
SHA1    5E89E34A2CEC89E0ABA4E12D18D96671151730EC
SHA256  69095E4EDA7269988F5A2F2D13F0EE9DFDF7573FDCA55BD3D11DF325B71DF7D5
```

### Patched English ROM

```text
File    Doraemon - Gadget Showdown (English).gb
Size    131,072 bytes
CRC32   0EE493EE
MD5     9E569011A21C440C3B08100C48FDEB7C
SHA1    DB17293E69E271CA2EBC2E315461898AD83B473F
SHA256  7E77BEC1CDB24E59F090A81C5408934AB26C4658C4936A05F6C175E1D0E99239
```

### IPS patch

```text
File    Doraemon - Gadget Showdown (English).ips
Size    15,620 bytes
CRC32   E305363B
MD5     050E3010489C728182F9910EC48AD859
SHA1    CEB81962BEF12566C44A5CC2DA04BAFE144089E1
SHA256  6D90FCC1F098B469BA44196A79C9111C26A0792DEEB07EB09775D698AE87B513
```

<!-- BUILD-HASHES:END -->

## Translation details

The build inserts **396 dialogue and credit entries, 17 fixed interface strings, and the title graphic**. It includes English dialogue, menus, credits, passwords, a custom English font, and the supplied Doraemon logo with the “Gadget Showdown” subtitle. Original author, publisher, and broadcaster credits are retained.

Long messages use native page waits. YES/NO prompts wait for confirmation before showing their choices. Dialogue alignment preserves wide letters and clears leftover margin pixels between pages. Numeric glyphs are reserved so the final score remains readable.

All known extracted text and inspected lettering have been translated. Automated native text checks cover **419 pages**; opening, menu, password, choice, and ending-score checks also run in an emulator. This remains a review build: a complete walkthrough of every route and manual confirmation of staff-name romanizations are outstanding.

## Playing and reviewing

In this project, `Launch English Game.sh` opens the same English ROM from `build/` in Mednafen at **4× scale (640 × 576)**. Keeping this internal filename preserves the existing save-state naming. `Launch Original Game.sh` opens the original ROM at the same scale. Restart the emulator after rebuilding to load the updated ROM.

Select menu items with Up/Down and confirm with A or Start. A advances dialogue. The English password codes are `BTH`, `MIC`, `NAP`, and `FUT`.

Open `review/index.html` directly from disk for the offline review site. It needs no server, ports, or online dependencies. Export browser reviews as JSON to preserve edits and notes.

For build commands, review exports, and implementation notes, see [docs/DEVELOPMENT.md](docs/DEVELOPMENT.md).
