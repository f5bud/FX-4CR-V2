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

## Revision "R" Radio
[FX-4CR-V2R-25-11-08.zip](https://github.com/user-attachments/files/23434011/FX-4CR-V2R-25-11-08.zip) **(Requires calibration for versions prior to 25-10-28)**
- some cosmetic changes as 'C'elsius, 'F'arenheit, 'V'olts in status bar
- moved bluetooth menu to second position
- Reintroduction of the always-on mode for the screen

[FX-4CR-V2R-25-10-30.zip](https://github.com/user-attachments/files/23229465/FX-4CR-V2R-25-10-30.zip) **(Requires calibration for versions prior to 25-10-28)**
- active mars/cap by IF.ATT + PWR

[FX-4CR-V2R-25-10-28.zip](https://github.com/user-attachments/files/23189468/FX-4CR-V2R-25-10-28.zip) **(Requires calibration)**
>[!IMPORTANT]
This version completely erases the EPROM.<br>
New radio memory management allows split frequency pairs to be stored.<br>
The EPROM is partitioned into three areas: calibrations, memories, and settings.<br>
Please read the **“Troubleshooting”** section of the user manual first.

- change the memory management logic
- change the SI5351 PLL frequency for sensitive models
 
[FX-4CR-V2R-25-10-18.zip](https://github.com/user-attachments/files/22983193/FX-4CR-V2R-25-10-18.zip) **(Need factory reset for versions prior to 25-10-15)**
- extension of the 10m to 11m band

[FX-4CR-V2-R-25-10-15.zip](https://github.com/user-attachments/files/22954374/FX-4CR-V2-R-25-10-15.zip) **(Need factory reset)**
- adds bandwidth adjustment to TX
- change the low level on mic and aux to 10
- add menu for initial mode SSB or DIG when CAT cmd is send
- fix corrects the value of the attenuators
- fixed problem with hamlib and split mode in wsjt-x
- change revision number to 2.14
- two displays (normal and large)
- see the changelog.txt in the zip file

## Revision "V" Radio
[FX-4CR-V2V-25-11-08.zip](https://github.com/user-attachments/files/23434013/FX-4CR-V2V-25-11-08.zip) **(Requires calibration for versions prior to 25-10-28)**
- some cosmetic changes as 'C'elsius, 'F'arenheit, 'V'olts in status bar
- moved bluetooth menu to second position
- Reintroduction of the always-on mode for the screen

[FX-4CR-V2V-25-10-30.zip](https://github.com/user-attachments/files/23229500/FX-4CR-V2V-25-10-30.zip) **(Requires calibration for versions prior to 25-10-28)**
- active mars/cap by IF.ATT + PWR

[FX-4CR-V2V-25-10-28.zip](https://github.com/user-attachments/files/23189682/FX-4CR-V2V-25-10-28.zip) **(Requires calibration)**
>[!IMPORTANT]
This version completely erases the EPROM.<br>
New radio memory management allows split frequency pairs to be stored.<br>
The EPROM is partitioned into three areas: calibrations, memories, and settings.<br>
Please read the **“Troubleshooting”** section of the user manual first.

- change the memory management logic
- change the SI5351 PLL frequency for sensitive models

[FX-4CR-V2V-25-10-18.zip](https://github.com/user-attachments/files/22983203/FX-4CR-V2V-25-10-18.zip) **(dont't use this version, jump directly to 25-10-28)**
- change revision number to 2.14
- extension of the 10m to 11m band
- adds bandwidth adjustment to TX
- add menu for initial mode SSB or DIG when CAT cmd is send
- two displays (normal and large)
- and more ...

[FX-4CR-V2-V-25-02-19.zip](https://github.com/user-attachments/files/19410620/FX-4CR-V2-V-25-02-19.zip)
- user manual update and warning regarding keyer and mic ports
- add user manual
- change in SSB and transmission bandwidth 300-2700 Hz
