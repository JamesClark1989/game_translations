# Doraemon - The Dream Thief and the Seven Gozans (English)

An unofficial, **partial English translation** of the Japanese Mega Drive game.
This package contains the current build with the rounded English logo and fitted,
scratchy red menu-selection circles. It is not a complete translation or a final
release; later content and a complete playthrough remain unfinished.

## Game information

| Field | Details |
| --- | --- |
| English title | Doraemon: The Dream Thief and the Seven Gozans |
| Original title | Doraemon - Yume Dorobou to 7 Nin no Gozans |
| Platform | Sega Mega Drive / Genesis |
| Game type | Action platform game |
| Original region | Japan / Japanese NTSC |
| Original header copyright | `(C)SEGA 1993.MAR` |
| Product code | `GM 00004094-00` |
| ROM size | 524,288 bytes (512 KiB), original and patched |
| Build identifier | Partial English build, Mega Drive checksum `28F1` |

The copyright/date and product information above come from the original ROM
header. The English subtitle is this project's translation.

## Files

- **`Doraemon - The Dream Thief and the Seven Gozans (English).bps`** — primary BPS patch, applied to the untouched Japanese ROM.
- `Doraemon-English.bps` — identical patch with the earlier short filename.
- `Doraemon-English-PATCHED.bin` — already patched ROM for local testing.
- `Doraemon-English.md` — the same patched ROM bytes with a Mega Drive extension.
  This `.md` file is a binary game ROM, not Markdown.
- Six native 320×224 emulator screenshots, linked below.
- `README.md` — these instructions and verified checksums.
- `README.txt` — compact package manifest and screenshot SHA-256 hashes.

Use one of the already patched ROM files to play locally. You do not need to
apply the patch to either of them. The BPS file itself contains patch data,
not a playable ROM.

## Patch notes

### English text and artwork

- English title subtitle, timed title lyrics and opening speech bubbles.
- Settings, quiz questions and choices, all eight quiz-result messages, and
  Continue/Quit text, with natural-English wording.
- Twelve later dialogue records covering boss challenges, Dream Orb prizes,
  musical-chairs instructions, final speeches and ending variants.
- Three wooden world-map signs, with small hand-drawn lettering in the original
  ink colour, preserving the wood, borders and sideways layouts.
- Six pickup announcements: Anywhere Door, Bamboo Copter, Butt Copter,
  Hustle Winder, Copy Robot and Ultra Stopper. Original red/yellow bubbles,
  borders, shadows and musical-note details are retained.

### Latest visual updates

- Replaced the earlier angular logo with the supplied rounded English wordmark,
  converted to crisp blue/cyan, white and yellow Mega Drive graphics.
- Kept the title subtitle red with a yellow outline and the bottom captions
  small and centred, using the original 8×8 English lettering.
- Fitted each red settings marker to its complete English label and placed it
  behind the black lettering. The circles now sit **two pixels lower than the
  previous fitted-outline build**, four pixels above the Japanese original.
- Restored the original scratchy pencil-circle artwork. Wider markers retain
  native pen strokes, gaps and overlapping marks rather than smooth ellipses.
- Preserved the exact approved Storybook Balanced 8×16 dialogue/menu glyph rows.
  The font has not been stretched or thickened.
- Preserved title animation tiles and gameplay graphics; earlier title-sprite
  and post-title transition issues have been addressed and retested.

## Applying the BPS patch

1. Make a separate copy of your **unmodified Japanese ROM**. It must be exactly
   524,288 bytes and match the original SHA-256 and CRC32 below.
2. Open a BPS-compatible patching tool and select its patch-application function.
3. Select `Doraemon - The Dream Thief and the Seven Gozans (English).bps` as the patch.
4. Select the verified original Japanese ROM as the source.
5. Save the result under a new name, such as
   `Doraemon - The Dream Thief and the Seven Gozans (English).md`.
6. Verify the output against the patched-ROM SHA-256 and CRC32 below, then open
   it in a Mega Drive emulator with the Japanese NTSC region selected.

Apply **one** BPS patch to the original ROM. The two supplied BPS filenames are
identical copies, not sequential updates. A source mismatch means a different
ROM revision or a previously patched file was selected; use the fingerprinted
original rather than forcing the patch. Keep the original ROM unchanged.

From the full project root, you can also reproduce the patch application using
only Python 3 and this project's BPS decoder:

```sh
python3 - <<'PYTHON'
from pathlib import Path
from tools.bps import apply
source = Path('Doraemon - Yume Dorobou to 7 Nin no Gozans (Japan).md').read_bytes()
patch = Path('_final/Doraemon - The Dream Thief and the Seven Gozans (English).bps').read_bytes()
output = Path('build/Doraemon - The Dream Thief and the Seven Gozans (English).md')
output.parent.mkdir(exist_ok=True)
output.write_bytes(apply(source, patch))
print(output.resolve())
PYTHON
```

