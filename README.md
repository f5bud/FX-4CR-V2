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

## Revision "R" Radio
[FX-4CR-V2-R-25-09-03.zip](https://github.com/user-attachments/files/22123386/FX-4CR-V2-R-25-09-03.zip) Factory reset if you come from a version prior to 25-08-11
- fix CW practice errors
- add trace of sent CW messages (long press AF to clear)
- change in split mode A or B indefinitely
- attempt to fix bug with hamlib and split mode (but it's not working at the moment)

[FX-4CR-V2-R-25-08-28.zip](https://github.com/user-attachments/files/22026212/FX-4CR-V2-R-25-08-28.zip) Factory reset if you come from a version prior to 25-08-11
- fix CAT error with hamlib
- reduced power consumption by lowering the CPU clock and using sleep mode
- without a signal, the consumption is less than 190mA at 12.0V
- add a copie of changelog.txt in the zip

[FX-4CR-V2-R-25-08-20.zip](https://github.com/user-attachments/files/21899473/FX-4CR-V2-R-25-08-20.zip) Factory reset if you come from a version prior to 25-08-11
- add table of contents in manual-user
- minor logic changes in SSB beacon mode

[FX-4CR-V2-R-25-08-11.zip](https://github.com/user-attachments/files/21712788/FX-4CR-V2-R-25-08-11.zip) Factory reset need !!!
- fix bug in backup calibration
- add timer and repeat beacon (see user-manual)

[FX-4CR-V2-R-25-08-01.zip](https://github.com/user-attachments/files/21550767/FX-4CR-V2-R-01-08-25.zip) Factory reset if you come from a version prior to 25-06-19
- update SM CAT commands, add PC, PS CAT commands
- The VFO can go down to 200kHz
- The spectral purity of the VFO has been improved
- Add DC remover over AM demod
- Fix loPass on AM

[FX-4CR-V2-R-25-06-26.zip](https://github.com/user-attachments/files/20928095/FX-4CR-V2-R-25-06-26.zip) Factory reset if you come from a version prior to 25-06-19
- Update CAT cmds for SIMPLE software, a logbook, and more for Android: [SIMPLE by SP5NZF](https://sites.google.com/view/9h48sqc6ygs8c3kx9pg2/home)

[FX-4CR-V2-R-25-06-19.zip](https://github.com/user-attachments/files/20818463/FX-4CR-V2-R-25-06-19.zip) Factory reset need !!!
- Add overruns indicator when signals are very hight
- Adopt global Rit, Xit, Split selection mode (Long press Tune to change mode)
- Upgrade CAT commands and put FR and FT
- Fixed a lost bit during I2S transfer
- Fixed float to 24bits conversion
- Active hipass in wm8978, remove software hipass
- Change version number to 2.12

[FX-4CR-V2-R-25-06-08.zip](https://github.com/user-attachments/files/20643460/FX-4CR-V2-R-25-06-08.zip) Factory reset need !!!
- Fixed a stupid bug in Bluetooth Rx/Tx
- Changed RSSI and FFT routines
- Added waterfall offset for the eatch band (-30 dB, +20 dB)
- Transparent menu background
- <b>RSSI calibration has changed !</b> (If you don't want to recalibrate, add +10 to RSSI-Cal)

[FX-4CR-V2-R-25-04-30.zip](https://github.com/user-attachments/files/19997009/FX-4CR-V2-R-25-04-30.zip) Factory reset need !!!
- Add noise blanker

[FX-4CR-V2-R-25-04-17.zip](https://github.com/user-attachments/files/19790533/FX-4CR-V2-R-25-04-17.zip) Factory reset need !!!
- Changed key assignments for more logic
- Add notch filter
- Improved message design
- Change waterfall colors
- Fix somes click on strong signal
- Fix possibly missing sign dit or dah in CW

Please refer to the user manual !<br>
Noise reduction and the notch is accessed using the FILTER button.<br>
There has been a slight redesign of the code and there may be a glitch.<br>
The calibration hasn't changed, so if you have a problem, revert to the previous version and do a factory reset.

From older vertions:
- Change the fft hanning filter (<b>RSSI calibration will need to be redone</b> It is dependent on the fft !)
- Add fft magnetude correction
- Active pass-through filter for frequencies below 3 MHz (for swl)
- Change Aux-Level max: 200 to 400
- Change DIG HiPass: 3000 to 3200
- Fixed SSB voice call and CW message call that could call outside of ham radio bands
- Fixed FM modulation
- Change Agc Medium: 600 to 1000mS
- Change method to compute waterfall and fft display
- Add RX only mode (Press and hold M.V)
- Add serial number in the first menu item
- Change the noise reducer with a Kalman filter, adapted to voice
- Change key to activate reducer ! (press AF)
- Change AF in ranges 0-63 to fine tune, especially headset
- Add bass and treble control for speaker
- Add bass and treble control for microphone in AM, FM, SSB

The zip file contains three files:
- FX-4CR-V2-R.hex: firmware to be flashed with ”STM32CubeProg” under Windows.
- FX-4CR-V2-R.bin: firmware to be flashed with “dfu-util” under Linux.
- FX-4CR-User-Manual (V2.xx-R).pdf: user and maintenance manuals included.


## Revision "V" Radio
[FX-4CR-V2-V-25-02-19.zip](https://github.com/user-attachments/files/19410620/FX-4CR-V2-V-25-02-19.zip)
+ User manual update and warning regarding keyer and mic ports
+ Add user manual
+ Change in SSB and transmission bandwidth 300-2700 Hz

[FX-4CR-V2-V-25-01-27.zip](https://github.com/user-attachments/files/19410621/FX-4CR-V2-V-25-01-27.zip)
- Fixed an inconsistent power level
- Fixed Screen error, sometimes the screen appears to be shifted by several lines.

As promised, this version lets you record a voice message of up to 10 seconds and play it back in a loop.
I've merged the user and service manuals into a single document.
The zip file contains three files:
- file.hex: firmware to be flashed with ”STM32CubeProg” under Windows.
- file.bin: firmware to be flashed with “dfu-util” under Linux.
- file.pfd: radio manual.
