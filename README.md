# Marlin 3D Printer Firmware for Anycubic Vyper
![GitHub](https://img.shields.io/github/license/marlinfirmware/marlin.svg)
<img align="right" width=175 src="buildroot/share/pixmaps/logo/marlin-250.png" />

Additional documentation can be found at the [Marlin Home Page](https://marlinfw.org/).
Please test this firmware and let us know if it misbehaves in any way. Volunteers are standing by!

## Downloads
At present there are no binary downloads since the STM license conditions for some of the libraries used restrict execution to STM devices only, the Vyper mainboard uses a non-STM device.
You may take this source and build for your board but it is your responsibility to ensure it is running in accordance with the license conditions.

## Releases
| Version | Marlin Version | Description                                                                                                                                                                                                                                                                                                                                                     |
|:-------:|:--------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|  0.1.0  |     2.0.8      | Official Anycubic version in which the following features have been activated: <br> - `Linear Advance` <br> - `SD_CHECK_AND_RETRY` <br> - `FAN_KICKSTART_TIME`  <br> - `PROBE_OFFSET_WIZARD`  <br> - `PROBE_OFFSET_WIZARD_XY_POS`  <br> - `STATUS_MESSAGE_SCROLLING` <br> - `SCROLL_LONG_FILENAMES` <br> - `HOST_ACTION_COMMANDS` <br> - `HOST_PROMPT_SUPPORT` <br> - `CANCEL_OBJECTS` |

## Building Marlin 2.0
To build Marlin 2.0 you'll need [Arduino IDE 1.8.8 or newer](https://www.arduino.cc/en/main/software) or [PlatformIO](https://docs.platformio.org/en/latest/ide.html#platformio-ide). We've posted detailed instructions on [Building Marlin with Arduino](https://marlinfw.org/docs/basics/install_arduino.html) and [Building Marlin with PlatformIO for ReArm](https://marlinfw.org/docs/basics/install_rearm.html) (which applies well to other 32-bit boards).

## Linear Advance
### General
Linear Advance is enabled in this firmware but disabled by setting the K Value to "0". You have to determine the K value and save it on the EProm via e.g. Pronterface. 

### Calibration
There is a K-factor calibration guide for Linear Advanced available from Marlin which can be found here:
[K-factor Calibration Pattern](https://marlinfw.org/tools/lin_advance/k-factor.html)


## License
Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
