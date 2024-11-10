---
layout: post
title: Terms & Acronyms
subtitle: This list is meant as an introduction to all the acronyms and terms used in the PS2 Homebrew Scene
author: TnA
wiptag: Not Completed
verified: NA
categories: General
banner: 
  image: https://media.istockphoto.com/id/1175294239/photo/acronym-word-from-wooden-blocks-with-letters.webp?s=2048x2048&w=is&k=20&c=5tjM7GGKSvhEDJlMmWInz9q3NmWq1ytegO2X3sjZP5I=
  opacity: 0.5
image: https://media.istockphoto.com/id/1175294239/photo/acronym-word-from-wooden-blocks-with-letters.webp?s=2048x2048&w=is&k=20&c=5tjM7GGKSvhEDJlMmWInz9q3NmWq1ytegO2X3sjZP5I=
tags: beginner
top: 1
sidebar: []
---

## Apps, Exploits, Softmods:

### **FMCB** = *"Free MemoryCard Boot"* -->
- This is the most commonly used exploit/Softmod used on a vast variety of models.
- It is being installed on the MemoryCard.
- Works on SCPH-10000 to SCPH-90xxx (depending on the program version).
- Some 90k have BOOT-ROM 2.30 however and won't automatically boot FMCB.

### **FHDB** = *"Free HardDrive/HardDisk Boot"* -->
- internal storage/HDD variation of FMCB for FAT PS2s as well as 70k-Slim PS2s!
- It is installed onto the internal HDD.
- Works on 10k to 70k! (Note: 10k, 15k and 18k consoles also need a MemoryCard update to boot from HDD)
-  70k need FMCB to boot FHDB.
-  it's MBR bootstrap performs quick S.M.A.R.T test, as well as testing sector errors and FileSystem Errors. and kicks the FSCK program to fix errors in case it finds something out of place.

### **OpenTuna** --> 
A MemoryCard Exploit for the newest PS2-Model (SCPH-90k, with a BOOT-ROM version of 2.30) or PS2-models as well as MemoryCards which are not working with MagicGate.


## Devices:

- **MC** = *"MemoryCard"*
- **HDD** = *"Harddisk Drive"* and this ALWAYS means INTERNAL HDD!!!
- **USB** = *any storage-device connected via USB, regardless if it is a HDD, Flash/pendrive, SSD, SD, etc.* You call a USB HDD "HDD" in our scene? You do it WRONG! It is **"USB"**!
- **MX4SIO** = *SD connected via MC-Port*
- **i.Link/FireWire/s400/IEEE1394** = Firewire etc., only available up to 39k!
- **LAN** = SMB, UDPBD, etc., available on EVERY PS2!
- **XFROM** = Internal Flash memory on the PSX DESRs. it holds the PSX main bootloader

## Other things:

### **BOOT-ROM** = *often falsely referred to as "BIOS"*
- This is the chip holding the software/firmware the PS2 comes shipped with!
- It is NOT rewriteable in itself!
- it is splitted/partitioned into several parts:
   + `rom0:` holds console software
   + `rom1:` holds console DVDPlayer (does not exist on `SCPH-10000`/`SCPH-15000`/`DTL-Hxxxxx`/`COH-Hxxxxx`)
   + `rom2:` only exists on `SCPH-50009`. holds the chinese special font and one additional file
   + `rom3:` the **ROMDRV** driver supports up to `rom3`. however, no PS2 was ever found having a `rom3` registered.
