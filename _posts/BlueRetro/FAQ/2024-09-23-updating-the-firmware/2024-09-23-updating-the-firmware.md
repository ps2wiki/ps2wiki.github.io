---
layout: post
title: Updating the Firmware on the BlueRetro
subtitle: The firmware for on BlueRetro is upgradable, with newer versions sometimes offering additional features like game-specific profiles. Here's how you can approach upgrading the firmware and what to expect from the update.
author: Ripto
categories: [BlueRetro]
banner: 
  image: https://repository-images.githubusercontent.com/198868981/98d05272-da79-4387-97af-7aaa665b2ff9
  opacity: 0.5
image: https://repository-images.githubusercontent.com/198868981/98d05272-da79-4387-97af-7aaa665b2ff9
tags: BlueRetro FAQ Tutorial
---

### Upgrading BlueRetro Firmware
4	
5	1. **Check Current Firmware Version**:
6	   - Access the BlueRetro web interface by connecting via Bluetooth and visiting:  
7	     **http://blueretro.io**
8	   - The current firmware version is often displayed in the interface or accessible via a settings/about page.
9	
10	2. **Download the Latest Firmware**:
11	   - Visit the BlueRetro GitHub releases page to find the latest firmware version:  
12	     **https://github.com/darthcloud/BlueRetro/releases**
13	   - Download the latest release compatible with your ESP32 board.
14	
15	3. **Update the Firmware**:
16	   - Follow the instructions in the **BlueRetro Wiki** for updating the firmware. This typically involves:
17	     - Connecting the ESP32 to your computer via USB.
18	     - Using tools like **esptool** to flash the new firmware onto the ESP32.
19	   - Detailed instructions for updating can be found here:  
20	     **https://blueretro.io/wiki/#/updating**
21	
22	4. **Verify Profile Management Features**:
23	   - After updating, recheck the BlueRetro web interface to confirm if **game-specific profiles** or advanced remapping features are available.
24	   - The latest firmware versions should include the ability to create and manage multiple profiles, allowing you to configure specific button mappings for different games.
25	
26	### What to Expect with Upgraded Firmware
27	
28	- **Game-Specific Profiles**: With newer firmware, you should be able to save and switch between different button remapping profiles. This means you can have specific configurations for different games.
29	- **Profile Management**: Look for options in the web interface that allow you to create, save, and switch profiles. This feature enables you to customize your setup based on the needs of each game.
30	- **Improved Functionality**: Upgrades often come with bug fixes and new features, improving overall performance and usability.
31	
32	### Resources
33	
34	- **BlueRetro GitHub Releases**:  
35	  **https://github.com/darthcloud/BlueRetro/releases**
36	
37	- **BlueRetro Wiki (Updating Firmware)**:  
38	  **https://blueretro.io/wiki/#/updating**
39	
40	By upgrading to the latest firmware, you can access advanced features like game-specific profiles, enhancing your gaming experience with customizable button mappings.
