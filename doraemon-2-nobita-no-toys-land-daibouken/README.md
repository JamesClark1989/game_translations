# Doraemon 2: Nobita's Toys Land Adventure

English translation — **Version 1.0** · Released October 18, 2026

An English fan localization of *Doraemon 2: Nobita no Toys Land Daibouken*,
originally released for the Super Famicom in 1993. Join Doraemon, Nobita,
Shizuka, Gian and Suneo in an adventure combining side-scrolling action,
town exploration, conversations and Doraemon's gadgets.

## Required original Japanese ROM

Apply this patch to the untouched Japanese game, **without a 512-byte copier
header**. A matching filename alone is not sufficient: check the file hashes.
Do not apply it to an already translated or otherwise modified ROM.

```text
Filename: Doraemon 2 - Nobita no Toys Land Daibouken (Japan).sfc
Revision: 0 (Japanese release)
Size:     1,048,576 bytes (1 MiB; headerless)
CRC32:    D343B398
MD5:      3908a11b8a82bc2e99766a1ed9ca17e4
SHA-1:    8672e208c3716b8fae3fd612bc80679a5459b616
SHA-256:  3fe6952b916dd6b4495eb9efc9e2a69c2e88317fbc82c01efbec490dac9ce5b4
```

## Applying the patch

1. Keep an unchanged backup of your Japanese ROM.
2. Open a ROM patcher that supports **BPS** and choose its apply-patch option.
3. Select `Doraemon 2 - Nobita's Toys Land Adventure (English v1.0).bps` as the patch.
4. Select the original Japanese `.sfc` file listed above as the source ROM.
5. Save the output as `Doraemon 2 - Nobita's Toys Land Adventure (English v1.0).sfc`.
6. Check the output size and hashes below, then open the patched ROM in your
   SNES emulator or copy it to your flash cartridge.

If the patcher reports a source/checksum mismatch, stop and check the ROM hashes,
revision and copier-header status. Do not force the patch onto a different ROM.
Renaming a file does not change its checksum or remove its header.

The private `_final` folder also contains the already patched ROM requested by
the project owner. That copy needs no further patching. **Share the BPS patch
and documentation only; do not distribute ROMs or save states.**

## Expected English ROM

```text
Filename: Doraemon 2 - Nobita's Toys Land Adventure (English v1.0).sfc
Size:     2,097,152 bytes (2 MiB)
CRC32:    9F6F4E24
SHA-256:  113194ec71aeb3e5ebf5a519160c433f97039493cf09a81ea947c9eac015ecc2
```

The ROM expands from 1 MiB to 2 MiB to hold English text and graphics. This is
expected. Version 1.0 uses the same ROM content as the verified v0.24 build;
the release name and package metadata were updated afterward.

## Patch identification

```text
Filename: Doraemon 2 - Nobita's Toys Land Adventure (English v1.0).bps
Format:   BPS
CRC32:    2144DF1C
SHA-256:  f6ffdce029045736283bc0a124d2c3c38dc8d8d2fd0d1f443e2b49db287840dc
```

## Translation features

- English dialogue, story text, tutorials, gadget descriptions and credits.
- English title, Options, Game Over, character selection and password displays.
- English final post-credit farewell: “See you in the next game!”
- Storybook Balanced lettering with the project's refined I, T, Y and j.
- Newly supplied English Doraemon title logo and translated sequel subtitle.
- Faster opening text while retaining input waits and scripted pauses.
- Latin-character passwords; an early-game generate/enter/resume check passed.

The current census contains **443 translated and inserted script pages, with
0 known pages left**, plus **25 inserted graphics entries**. Graphics are counted
separately from script pages. File-based editorial records show 31 approved
script pages and 412 awaiting review; browser feedback may be newer.

## Playing and testing notes

This is an unofficial fan translation. Doraemon and the original game belong to
their respective rights holders; the translation is not an official release.

The game normally starts with all weapons available; story gadgets and
blueprints are separate. Game Over's English labels and both Continue choices
were checked directly. Password generation, entry and an early-game restore
were also checked. Passwords are now shown using Latin letters, digits and
punctuation; do not assume a Japanese-script password can be typed directly
without converting its character indices.

The project owner reported a completed playthrough with everything working
until the final Japanese farewell. That line was subsequently translated.
The title logo was then replaced at the owner's request. Automated byte checks
showed that the logo update changed only its private tiles/colors and the ROM
checksum. The original Japanese ROM is preserved unchanged.

Targeted emulator checks supplement that user report; they do not establish
exhaustive branch coverage or a new SNES/FXPAK Pro hardware certification.
The direct-entry final-card test has a palette discrepancy shared by its
Japanese and English fixtures: the English glyph shape and unchanged picture
were compared, but final colors have not been rechecked through a natural
ending. Shipping palette bytes were not changed by that text fix.

FXPAK Pro music behavior after loading a save state is a separate compatibility
question. This release does not claim to fix audio-state restoration. Prefer
normal game progress/passwords when checking behavior independently of states.

## Included screenshots

All five PNG files are actual emulator captures, not reconstructed previews.

| File | Content |
| --- | --- |
| `01-title-screen.png` | English title/menu with the supplied rounded Doraemon logo |
| `02-dialogue-Sayuri.png` | The doctor reacts to Sayuri being taken |
| `03-dialogue-Gian.png` | Gian: “We've got Doraemon!” |
| `04-dialogue-rescue.png` | Doraemon promises to rescue her |
| `05-dialogue-danger.png` | Doraemon: “We have to stop him!” |

The title screenshot was captured from v0.24, whose ROM is byte-identical to
v1.0. The four dialogue screenshots are existing v0.13 captures; their displayed
English wording and font were checked against v1.0 and match. No new playthrough
was performed to create this release package.

`CONTENTS.json` records screenshot sources and hashes. `build.json` records build
provenance. The project README and `analysis/QA.json` contain fuller technical
notes, test scope and remaining verification limits.

For issue reports, include your patch/output ROM hash, emulator or hardware,
password or location, reproduction steps and a screenshot when possible.
