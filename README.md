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
[FX-4CR-Backup.pdf](updates/FX-4CR-Backup.pdf)
&nbsp;
To use these versions, you must calibrate the radio. Consult the manual and follow the recommendations!

>[!NOTE]
A firmware update may cause the radio to crash at startup.
In this case perform a <ins><b>FACTORY RESET</b></ins>. Press A.B. + PWR until radio starts.

## Revision "R" Radio
[FX-4CR-V2-R-25-03-23.zip](https://github.com/user-attachments/files/19410614/FX-4CR-V2-R-25-03-23.zip)

[FX-4CR-V2-R-25-03-23.zip](updates/FX-4CR-V2-R-25-03-23.zip) $${\color{red}Factory \space reset \space need \space !!!}$$
- Add serial number in the first menu item
- Change the noise reducer with a Kalman filter, adapted to voice
- Change key to activate reducer ! (press AF)

[FX-4CR-V2-R-25-03-10.zip](updates/FX-4CR-V2-R-25-03-10.zip) $${\color{red}Factory \space reset \space need \space !!!}$$ (if you are coming from a version prior to 25-03-08)
- Change AF in ranges 0-63 to fine tune, especially headset

[FX-4CR-V2-R-25-03-08.zip](updates/FX-4CR-V2-R-25-03-08.zip) $${\color{red}Factory \ reset \ need \ !!!}$$
- Add bass and treble control for speaker
- Add bass and treble control for microphone in AM, FM, SSB

The zip file contains three files:
- FX-4CR-V2-R.hex: firmware to be flashed with ”STM32CubeProg” under Windows.
- FX-4CR-V2-R.bin: firmware to be flashed with “dfu-util” under Linux.
- FX-4CR-User-Manual (V2.xx-R).pdf: user and maintenance manuals included.



## Revision "V" Radio
[FX-4CR-V2-V-25-02-19.zip](updates/FX-4CR-V2-V-25-02-19.zip)
+ User manual update and warning regarding keyer and mic ports
+ Add user manual
+ Change in SSB and transmission bandwidth 300-2700 Hz

[FX-4CR-V2-V-25-01-27.zip](updates/FX-4CR-V2-V-25-01-27.zip)
- Fix an inconsistent power level
- Fix Screen error, sometimes the screen appears to be shifted by several lines.

As promised, this version lets you record a voice message of up to 10 seconds and play it back in a loop.
I've merged the user and service manuals into a single document.
The zip file contains three files:
- file.hex: firmware to be flashed with ”STM32CubeProg” under Windows.
- file.bin: firmware to be flashed with “dfu-util” under Linux.
- file.pfd: radio manual.
