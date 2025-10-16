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
- FX-4CR-V2-R.hex: firmware to be flashed with ”STM32CubeProg” under Windows.
- FX-4CR-V2-R.bin: firmware to be flashed with “dfu-util” under Linux.
- FX-4CR-V2R-User-Manual-US.pdf: user and maintenance manuals included.

## Revision "R" Radio
[FX-4CR-V2-R-25-10-15.zip](https://github.com/user-attachments/files/22954374/FX-4CR-V2-R-25-10-15.zip) **(Factory reset need)**
- adds bandwidth adjustment to TX
- change the low level on mic and aux to 10

[FX-4CR-V2-R-25-10-08.zip](https://github.com/user-attachments/files/22763898/FX-4CR-V2-R-25-10-08.zip) **(Factory reset need)**
- add menu for initial mode SSB or DIG when CAT cmd is send
- fix corrects the value of the attenuators

[FX-4CR-V2-R-25-10-07.zip](https://github.com/user-attachments/files/22737827/FX-4CR-V2-R-25-10-07.zip) **(Factory reset need)**
- fixed problem with hamlib and split mode in wsjt-x
- Changed the status bar to include the temperature
- Added an information splash in running beacon mode

[FX-4CR-V2-R-25-10-04.zip](https://github.com/user-attachments/files/22696031/FX-4CR-V2-R-25-10-04.zip) **(Factory reset need)**
- fix switching band filters error
- change revision number to 2.14
- two displays (normal and large)
- removed temperature in favor of larger font
- modification in the sidetone audio volume control
- reduced rx/tx switching time and logic change
- raised cosine waveform shaping for CW
- change in CW and SSB beacon, repeat 1 to 20
- faster power indicator to modulation
- add logic to exit menus when keyer or ptt is pressed

[FX-4CR-V2-R-25-09-23.zip](https://github.com/user-attachments/files/22500009/FX-4CR-V2-R-25-09-23.zip) Factory reset if you come from a version prior to 25-08-11
- change range Mic-Input-Level to (50 ... 400) Some people have problems with mic gain.

[FX-4CR-V2-R-25-09-13.zip](https://github.com/user-attachments/files/22311808/FX-4CR-V2-R-25-09-13.zip) Factory reset if you come from a version prior to 25-08-11
- add a short delay for displaying CW messages

[FX-4CR-V2-R-25-09-03.zip](https://github.com/user-attachments/files/22123386/FX-4CR-V2-R-25-09-03.zip) Factory reset if you come from a version prior to 25-08-11
- fix CW practice errors
- add trace of sent CW messages (long press AF to clear)
- change in split mode A or B indefinitely
- attempt to fix bug with hamlib and split mode (but it's not working at the moment)

## Revision "V" Radio
[FX-4CR-V2-V-25-02-19.zip](https://github.com/user-attachments/files/19410620/FX-4CR-V2-V-25-02-19.zip)
+ User manual update and warning regarding keyer and mic ports
+ Add user manual
+ Change in SSB and transmission bandwidth 300-2700 Hz

[FX-4CR-V2-V-25-01-27.zip](https://github.com/user-attachments/files/19410621/FX-4CR-V2-V-25-01-27.zip)
- Fixed an inconsistent power level
- Fixed Screen error, sometimes the screen appears to be shifted by several lines.
- As promised, this version lets you record a voice message of up to 10 seconds and play it back in a loop.
- I've merged the user and service manuals into a single document.
