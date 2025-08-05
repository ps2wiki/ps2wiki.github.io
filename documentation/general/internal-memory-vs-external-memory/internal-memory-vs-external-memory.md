---
layout: docs-general
title: Internal Memory VS External Memory
subtitle: >-
  Description and comparison of different storage mediums used by the PS2

image: https://img4.dhresource.com/webp/m/0x0/f3/albu/jc/s/09/b6343f23-fd05-4413-aafb-1ba7b38dc6cc.jpg
thumbnail: https://img4.dhresource.com/webp/m/0x0/f3/albu/jc/s/09/b6343f23-fd05-4413-aafb-1ba7b38dc6cc.jpg
category: docs
last_updated: 2025/05/09
wiptag: Completed
authors: Berion
factcheck: Verified
---

## Internal Memory VS External Memory

The **PlayStation 2** doesn't have an operating system, making it handle all the storage by *each application separately*! Programs can use the firmware's built-in modules, but these only exist for the internal hard drive. So depending on the program and device, different logical structures are supported. In the following material, I try to describe the differences, which as much as possible can be -- and often are -- confusing to someone so far unfamiliar with the PS2 homebrew scene.

## External Memory:

### USB
The first ever support for additional storage was **USB** (i.e. flash drives), which was even implemented in a few games (e.g. “Gran Turismo 4”). Initially, compatibility with devices was low and for some reason higher if the file system was not **FAT32** but **FAT16** or even **FAT12** (there were also times when users juggled "USBD.IRX" files because just such a module from just such a game or application, supported their device). Due to the fact that many programs have closed code and their authors abandoned them long ago, the universal medium is and will remain a flash drive: with a partition table **MBR** and **one partition** with any of the file systems I mentioned earlier.

### i.Link
With the advent of the [PS2ESDL](https://sites.google.com/view/ysai187/home/projects/ps2esdl#h.p_DeSddFqr7A1v) (game loader, one of the alternatives to the USB Advance/Extreme and, of course, the [Open PS2 Loader](https://github.com/ps2homebrew/Open-PS2-Loader/releases)) came support for i.Link (a **FireWire 400** compatible standard), which was briefly installed in PS2 consoles (present in SCPH-30004R models, for example). It has never gained popularity, and requires external power supply for, say, a hard drive or pendrive.

### MX4SIO
A few years later, the **MX4SIO**, an SDHC/SDXC card reader that plugs into a memory card slot (not to be confused with a PlayStation 2 Memory Card, which it is not and cannot be), also joined the family.

### MMCE
The successor to MX4SIO today is MMCE (**Multi-purpose Memory Card Emulator**). It allows you to access a microSD card (just like MX4SIO), but at the same time it also pretends to be a real memory card for PSX or PS2 (the selected card image, the console sees as a real memory card).

* **Interface**: USB, i.Link, SIO2
* **Partition Tables**: MBR, GPT or none (MMCE supporting MBR only)
* **File Systems**: FAT12, FAT16, FAT32, exFAT, EXT2 (the last exclusively by E2OPL)

## Internal Memory:

A separate world is **INTERNAL MEMORY**, i.e. a **PATA** (Parallel ATA) hard drive, connected to (depending on the console model) a **special external enclosure** via PCMCIA (SCPH-1xxxx) or **Network Adaptor** via a dedicated port (SCPH-3xxxx/5xxxx models), or if you solder well ;) then directly to the motherboard (SCPH-700xx). Even if the Network Adaptor is unlicensed or a counterfeit and/or with a board replacing the old PATA by the newer **SATA** (Serial ATA), such a solution is most often referred to simply as **IDE** (as this is the standard). You may still encounter the term "iHDD" (from "internal HDD"), but it is rarely used.

<div class="note">
  <strong>NOTE:</strong> Connecting a hard drive via USB or i.Link, does not make it an internal drive!
</div>

* **Interface**: PATA (SATA, after board replacement in Network Adaptor)
* **Partition Tables**: APA (native), MBR, GPT or none (the last three via BDM)
* **File Systems**: PFS (native), EXT2 (Linux), RFS v3.5 (Linux), RAW (e.g. game disc images for the PS2), exFAT (the last one via BDM)

## Drivers

As on any platform, dedicated drivers, or modules precisely, are needed to support the devices and logical structure. Unfortunately, such that would support "everything on everything" do not exist and are unlikely to ever exist. Currently, we can speak of a division into three environments:
1. the first, which supports APA and PFS, i.e. native partition table and native file system -- exclusively on internal memory
2. the second, which deals with external memory, but without MMCE and with internal memory (but with logical structures as for external: MBR/GPT and all FATs)
3. the third is MMCE

To make life even more complicated for the ordinary user, remember that old applications use old modules and newer ones won't without major code changes. Which means old applications can't take advantage of BDM, because they use dedicated modules for dedicated devices and file systems, which can't be replaced just like that.

### Block Device Manager (BDM)
**BDM** combines USB/i.Link/MX4SIO support, including partition tables (in addition to MBR, also **GPT**) and file systems (such as the recently added **exFAT**). BDM is the first attempt at driver unification on the PS2 scene.
