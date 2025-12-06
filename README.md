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
The "R" version uses the same firmware. See the user manual.

## Firmwares:
[FX-4CR-V2V-25-11-26.zip](https://github.com/user-attachments/files/23770914/FX-4CR-V2V-25-11-26.zip) **(Requires calibration for versions prior to 25-10-28)** <br>
[FX-4CR-V2VR-25-11-26.zip](https://github.com/user-attachments/files/23770916/FX-4CR-V2VR-25-11-26.zip) **(Requires calibration for versions prior to 25-11-20)** <br>
[FX-4CR-V2R-25-11-26.zip](https://github.com/user-attachments/files/23770917/FX-4CR-V2R-25-11-26.zip) **(Requires calibration for versions prior to 25-10-28)** <br>

- fix a problem with DAC initialization
- menu divided into sections specific to CW, Voice and Digi
##
[FX-4CR-V2V-25-11-20.zip](https://github.com/user-attachments/files/23724151/FX-4CR-V2V-25-11-20.zip) **(Requires calibration for versions prior to 25-10-28)** <br>
[FX-4CR-V2VR-25-11-20.zip](https://github.com/user-attachments/files/23724152/FX-4CR-V2VR-25-11-20.zip) **(Requires calibration)** <br>
[FX-4CR-V2R-25-11-20.zip](https://github.com/user-attachments/files/23724154/FX-4CR-V2R-25-11-20.zip) **(Requires calibration for versions prior to 25-10-28)** <br>

- raised cosine for the less sweet CW sidetone
- added hardware modifications "R-2025"
- standardization of versions
- "VR" radio support

## Older firmwares:
[FX-4CR-V2R-25-11-15.zip](https://github.com/user-attachments/files/23562756/FX-4CR-V2R-25-11-15.zip) **(Requires calibration for versions prior to 25-10-28)** <br>
[FX-4CR-V2V-25-11-15.zip](https://github.com/user-attachments/files/23562760/FX-4CR-V2V-25-11-15.zip) **(Requires calibration for versions prior to 25-10-28)** <br>
- raised cosine for CW sidetone
- some cosmetic changes as 'C'elsius, 'F'arenheit, 'V'olts in status bar
- moved bluetooth menu to second position
- Reintroduction of the always-on mode for the screen
- active mars/cap by IF.ATT + PWR
- change the memory management logic
- change the SI5351 PLL frequency for sensitive models
- extension of the 10m to 11m band
- adds bandwidth adjustment to TX
- change the low level on mic and aux to 10
- add menu for initial mode SSB or DIG when CAT cmd is send
- fix corrects the value of the attenuators
- fixed problem with hamlib and split mode in wsjt-x
- change revision number to 2.14
- two displays (normal and large)
- see the changelog.txt in the zip file
