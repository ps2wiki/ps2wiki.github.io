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
---

<h3>Scope</h3> 
This guide will walk you through the very very basics of installing an App via it's SAS Compliant APP PSU* in your MemoryCard.

<h3>What is an App PSU</h3>
Before beginning, you might ask yourself what is an APP PSU and why do we need it? For starters a PSU file is like a .zip file for the PS2, we can use it to pack stuff on the console. 
Much like zip files, if you package some files in a PSU they remain exactly in the same position after extraction. The reason this is useful is that we can package PS2 executables (or ELFs) along with other interesting stuff like icons and configuration into 1 easy to share and install file.
PSUs also preserve the timestamp data of the package, allowing for pinned applications within the PS2 Browser or knowing when an app was last updated.

<h3>What makes a PSU SAS Compliant</h3>
SAS is a new upcoming standard on the PS2 which aims to unify how apps work and interact with each other on the PS2. When we talk about a SAS Compliant PSU we mean a PSU which has the following:
<ul>
  <li>A 'prefix' to denote what 'type' of Application is in the package. Example: <code>SYS</code> for System-Apps, <code>GME</code> for Games, <code>APP</code> for Standard executables.</li>
  <li>A 3D icon with it's type indicators which shows up in the OSDSYS (PS2's Browser) with separate Copy and Delete icons for the respective action.</li>
  <li>A <code>title.cfg</code> file which contains basic information about the app and makes it readable and executable from other apps such as Open PS2 Loader (OPL) and RetroLauncher.</li>
</ul>
...and more. <br>

Now that we know what we are working with let us move on to the... 

<h3>Prerequisites</h3>
You'll need:
<ol>
  <li>A MemoryCard with atleast 1MB free space</li>
  <li>A way to launch LaunchELF/uLaunchELF/wLaunchELF</li>
  <li>A USB drive formatted as FAT32 with atleast 2MB free space</li>
  <li>A way to copy over the APP PSU downloaded from <a href="https://ps2wiki.github.io/sas-apps-archive/">SAS Apps Archive</a></li>
  <li>Patience to follow the guide (Most important)</li>
</ol>

<h3>Steps</h3>

<h4>Step 1 Open LaunchELF</h4>
Once you are in LaunchELF, check the version to make sure the one you are using can extract PSUs.<br><br>
<div class="container">
    <img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-1.png?raw=true">
</div><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-2.png?raw=true">
</div><br>

<h4>Step 2 Find the PSU</h4>
Press 'Circle' to enter the FileBrowser, then navigate to your FAT32 formatted USB <br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-3.png?raw=true">
</div><br>
Press circle to enter it and look for the PSU you want to install. <br><br>


<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-5.png?raw=true">
</div><br>
Once you have highlighted the PSU you want to install, Press 'R1' to bring up the Menu and navigate to 'Copy' and select it by pressing 'Circle'. <br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-6.png?raw=true">
</div><br>
<h4>Step 3 Installing</h4>
Once you have successfully 'Copied' the file (check the box on the right), we will now paste it.<br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-7.png?raw=true">
</div><br>
Navigate to your MemoryCard where you wish to install the App and press 'Circle' to Enter it.<br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-8.png?raw=true">
</div><br>
Now press 'R1' to open the Menu again and navigate to the <strong style="color: red">psuPaste</strong> option and press circle.<br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-9.png?raw=true">
</div><br>
Now relax for a while and let the PS2 copy stuff over. Don't press any buttons on the controller or unplug/remove your MC, USB drive, controller or any other accessory.<br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-10.png?raw=true">
</div><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-11.png?raw=true">
</div><br>
Once the dialogue box disappears, the app should be installed on your MemoryCard.<br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-12.png?raw=true">
</div><br>

<h4>Step 4 Verification</h4>
You can verify if everything is installed as expected. <br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-13.png?raw=true">
</div><br>
Now reboot your PS2 and naviagte to the 'Browser' and 'MemoryCard 1 or 2' (depending on where you installed the app)<br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-14.png?raw=true">
</div><br>

<h4>Step 5 Rinse and Repeat</h4>
Congratulations! Now that you have learned how to install SAS Compliant APP PSUs you are ready to install whatever apps you may desire. <br><br>
<div class="container">
<img style="border:2px solid #16537e" align="left | top" width="600" height="400" src="https://github.com/ps2wiki/ps2wiki.github.io/blob/upstream/_posts/PS2-App-System/SAS/2024-12-13-how-to-install-app-psus/assets/2024-12-13-how-to-install-app-psus-15.png?raw=true">
</div><br>
If you come across something which is not on the <a href="https://ps2wiki.github.io/sas-apps-archive/">SAS Apps Archive</a>, let us know and we will add it at the earliest! <br><br>
<div style="display: flex"><div style="float:left" >See ya! &nbsp;</div> <div style="float: left"><img height="20" src="https://media.tenor.com/apJYeMKWeC4AAAAj/hi-hello.gif"></div>

