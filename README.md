# QuickFlash v2.1.0

QuickFlash is a professional desktop application for programming STM32 microcontrollers using ST-Link. It provides a simple and reliable way to flash bootloader and application binaries with automatic device handling and clear status feedback.

## Overview

QuickFlash is designed for production, development, and testing environments where consistent and repeatable STM32 flashing is required. The tool combines common programming tasks into a single workflow with a user-friendly graphical interface.

## Features

* Dual binary programming (bootloader and application)
* Automatic detection and handling of Read-Out Protection (RDP)
* Full flash memory erase
* ST-Link connection testing
* Real-time log output
* MCU device information reading
* Keyboard shortcuts for faster operation
* Clean and intuitive GUI inspired by ST-Link Utility

## System Requirements

* Operating System: Windows 7, 8, 10, or 11 (64-bit)
* Memory: Minimum 2 GB RAM
* Disk Space: At least 50 MB
* Programmer: ST-Link V2 or compatible
* Driver: ST-Link USB driver

## Dependencies

QuickFlash requires the ST-Link Command Line Interface.

* Required executable: ST-LINK_CLI.exe
* Installed with: STM32 ST-Link Utility
* Default installation path:
  C:\Program Files (x86)\STMicroelectronics\STM32 ST-LINK Utility\ST-LINK Utility\

## Installation

### Installer Version

1. Download QuickFlash-v2.1.0-Setup.exe
2. Run the installer with administrator privileges
3. Follow the setup instructions
4. Launch QuickFlash from the Start Menu or Desktop shortcut

### Portable Version

1. Download QuickFlash-v2.1.0.exe
2. Place the executable in any directory
3. Ensure the stlink folder containing ST-LINK_CLI.exe is located in the same directory
4. Run QuickFlash-v2.1.0.exe

## Getting Started

### ST-Link Setup

* Connect the STM32 board using ST-Link
* Ensure the ST-Link driver is properly installed
* Launch QuickFlash
* The application will automatically detect ST-LINK_CLI.exe
* If detection fails, manually browse to the executable location

### Loading Binary Files

Bootloader:

* Select the bootloader binary file
* Default flash address: 0x08000000

Application:

* Select the application binary file
* Set the correct flash start address according to your memory layout

### Programming the Device

1. Click the Connect button to verify communication
2. Optionally read device information and RDP status
3. Click Start Upload
4. QuickFlash will perform the following steps automatically:

   * Disable RDP if enabled
   * Erase flash memory
   * Program the bootloader
   * Program the application
   * Reset and start the MCU

## Keyboard Shortcuts

* Ctrl+B: Load bootloader file
* Ctrl+A: Load application file
* Ctrl+T: Test connection
* Ctrl+I: Read device information
* Ctrl+R: Check RDP status
* Ctrl+E: Erase flash memory
* Ctrl+L: Clear log
* Alt+F4: Exit application

## Notes

* Do not disconnect the ST-Link or target device during flashing
* Ensure correct flash addresses before programming
* Close other ST-Link-based tools before running QuickFlash

## License

Specify the license information here.

## Support

For issues, feature requests, or improvements, please use the GitHub Issues section.