The decoder verifies the BPS source, target and patch CRC32 fields.

## Playing the game

Open `Doraemon-English-PATCHED.bin` or `Doraemon-English.md` in Mednafen and use
Japanese NTSC. In the full project, run this from the project root:

```sh
./launch_game.sh
```

The launcher verifies and opens the current production ROM in `build/` using
Mednafen, windowed at exactly 4× native resolution (1280×896). It passes no key
remaps. Mednafen's factory keyboard controls are WASD for directions, keypad
1/2/3 for Mega Drive A/B/C, and Enter for Start. Existing personal emulator
bindings may differ.

With the game's **Doraemon controls**, A jumps, B attacks and C runs.
With **Standard controls**, A runs, B jumps and C attacks.
Use the settings menu to choose the control scheme and Normal/Fun mode.

Other project launchers:

```sh
./launch_original.sh   # Untouched Japanese game in Mednafen
./launch_review.sh     # Offline screenshot review; local files, no server or ports
```

These scripts live in the full project root, one directory above `_final`.
They are not required when opening a patched ROM directly in an emulator.

## SHA-256, CRC32 and header checksums

These values are calculated from the actual files. The two patched ROM names
are byte-identical; the two BPS names are also byte-identical. CRC32 values in
the table cover the **entire file**, including the BPS footer where applicable.

| File | Bytes | CRC32 |
| --- | ---: | --- |
| `Doraemon - Yume Dorobou to 7 Nin no Gozans (Japan).md` | 524,288 | `EEED1130` |
| `Doraemon-English-PATCHED.bin` | 524,288 | `A227D16F` |
| `Doraemon-English.md` | 524,288 | `A227D16F` |
| `Doraemon - The Dream Thief and the Seven Gozans (English).bps` | 26,493 | `2144DF1C` |
| `Doraemon-English.bps` | 26,493 | `2144DF1C` |

SHA-256:

```text
54aac77159188dc230b8b6130d5207eb4aadce92a7bf5bd63ee48230510d193a  Doraemon - Yume Dorobou to 7 Nin no Gozans (Japan).md
3461c60d2871c719a120aa238e7d9a8f2ef7098a9f5684fbc0330740b0d987bc  Doraemon-English-PATCHED.bin
3461c60d2871c719a120aa238e7d9a8f2ef7098a9f5684fbc0330740b0d987bc  Doraemon-English.md
44ab2192cd3a2a76aea574c4a7074bb9292f6963e8f769a043366a5e5523bbb4  Doraemon - The Dream Thief and the Seven Gozans (English).bps
44ab2192cd3a2a76aea574c4a7074bb9292f6963e8f769a043366a5e5523bbb4  Doraemon-English.bps
```

Mega Drive header checksums (16-bit sums, distinct from CRC32):

- Original ROM: `5D37`.
- Patched ROM: `28F1`.

The BPS footer separately records:

- Source ROM CRC32: `EEED1130`.
- Target ROM CRC32: `A227D16F`.
- Patch integrity CRC32, excluding its final four-byte CRC field:
  `4E245A49`.

On Linux, `sha256sum "filename"` verifies a file's SHA-256. Use a CRC32 tool
that reports CRC32 rather than the different POSIX `cksum` algorithm.

## Screenshots

- [01-title.png](01-title.png)
- [02-world-map.png](02-world-map.png)
- [03-gameplay-stage-1.png](03-gameplay-stage-1.png)
- [04-gameplay-stage-3.png](04-gameplay-stage-3.png)
- [05-gameplay-stage-6.png](05-gameplay-stage-6.png)
- [06-settings-menu.png](06-settings-menu.png)

All six screenshots use this production ROM. Title and Stage 1 captures are from
Mednafen. The world map and settings are MAME captures reached through normal
startup input. Stage 3 and Stage 6 show the game's built-in attract demonstrations,
not completed manual playthroughs. Screenshot SHA-256 values are in `README.txt`.

## Verification and remaining limitations

This build has passed original-ROM fingerprint checks, ROM size/header checksum
checks, byte-exact BPS application, 24 Python tests and both offline review checks.
Native Mednafen and MAME checks cover startup, title animation, settings, quiz,
opening scenes, world map, gameplay entry and Continue/restart. All six settings
choices were checked for marker placement and unobscured black text. Six pickup
announcements were also verified in separate diagnostic ROMs; those diagnostics
do not establish natural collection of every item.

Some reaction labels and later-game artwork/dialogue remain untranslated or
unverified. A full natural playthrough, every boss and complete ending coverage
have not been established. This package should be treated as a work-in-progress
translation. Keep feedback with the scene and a screenshot where possible; the
offline review page supports notes and feedback export/import.

Distribute the BPS patch and documentation rather than full game ROMs.
