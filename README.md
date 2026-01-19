## FX-4CR-V2 firmware
This is a new firmware written from scratch for the [FX-4CR](https://bg2fx.com) radio.<br>

>[!CAUTION]
Use this firmware only if you are comfortable with the technique.<br>
Read and comprehend the service manual.<br>
Note down all the values of the various menus, both user and technical.<br>
The EEPROM memory has been erased.<br>
To return to official firmware, you must re-enter the previously noted values.

>[!IMPORTANT]
Use this document to back up your official radio setup
[FX-4CR-Backup.pdf](https://github.com/user-attachments/files/19410636/FX-4CR-Backup.pdf)
<br>To use these versions, you must calibrate the radio. Consult the manual and follow the recommendations!

>[!NOTE]
A firmware update may cause the radio to crash at startup.
In this case perform a <ins><b>FACTORY RESET</b></ins>. Press A.B. + PWR until radio starts.

The zip file contains three files:
- changelog.txt: history of changes and corrections
- (firmware).hex: firmware to be flashed with ”STM32CubeProg” under Windows.
- (firmware).bin: firmware to be flashed with “dfu-util” under Linux.
- (UserManual US).pdf: user and maintenance manuals included.

## Revision Radio:
- "V-2022" (October 2022)
- "VR-2024" (March 2024)
- "R-2024" (June 2024)
- "R-2025" (August 2025)

The "V" and "VR" versions are distinguished by their XT60 power connector and 3.5 mm USB jack connector.<br>
The "VR" version uses metal knobs.<br>
The "R" versions uses the same firmware. See the user manual.

## Firmwares:
[The versions can be found in Releases](https://github.com/f5bud/FX-4CR-V2/releases)
