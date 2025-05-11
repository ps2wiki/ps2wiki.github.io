---
layout: post
title: Open PS2 Loader flavors
subtitle: A description of how versions and flavors of Open PS2 Loader flavors differ from the each other
author: Berion
wiptag: Completed
last_updated: 2025/05/10
factcheck: Verified
categories: [Open PS2 Loader]
banner: 
  image: https://www.psx-place.com/attachments/opl-logo-2025-png.45831/
  opacity: 0.5
image: https://www.psx-place.com/attachments/opl-logo-2025-png.45831/
tags: Beginner FAQ OPL
---

## Open PS2 Loader flavors

The **Open PS2 Loader** project has managed to grow into a number of stable as well as beta versions, plus some significant forks. There are so many that it is difficult for someone not following the so-called scene to choose the right one. I have listed the OPL versions below in order of appearance of the projects. Each with a brief description of how it differs from the others.

*The short name for **Open PS2 Loader** is **OPL** but you may also come across **OPNPS2LD**. Both are correct.*

## Open PS2 Loader <sup>[[1](https://github.com/ps2homebrew/Open-PS2-Loader/releases)]</sup>
That is **OPL**. Due to the nature of the PlayStation 2, it is worth keeping a few versions that differ in their compatibility with games, especially with additional features such as IGR, IGS, GSM, PADEMU, VMC. These I think are worth keeping:
- 0.9.3
- 1.1.0
- 1.2.0 beta (build 2049)
- 1.2.0 beta (newest build)

