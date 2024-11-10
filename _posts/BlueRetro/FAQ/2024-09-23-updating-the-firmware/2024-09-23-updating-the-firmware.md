---
layout: post
title: Updating the Firmware on the BlueRetro
subtitle: The firmware for on BlueRetro is upgradable, with newer versions sometimes offering additional features like game-specific profiles. Here's how you can approach upgrading the firmware and what to expect from the update.
author: Ripto
wiptag: Completed
factcheck: Verified
categories: [BlueRetro]
banner: 
  image: https://repository-images.githubusercontent.com/198868981/98d05272-da79-4387-97af-7aaa665b2ff9
  opacity: 0.5
image: https://repository-images.githubusercontent.com/198868981/98d05272-da79-4387-97af-7aaa665b2ff9
tags: BlueRetro FAQ Tutorial
---

## Upgrading BlueRetro Firmware

1. **Check Current Firmware Version**:
   - Access the BlueRetro web interface by connecting via Bluetooth and visiting:  
     **http://blueretro.io**
   - The current firmware version is often displayed in the interface or accessible via a settings/about page.

2. **Download the Latest Firmware**:
   - Visit the BlueRetro GitHub releases page to find the latest firmware version:  
     **https://github.com/darthcloud/BlueRetro/releases**
   - Download the latest release compatible with your ESP32 board.

3. **Update the Firmware**:
   - Follow the instructions in the **BlueRetro Wiki** for updating the firmware. This typically involves:
     - Connecting the ESP32 to your computer via USB.
     - Using tools like **esptool** to flash the new firmware onto the ESP32.
   - Detailed instructions for updating can be found here:  
     **https://blueretro.io/wiki/#/updating**

4. **Verify Profile Management Features**:
   - After updating, recheck the BlueRetro web interface to confirm if **game-specific profiles** or advanced remapping features are available.
   - The latest firmware versions should include the ability to create and manage multiple profiles, allowing you to configure specific button mappings for different games.

## What to Expect with Upgraded Firmware

- **Game-Specific Profiles**: With newer firmware, you should be able to save and switch between different button remapping profiles. This means you can have specific configurations for different games.
- **Profile Management**: Look for options in the web interface that allow you to create, save, and switch profiles. This feature enables you to customize your setup based on the needs of each game.
- **Improved Functionality**: Upgrades often come with bug fixes and new features, improving overall performance and usability.

## Resources

- **BlueRetro GitHub Releases**:  
  **https://github.com/darthcloud/BlueRetro/releases**

- **BlueRetro Wiki (Updating Firmware)**:  
  **https://blueretro.io/wiki/#/updating**

By upgrading to the latest firmware, you can access advanced features like game-specific profiles, enhancing your gaming experience with customizable button mappings. 
