# unit_ut61eplus
Access UNI-T UT61E+ Digital Multimeter from Python via CP2110 / CH9329 based USB HID Device 
**NOTE:** It seems newer UNI-T UT61x DMMs come with a `CH9329` based HID->UART Adapter.
This project now detects both and automatically chooses which VID/PID to use


This Project should work also for other models, but with adjustments for the unit conversion.
(See `from_vendor/*.json`)
* UT60BT
* UT61B+
* UT61D+
* UT161B
* UT161D
* UT161E

## Status
> Working with Linux. Patches/Documentation for Windows is welcome
> Tested with UT61E+ and UT61B+


## Example Output From readDMM.py
```
Opened: VID=0x1A86, PID=0xE429
mode=DCV
range=0
display=0.0002
display_decimal=0.0002
display_unit=V
overload=False
value=0.0002
unit=V
isMax=False
ismin=False
isHold=False
isRel=False
isAuto=True
hasBatteryWarning=False
hashasHVWarning=False
isDC=False
isMaxPeak=False
```
