# Tekken 6 Native Online (Xbox 360)

This is a forked version to fix the "unimplemented function mscms.dll.WcsCreateIccProfile" error i was getting when running through Lutris.

Tekken 6 for Xbox 360 running natively on Windows (recompiled, no emulator) with rollback netcode (GGPO principle) and
an online lobby in the launcher.

**This is a test release (v0.1).** Expect bugs; please report them.

Download: see **Releases** (`tekken6_native_online.zip`). The package contains **no part of the game**. You build the
game yourself from **your own copy** of Tekken 6 for Xbox 360 (a disc image `.iso`). Both players must use the same
version of the package.

## Requirements

- Windows 10 or 11, 64-bit
- A graphics card with DirectX 12
- Your own Tekken 6 for Xbox 360 disc image: **Tekken 6 (USA, Europe), Rev 1** (`.iso`, or the extracted disc folder).
  Other versions are refused by the builder.
- About 10 GB of free disk space (game data 6.7 GB + the build)

## Installation (first time only)

1. Extract `tekken6_native_online.zip` into its own folder (not into Program Files).
2. If Windows reports missing Visual C++ files, run `vc_redist.x64.exe` from the folder.
3. Start `Tekken6 Native Online.exe`.
4. In the launcher open **Profile -> BUILD GAME**, pick your Tekken 6 `.iso` and start the build.
   The launcher checks the image, copies the game data to `native\game`, translates the game's code from your copy
   and compiles it on your PC (about 3-10 minutes depending on the CPU). Everything stays in the package folder.
5. Done. The launcher uses the built game automatically.

## Playing

Log in (or play as a guest), find an opponent in the lobby and play. The game starts directly in the fight; it stays
open between matches. Matches are first to 3 rounds. A stable connection matters (cable is better than Wi-Fi).

## Updating

The launcher looks for new versions and updates itself with one click (from v0.2 on). After an update that changes the
game code, the launcher asks you to build the game again (your game data is kept).

## Bug reports

Please send the files from the package folder: `native\build.log` (build problems) and the newest log of the game.

## Credits

Big thanks to **mahmoud-mess** for [tekken6-recomp](https://github.com/mahmoud-mess/tekken6-recomp) - his Tekken 6
recompilation work gave this project faster recompiled code. Thank you!
