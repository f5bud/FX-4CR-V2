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
>[!NOTE]
First, consider this a beta test because there have been some important corrections.<br>
The RSSI calibration needs to be redone because one of the corrections concerns the ADC data.<br>
This results in an improvement in dynamics.

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
