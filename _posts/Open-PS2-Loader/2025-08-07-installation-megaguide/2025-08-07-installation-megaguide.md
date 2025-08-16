---
layout: post
title: OPL Installation Megaguide
subtitle: Easy to follow guide to upgrade/setup/troubleshoot Open PS2 Loader installations.
author: korax
wiptag: Not Completed
factcheck: Article Incomplete
categories: [Open-PS2-Loader]
# banner: 
#  image: NA
#  opacity: 0.5
# image: NA
tags: OPL Beginner FAQ
---

<!-- Warning -->
<div class="warning">
  <strong>WARNING:</strong> This page is still being worked on. Information might be missing or lacking important context. DO NOT use or cite this page or any information here as a relevant source till this message disappears.
</div>

### ➛ Scope
This guide will walk you through the processes of:
- Installing OPL with (preferably best settings & configurations for your unique setup and) no prior experience or knowledge of PS2 Modding.
- Upgrading / Downgrading an existing OPL installation in the event you encounter a bug or wish to try out a new or deprecated feature.
- Troubleshoot an error with a bad OPL install due to environment changes or improper config.

### ➛ What is Open PS2 Loader?
Before beginning, it is important to understand what OPL is and why are we using it in the first place. 
OPL is a game and application loader compatible with all PS2 & backwards compatible PS3 units with support for various devices (on PS2 units) namely:
- BDM (USB/MMCE/MX4SIO/exFAT format HDDs)
- APA format HDDs
- SMBv1 share devices
- UPDBD
- iLink (SBP2 compliant storage devices via IEE1394)

It supports loading files in the:
- *.iso
- *.zso
- .elf (for APPS)  
formats.

Along with this, OPL is also capable of advanced features like resolution switching (upto 1080i) via **GSM**,
emulating other gamepads like DS3/DS4 and passing them as PS2 compatible DualShock 2 controllers via **PADEMU ** and also injecting cheats into games at runtime.


### ➛ Determining the best configuration for our OPL install
Now that we have a good idea of *what OPL is*, we will now proceed to understand the various configurations it can be adapted to so you can determine which one works best with your particular setup. 

<div class="note">
 <strong>Note: </strong>It is recommended that you read <a href="https://ps2wiki.github.io/get_started.html#Getting-started-with-PS2-Modding-1">this section of 'Get Started'</a> to find out about the various PS2 Models.
</div> 

#### - For Phat PS2s
If you have a Phat model PS2 or a SCPH-70XXX model slim with the IDE HDD mod, you can use these setups below (sorted: best to worst):
1. APA Jail setup (APA Partitions + exFAT partitions on same disk)
2. Pure exFAT format HDD 
3. APA HDD Method
4. MMCE
5. MX4SIO
6. UDPBD 
7. SMBv1 share 
8. exFAT format USB Storage
9. iLink (only on models <SCPH-50XXX)

#### - For Slim PS2s
If you have a Slimline model PS2, you can use these setups below (sorted: best to worst):
1. MMCE
2. MX4SIO
3. UDPBD 
4. SMBv1 share 
5. exFAT format USB Storage

### ➛ APA Jail

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Phat model PS2
    2. Network Adaptor
    3. HDD/SSD
  </p></div>

### ➛ exFAT format HDD 

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Phat model PS2
    2. Network Adaptor
    3. HDD/SSD
  </p></div>

### ➛ APA format HDD 

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Phat model PS2
    2. Network Adaptor
    3. HDD/SSD
  </p></div>


### ➛  MMCE

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Any model PS2
    2. MMCE device like SD2PSX, Memcard Pro 2
  </p></div>

### ➛  MX4SIO

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Any model PS2
    2. MX4SIO Card
  </p></div>

### ➛  UDPBD 

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Any model PS2
    2. Network Adaptor (if Phat model PS2s)
  </p></div>

### ➛ SMBv1 share 

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Any model PS2
    2. Network Adaptor (if Phat model PS2s)
  </p></div>

### ➛  exFAT format USB Storage

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. Any model PS2
    2. USB Storage medium like Pendrive, external HDD
  </p></div>

### ➛ iLink 

<button type="button" class="collapsible">Requirements:</button>
<div class="content">
  <p>
    1. <SCPH-50XXX model PS2
    2. ??
  </p></div>





<!-- Script-->
<script>
var coll = document.getElementsByClassName("collapsible");
var i;

for (i = 0; i < coll.length; i++) {
  coll[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var content = this.nextElementSibling;
    if (content.style.display === "block") {
      content.style.display = "none";
    } else {
      content.style.display = "block";
    }
  });
}
</script>
