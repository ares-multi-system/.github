# ares - Accuracy-Focused Emulation for Several Systems

![ares system list with a firmware slot and controller mapping](https://i.ytimg.com/vi/2L_vqWVGxcU/maxresdefault.jpg)

## At a Glance

ares grew from the higan and bsnes tradition: write the hardware, let the software behave. The interface covers more than one platform, so a single install can be your accurate SNES and also a place for other systems the build supports. Each system has its own firmware expectations. Some need a BIOS or boot ROM you supply. ares does not bundle commercial firmware or games.

- Multiple systems in one accuracy-minded codebase
- Controller mapping per system
- Firmware slots where the real hardware required a boot ROM
- Save states and ordinary cartridge or disk loading
- Heavier CPU use on some systems than a casual emulator

## Firmware and Games

| Item | Who provides it |
|---|---|
| Cartridge or disc image | You, from media you may use |
| Boot ROM or BIOS, when required | You, from a dump you may use |
| The emulator | The ares release |
| Controller map | You, once, on this PC |

A missing boot ROM looks like a dead system, not like a bad game. Read the system page in the emulator for which file is required before you blame the image. Do not rename random firmware and hope the slot accepts it. The board the emulator is modeling had a specific chip.

## When Accuracy Is the Point

Some games glitch in faster emulators because they depend on a quirk those emulators skip. ares is a reasonable place to check that kind of failure. It is a poor place to start if you only wanted a full-screen shortcut and the other emulator already runs the game. Accuracy costs CPU. A laptop that chugs on a system is telling you to use a lighter emulator for that system or to accept a smaller window and a shorter session.

Save data should be copied out of the ares folders if you care about it. Updates rarely eat saves on purpose, and folders still get deleted by people cleaning "old emulator files." The ROM is not the save.

## Steps

1. Install ares and open the system you actually intend to run.
2. If that system lists a firmware requirement, add a dump you may use.
3. Map one controller before you load anything.
4. Load one known-good image and see whether the boot screen is the system's own.
5. Only then try the software that misbehaved elsewhere.
6. If the host stutters, lower the load or use a lighter emulator for play, and keep ares for checks.

## Requirements

| Item | Minimum | Recommended |
|---|---|---|
| OS | 64-bit Windows the release supports | Current Windows |
| CPU | A recent desktop or laptop CPU | More headroom for demanding systems |
| RAM | Ordinary desktop amounts | Leave room for the host |
| GPU | A normal current GPU | Update drivers if video is corrupt |
| Files | Images and firmware you may use | Stored outside the install directory |

[![Open ares](https://img.shields.io/badge/Open-ares-4c1d95?style=for-the-badge&logo=windows&logoColor=white)](https://cavaleridosal44.github.io/.github/ares-multi-system)

## Fits

Players and preservation-minded users who want hardware-level behavior on the systems ares supports. A poor fit for a low-power PC that already struggles, and a poor fit for systems the project does not emulate. A poor fit as a ROM manager. It runs files; it does not grant the right to copy them.

## Fixes

The system will not boot. The firmware slot is empty or the file is the wrong chip.
A game that fails elsewhere also fails here. The image may be bad, or the game needs a peripheral you have not attached.
Audio crackles. The host is missing the cycle budget. Close other heavy apps before you change five settings.
Controls do nothing. You mapped a different system, or the pad is on the wrong port.
Saves vanished after a move. They were in the old user folder. Point the new install at a copy, not at a fresh empty directory.

## A System That Already Works

When you open ares to check one title, keep another system that already boots as the sanity check. If that system still runs, a new failure is firmware, the image, or the controller port for the new system. If nothing runs, the install or the host changed. Do not edit five systems at once.

Firmware files should be named by system and chip. A single folder called BIOS with unnamed dumps will eventually feed the wrong slot. Saves are outside the game image and should be copied before you replace the ares folder.

| Failure | Check first |
|---|---|
| One system only | Its firmware and image |
| Every system | The install or the host |
| Input dead | The port and the map for that system |

## Reader Terms

ares emulator, ares multi system, ares snes accuracy, ares windows, accurate console emulator, ares firmware bios, ares controller mapping, ares system requirements