#### Main Changes:
Version 1.0.0 added support for **[MX4SIO](https://www.trisaster.de/page/index.php?topic=575)** and significantly increased compatibility with games. In 1.1.0 added support for **[i.Link](https://en.wikipedia.org/wiki/I.link)** and "<span style="color:#0F86FF">hdd0:/__common/OPL/conf_hdd.cfg</span>", a configuration file with the path to the resource partition (the default is "hdd0:/+OPL"). 1.2.0 brought many revolutionary features like, **[NBD](https://en.wikipedia.org/wiki/Network_block_device)** server (build 1635), <span style="color:#0F86FF">*.zso</span> support (build 1871), **exFAT** file system and **GPT** partition table (build 1987, but on internal HDD only in 2184), **[APA-Jail](https://www.psx-place.com/resources/ps2-hdd-decryption-helper.1507/)**. You can find a complete list per build in the changelog (inside release archive).

#### Which archive to download?
The file "<span style="color:#0F86FF">OPNPS2LD.7z</span>" contains the zipped all-in-one version. The file with "<span style="color:#0F86FF">VARIANTS*</span>" contains the uncompressed, all-revisions of a specific build (i.e. with selected functionalities). The others are source code, language files and direct link files for automatic updates.

If you need a specific build, you can find them all [here](https://mega.nz/folder/Ndwi1bAK#oLWNhH_g-h0p4BoT4c556A/folder/FR4Q3YgC).

<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44451-337b977395038b14775f6d8891d5c501.jpg" width=50%"/></p>

## E2OPL <sup>[[1](https://sourceforge.net/projects/e2opl/files/)]</sup>
Fork adding support for the EXT2 file system, based on (if I remember correctly) OPL v0.9.3.

#### Version:
- 0.1.1

#### Unique Features:
- EXT2 support.
- No need to defragment disc images on EXT2.

## Open PS2 Loader Daily Build <sup>[[1](https://github.com/Jay-Jay-OPL/OPL-Daily-Builds/releases)]</sup>
That is, **OPL DB** or **OPL TA**. Although the name suggests that it is the official OPL so much that it is the latest, in reality it is a fork of the OPL - on top of which it is not respected among the so-called scene (and unfortunately it is still wildly popular on YouTube, Reddit, sellers etc.). This is because it has an integrated [POPStarter](https://www.psx-place.com/resources/popstarter.683/) against the wishes of the author; a number of disastrous code changes that result in problems unknown in OPL and other forks (e.g. lower compatibility; VRAM problems; random zeroing virtual PSX cards); a plagiarised theme that includes bitmaps belonging to Apple. The author himself repeatedly lies about the OPL DB, so you may find information on the internet contradicting that above...

#### Versions not worth owning: ;)
- 0.9.1 (which is called 10th Anniversary, hence the abbreviations OPL DB TA or OPL TA)
- 1.2.0 beta (the latest build)

#### Unique Features:
- Due to the integration of the PSX emulator, it includes an ELM category where PSX disc images are listed. While this is a very important functionality for many, please note that OPL can do the same, only not in a dedicated category, but in APPS (e.g. [that way]()).
- Additional assets in themes (e.g. third frame for screenshot, game logo).

<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44452-c9817122c2ed37dfffc3643206b484a8.jpg" width=50%"/></p>

## Open PS2 Loader v1-MOD <sup>[[1](https://github.com/SvenGDK/Open-PS2-Loader/releases)]</sup>
Fork based on OPL v1.0.0, with some changes from more recent versions backported.

#### Version:
- 2024-05-16

#### Unique Features:
- Supports guitars from the PS3
- Enables booting of games via OPL-Launcher on DESR models.

<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44455-ac1c2136e002216137177992da3abb69.jpg" width=50%"/></p>

## Open PS2 Loader Modular PADEMU <sup>[[1](https://github.com/belek666/Open-PS2-Loader/tree/modularPademu)]</sup>
OPL fork with joypad support for Xbox 360. Unfortunately unfinished, only source code available.

## Open PS2 Loader Grimdoomer <sup>[[1](https://github.com/grimdoomer/Open-PS2-Loader/releases)][[2](https://www.psx-place.com/threads/testers-needed-opl-internal-exfat-2tb-hdd-and-multi-bdm-devices.40018/)]</sup>
That is, **OPL GD** (unofficial abbreviation). Fork focusing on support for an internal hard drive formatted with MBR/GPT/no partition table, with exFAT file system.

#### Versions:
- 1.2.0.6-1996 Beta
- 1.2.0.6-1996 Beta (PADEMU)
- 1.2.0.6-1996 Beta (UDMA+, which means support for UDMA5/UDMA6 mode)

#### Unique Features:
- Support for exFAT and GPT (this functionality has now been added to OPL v1.2.0).

<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44453-15cd93245d925c5f4db43b981e886fda.jpg" width=50%"/></p>

## X2P <sup>[[1](https://github.com/koraxial/Xbox-2-PlayStation-Emulator-AlFa/releases)]</sup>
**Xbox-to-PlayStation** is a fork based on the OPL 1.2.0 Beta build **2081**. Although it was just an April Fools' joke (X2P pretends to be an Xbox Classic emulator for the PS2), it is still a full-fledged OPL that can be used almost in the same way as any other (it differs in folder names for covers, disc images, etc.).

#### Version:
- 0.5.4 alpha 17022 REV5

<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44459-5a6851550d25953e3909c5cca4b1f681.jpg" width=50%"/></p>

## unofficial Open PS2 Loader <sup>[[1](https://www.psx-place.com/resources/abandoned-unofficial-open-ps2-loader-uopl.1523/)][[2](https://github.com/NathanNeurotic/uOPL/releases)]</sup>
That is, **uOPL**. Fork based on OPL v1.2.0 beta build 2049, but backported to PS2SDK v1.0.

#### Versions:
- 2024-12-23
- 2024-12-23 Betrayal (replaced grey-white background with black, not recommended :P)

#### Unique Features:
- Favourites category added.
- BDM GPT and APA-Jail support (this functionality has now been added to the OPL v1.2.0).
- Support for multiple partitions and multiple BDMs at once (this functionality has now been added to OPL v1.2.0).
- Cover Flow style theme (but there is also a classic list).

<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44456-6453d8a44fba81bcdcf6958a60678ca3.jpg" width=50%"/></p>
<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44457-2209020c5336bb21ece6ac5bbd956088.jpg" width=50%"/></p>

## Open PS2 Loader MMCE <sup>[[1](https://github.com/ps2-mmce/Open-PS2-Loader/releases)]</sup>
That is, the **OPL MMCE**. Fork dedicated to memory card emulators such as **[SD2PSX](https://sd2psx.net/)**, **[PSXMCG2](https://www.bitfunx.com/product/psxmemcard-gen2-memory-card-for-playstation1-ps-one-playstation2-game-consoles/)** or **[MCP2](https://www.8bitmods.wiki/memcard-pro2)**.

#### Versions:
- beta2 i beta3 (beta3 differs from beta2 only in having the correct MMCE icon)
- beta2 HDD Fix (beta2 but with correct support for BDM HDD and APA)

#### Unique Features:
- Enables automatic switching of the virtual PS2 card to match the game's GameID.
- Allows the loading of disc images from a microSD card inserted in the MMCE.

<p align="center"><img src="https://www.psx-place.com/data/attachments/44/44454-81644aa3df8dc45eaa4c861f7305f6ad.jpg" width=50%"/></p>
