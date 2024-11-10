---
layout: post
title: Format PS2's internal storage (using PS2 or PC)
subtitle: Formatting the PS2's internal HDD for various setups according to user preference
author: TnA & Ripto
wiptag: Completed
factcheck: Pending
categories: General
banner: 
  image: https://images.pexels.com/photos/6429164/pexels-photo-6429164.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1
  opacity: 0.5
image: https://images.pexels.com/photos/6429164/pexels-photo-6429164.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1
tags: Tutorial iHDD
top: 1
sidebar: []
---

<h2>Format via PS2 </h2>

<h3>Prerequisites:</h3>
- a way to launch Homebrew
- "wLaunchELF"

<h3>Procedure:</h3>
1. Start **"wLaunchELF"**
2. Enter **"Filebrowser"** (usually via `CIRCLE`)
3. Enter **"MISC"** (scroll to it and use the "confirmation button", which is either `CIRCLE` or `CROSS` depending on your configuration)
4. Launch **"HDDManager"**
5. Tap `R1`
6. Select **"format"** (scroll to it and mark it, then confirm)
7. Confirm formatting and it should be done in a few seconds.


<h4>***If you intend to use OPL,*** please stay in the HDDManager and create an appropriately sized +OPL-Partition!</h4>
1. Tap `R1`
2. Select **"create"**
3. Name it **"+OPL"**
4. Choose a size! This depends on the size of the HDD as well on what you want to use (i.e. 768MB for a 500GB storage, 1.2GB for a 1TB storage, 1.5GB for a 2TB storage.). VMCs require a bit more space, so keep that in mind!

<h4>***If you intend to use POPStarter, POPSLoader, or wLaunchELF_kHn***, please stay in the HDDManager and create one or more of the following partitions at up to 128GB each to meet your .VCD storage needs the same way you created the +OPL partition above.</h4>
- __.POPS
- __.POPS0
- __.POPS1
- __.POPS2
- __.POPS3
- __.POPS4
- __.POPS5
- __.POPS6
- __.POPS7
- __.POPS8
- __.POPS9

<h2>Format via Windows PC </h2>

<h3>Prerequisites:</h3>
* PFS-BatchKit-Manager: A utility for Windows that allows for the management and formatting of hard drives for PS2 use.
* https://github.com/GDX-X/PFS-BatchKit-Manager

<h3>Procedure:</h3>

1. Prepare Your PC Environment
Locate the PFS-BatchKit-Manager:
Find the folder on your PC where you've stored the PFS-BatchKit-Manager.
Right-click the .bat file (likely named !pfs-batchkit-manager.bat or similar) and select "Run as Administrator" to ensure it has the necessary permissions.

2. Access PFS-BatchKit Manager
Navigate to Advanced Menu:
Within the PFS-BatchKit Manager interface, find and enter the Advanced menu.
Select "HDD Management" from the list of options.

3. Hack Your HDD for PS2 Format
Choose the Option for PS2 Format:
Look for and select option "8 - Hack your HDD to PS2 Format".
This prepares your hard drive to be recognized and used by the PS2 system.

4. Format Hard Drive with wLaunchELF
After completing the preparation steps on your PC, safely disconnect the hard drive.
Connect the hard drive to your PlayStation 2 system, using the appropriate adapter if necessary.

5. Use wLaunchELF on Your PS2 to format again properly as instructed above.


<h2>Completing the Setup</h2>
After formatting and partitioning the HDD as required, you can proceed to install your Homebrew applications, games, or other content onto the newly prepared storage.
