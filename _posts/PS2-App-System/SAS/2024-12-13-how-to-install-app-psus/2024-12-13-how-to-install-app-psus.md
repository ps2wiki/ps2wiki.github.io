---
layout: post
title: How to install App PSUs
subtitle: Easy to follow guide that demonstrates how to install SAS compliant App PSUs
author: korax
wiptag: Completed
factcheck: Pending
categories: [PS2-App-System/SAS]
banner: 
  image: https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/banner.png?raw=true
  opacity: 0.5
image: https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/banner.png?raw=true
tags: SAS Beginner FAQ
top: 1
sidebar: []
---

### Scope 
This guide will walk you through the very very basics of installing an App via it's SAS Compliant APP PSU* in your MemoryCard.

### What is an App PSU?
Before beginning, you might ask yourself what is an APP PSU and why do we need it? For starters a PSU file is like a .zip file for the PS2, we can use it to pack stuff on the console. Much like zip files, if you package some files in a PSU they remain exactly in the same position after extraction. The reason this is useful is that we can package PS2 executables (or ELFs) along with other interesting stuff like icons and configuration into 1 easy to share and install file.

### What makes a PSU 'SAS Compliant'?
SAS is a new upcoming standard on the PS2 which aims to unify how apps work and interact with each other on the PS2. When we talk about a SAS Compliant PSU we mean a PSU which has the following:
- A 'prefix' to denote what 'type' of Application is in the package. Example: `SYS` for System-Apps, `GME` for Games, `APP` for Standard executables.
- A 3D icon with it's type indicators which shows up in the OSDSYS (PS2's Browser) with separate Copy and Delete icons for the respective action.
- A `title.cfg` file which contains basic information about the app and makes it readable and executable from other apps such as Open PS2 Loader (OPL) and RetroLauncher.
...and more. <br>

Now that we know what we are working with let us move on to the 

### Prerequisites
You'll need:
- A MemoryCard with atleast 1MB free space
- A way to launch LaunchELF/uLaunchELF/wLaunchELF
- A USB drive formatted as FAT32 with atleast 2MB free space
- A way to copy over the APP PSU downloaded from [SAS Apps Archive](https://ps2wiki.github.io/sas-apps-archive/)
- Patience to follow the guide (Most important)

### Steps 
#### Step 1: Open LaunchELF
Once you are in LaunchELF, check the version to make sure the one you are using can extract PSUs.
<div class="container">
    <img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-1.png?raw=true">
</div><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-2.png?raw=true">
</div><br>

#### Step 2: Find the PSU
Press 'Circle' to enterthe FileBrowser, then navigate to your FAT32 formatted USB 
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-3.png?raw=true">
</div><br>
Press circle to enter it and look for the PSU(s) you want to install.  
Tip: You can select multiple PSUs by pressing 'Cross' on each one of them a dot will appear before their name to let you know they are selected.
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-5.png?raw=true">
</div><br>
Once you have highlighted the PSU(s) you want to install, Press 'R1' to bring up the Menu and navigate to 'Copy' and select it by pressing 'Circle'.
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-6.png?raw=true">
</div><br>
#### Step 3: Installing
Once you have successfully 'Copied' the file(s) (check the box on the right), we will now paste them.
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-7.png?raw=true">
</div><br>
Navigate to your MemoryCard where you wish to install the App and press 'Circle' to Enter it.
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-8.png?raw=true">
</div><br>
Now press 'R1' to open the Menu again and navigate to the <strong style="color: red">psuPaste</strong> option and press circle.
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-9.png?raw=true">
</div><br>
Now relax for a while and let the PS2 copy stuff over. Don't press any buttons on the controller or unplug/remove your MC, USB drive, controller or any other accessory.
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-10.png?raw=true">
</div><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-11.png?raw=true">
</div><br>
Once the dialogue box disappears, the app should be installed on your MemoryCard.
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-12.png?raw=true">
</div><br>

#### Step 4: Verification
You can verify if everything is installed as expected. 
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-13.png?raw=true">
</div><br>
Now reboot your PS2 and naviagte to the 'Browser' and 'MemoryCard 1 or 2' (depending on where you installed the app)
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-14.png?raw=true">
</div><br>

#### Step 5: Rinse and Repeat!
Congratulations! Now that you have learned how to install SAS Compliant APP PSUs you are free to explore whatever apps you may come across. 
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-15.png?raw=true">
</div><br>
If you come across somethimg which is not on the [SAS Apps Archive](https://ps2wiki.github.io/sas-apps-archive/), let us know and we will add it at the earliest! See ya! <div style="height: 20px" class="tenor-gif-embed" data-postid="7679297590304077870" data-share-method="host" data-aspect-ratio="1.56028" data-width="100%"><a href="https://tenor.com/view/hi-hello-smile-smiley-face-goofy-gif-7679297590304077870"></a>from <a href="https://tenor.com/search/hi-stickers"></a></div> <script type="text/javascript" async src="https://tenor.com/embed.js"></script>

