---
layout: post
title: Internal Memory VS External Memory
subtitle: Description and comparison of different storage mediums used by the PS2
author: Berion
wiptag: Completed
factcheck: Verified
categories: General
banner: 
  image: https://img4.dhresource.com/webp/m/0x0/f3/albu/jc/s/09/b6343f23-fd05-4413-aafb-1ba7b38dc6cc.jpg
  opacity: 0.5
image: https://img4.dhresource.com/webp/m/0x0/f3/albu/jc/s/09/b6343f23-fd05-4413-aafb-1ba7b38dc6cc.jpg
tags: Beginner FAQ
top: 1
sidebar: []
---

## Internal Memory VS External Memory

The **PlayStation 2** doesn't have an operating system, making it handle all the storage by *each application separately*! Programs can use the firmware's built-in modules, but these only exist for the internal hard drive. So depending on the program and device, different logical structures are supported. In the following material, I try to describe the differences, which as much as possible can be -- and often are -- confusing to someone so far unfamiliar with the PS2 homebrew scene.

### External Memory:

#### USB
The first ever support for additional storage was **USB** (i.e. flash drives), which was even implemented in a few games (e.g. “Gran Turismo 4”). Initially, compatibility with devices was low and for some reason higher if the file system was not **FAT32** but **FAT16** or even **FAT12** (there were also times when users juggled "USBD.IRX" files because just such a module from just such a game or application, supported their device). Due to the fact that many programs have closed code and their authors abandoned them long ago, the universal medium is and will remain a flash drive: with a partition table **MBR** and **one partition** with any of the file systems I mentioned earlier.

#### i.Link
With the advent of the [PS2ESDL](https://sites.google.com/view/ysai187/home/projects/ps2esdl#h.p_DeSddFqr7A1v) (game loader, one of the alternatives to the USB Advance/Extreme and, of course, the [Open PS2 Loader](https://github.com/ps2homebrew/Open-PS2-Loader/releases)) came support for i.Link (a **FireWire 400** compatible standard), which was briefly installed in PS2 consoles (present in SCPH-30004R models, for example). It has never gained popularity, and requires external power supply for, say, a hard drive or pendrive.

#### MX4SIO
A few years later, the **MX4SIO**, an SDHC/SDXC card reader that plugs into a memory card slot (not to be confused with a PlayStation 2 Memory Card, which it is not and cannot be), also joined the family.

#### Block Device Manager (BDM)
All of the above mess of modules ("USBD.IRX"/"USBMASS.IRX"/"ILINK.IRX") has been replaced by the eponymous **BDM**, which has unified support for all of these devices, multiple partition tables (in addition to MBR, also **GPT**) and multiple file systems (such as the recently added **exFAT**). Thus, we can assume that BDM is now synonymous of support for **all EXTERNAL memory** (although in the case of BDM used, for the time being **exclusively** in [OPL GD](https://github.com/grimdoomer/Open-PS2-Loader/releases), also internal).

* **Interface**: USB, i.Link, MX4SIO
* **Partition Tables**: MBR, GPT or none (the last two exclusively by [OPL GD](https://github.com/grimdoomer/Open-PS2-Loader/releases))
* **File Systems**: FAT12, FAT16, FAT32, exFAT, EXT2 (the last exclusively by [E2OPL](https://sourceforge.net/projects/e2opl/files/))

### Internal Memory:

A separate world is **INTERNAL MEMORY**, i.e. a **PATA** (Parallel ATA) hard drive, connected to (depending on the console model) a **special external enclosure** via PCMCIA (SCPH-1xxxx) or **Network Adaptor** via a dedicated port (SCPH-3xxxx/5xxxx models), or if you solder well ;) then directly to the motherboard (SCPH-700xx). Even if the Network Adaptor is unlicensed or a counterfeit and/or with a board replacing the old PATA by the newer **SATA** (Serial ATA), such a solution is most often referred to simply as **IDE** (as this is the standard). You may still encounter the term "iHDD" (from "internal HDD"), but it is rarely used.

<div class="note">
  <strong>NOTE:</strong> Connecting a hard drive via USB or i.Link, does not make it an internal drive!
</div>

* **Interface**: PATA (SATA, after board replacement in Network Adaptor)
* **Partition Tables**: APA (native), GPT or none (the last two exclusively by [OPL GD](https://github.com/grimdoomer/Open-PS2-Loader/releases))
* **File Systems**: PFS (native), EXT2 (Linux), RFS v3.5 (Linux), RAW (e.g. game disc images for the PS2), exFAT (the last exclusively by the [OPL GD](https://github.com/grimdoomer/Open-PS2-Loader/releases), but **not** on the APA)
