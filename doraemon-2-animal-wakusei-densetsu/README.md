DORAEMON 2: ANIMAL PLANET LEGEND
English Translation — Version 1.0
Author: mr_sausage
Platform: Nintendo Game Boy
Original title: Doraemon 2: Animal Wakusei Densetsu

ABOUT THE GAME

Join Doraemon and his friends on Animal Planet as they help Chippo and
Romy. Explore the world, talk to its inhabitants, collect useful gadgets,
and tackle action stages and bosses.

ABOUT THIS TRANSLATION

Version 1.0 translates all 1,066 discovered script fragments, including
dialogue, menus, gadget names, signs, and credits. Five text graphics have
also been translated, including title artwork and the gameplay HUD logo.
English artwork aims to preserve the style of the original Game Boy game.

The release includes fixes for dialogue spacing, unwanted blank dialogue
pages, item-return hangs, and the reported Star Ship and ending scene hangs.
Targeted checks passed, but a complete start-to-finish playthrough and
exhaustive translation review remain unfinished. Undiscovered issues may
remain; translating every discovered fragment does not prove that every
possible text entry has been found.

WHAT YOU NEED

- An unmodified Japanese ROM matching the source checksums below.
- The patch: Doraemon 2 - Animal Planet Legend (English) v1.0.ips
- An IPS-compatible patching program.
- A Game Boy emulator or compatible hardware to play the patched ROM.

HOW TO INSTALL THE PATCH

1. Keep a backup of your original Japanese ROM. Do not patch over it.
2. Compare the original ROM's SHA-256 or CRC32 with the values below.
   If they differ, use the correct source ROM before proceeding. IPS does
   not identify or reliably reject an incorrect source ROM.
3. Open your IPS patcher and select the original Japanese ROM as the input.
4. Select the included .ips file as the patch.
5. Apply the patch and save the result as a NEW .gb file, for example:
   Doraemon 2 - Animal Planet Legend (English) v1.0.gb
6. Verify that the output is 262,144 bytes and matches the patched ROM
   SHA-256 below.
7. Open that new .gb file in your emulator.

Apply the patch once to the unmodified original. Do not apply it to an
older English build. The ROM grows from 128 KiB to 256 KiB; this is expected.
If you already have the matching patched .gb file, open it directly.

CHECKSUMS

A checksum identifies the exact contents of a file. Renaming a file does
not change its checksum. SHA-256 is the preferred verification value;
CRC32, MD5, and SHA-1 are also listed for compatibility with ROM tools.

ORIGINAL JAPANESE ROM — INPUT TO PATCHER

File: Doraemon 2 - Animal Planet Densetsu (Japan).gb
Size: 131,072 bytes
CRC32: 843BD5BC
MD5: bbf5e9e76b28352665aff796a13830e8
SHA-1: 0d72e0310bbf0b23483f37688df61543048c4b31
SHA-256: dc51a652dfd6a1f4905897abf7f4d6248c5cfc376eaa26f1d00dbcbd75a924e9

ENGLISH VERSION 1.0 ROM — EXPECTED OUTPUT

File: Doraemon 2 - Animal Planet Legend (English) v1.0.gb
Size: 262,144 bytes
CRC32: 475FC5EB
MD5: 76b6e65d600dd88db899fd17bf806541
SHA-1: 44b5942cc6810449a0e3003fa3cf028b5ccbf93e
SHA-256: dc8895fe8bd0dd202dee01f2d2dccb4a1a584e44ef5253bc7822e64eb9c83574

IPS PATCH

File: Doraemon 2 - Animal Planet Legend (English) v1.0.ips
Size: 135,462 bytes
CRC32: BCE2AFB4
MD5: b507d0fb226dcacaec18e15e3de5c87a
SHA-1: 7922a7e1549e0249ac4a18868e02b97b94f63aab
SHA-256: e2059821de821a4263207c4efc2ca6c084d9f70a019393f707d1ae37c0b87608

On Linux, calculate SHA-256 with:
  sha256sum "filename.gb"

On Windows PowerShell, calculate SHA-256 with:
  Get-FileHash -Algorithm SHA256 -LiteralPath "filename.gb"

Replace filename.gb with the actual ROM filename. Use the same commands
with the .ips filename to verify the patch itself.

PLAYING FROM THIS PROJECT FOLDER

Patched game in Mednafen at 4x window scale:
  ./launch_game.sh

Original Japanese game in Mednafen at 4x window scale:
  ./launch_original.sh

Local translation review workshop:
  ./launch_review.sh

Optional mGBA launcher at 4x scale:
  ./launch_mgba_version.sh
This launcher loads the saved QA checkpoint in the underwater route before
Hedoron. It does not start a new game.

These scripts belong to the full project folder; they are not required to
apply the standalone IPS patch. Use your emulator's configured controls.
Screenshots supplied with this release are native 160 x 144 pixels.

SAVE STATES

Back up your saves before changing ROM versions or filenames. Save-state
formats differ between emulators; mGBA states cannot be loaded directly
in Mednafen. Renaming the release can also change where Mednafen looks
for its save states.

In the full project folder, close Mednafen and run:
  ./install_mednafen_state.sh

This prepares compatible saves under the current release filename while
preserving existing destination slots. It skips states it cannot safely
migrate. Save-state compatibility with arbitrary older builds is not
promised.

TROUBLESHOOTING AND BUG REPORTS

If the game will not start, check both the original and patched ROM hashes.
If an old state causes problems, test a fresh boot of the patched ROM.

For a bug report, include the release version, emulator and version, the
location in the game, the steps that caused the issue, and whether you
loaded a state from an older build. A screenshot or short video and a
save state from just before the issue are helpful.

CREDITS

English translation release: mr_sausage.
Doraemon and the original game belong to their respective rights holders.
This is an unofficial fan translation.
