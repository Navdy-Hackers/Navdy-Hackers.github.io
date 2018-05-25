## How to flash your Navdy to a new firmware

1. Download firmware.  Unzip the package on computer.
2. If you're on windows and haven't used Android ADB or fastboot before, go to `tools\usb_driver` folder inside package and run `dpinst_x64` or `dpinst_x86` to install the usb driver. If you don't know whether your PC is 32 or 64 bit don't worry, try running one and if it doesn't work run the other one.
3. Take your navdy (not plugged into car), hold down the power button and plug it into computer with the micro usb cable in the back. The navdy power light should come on red.
4. On windows, run `FLASH_WIN` to start the upgrade. If there are any errors reported, please reach out to the firmware's author. Mac or Linux does work as well but hasn't been tested as much. You should be able to run `FLASH_OSX_LINUX` script though to start the upgrade. Linux users need to provide their sudo password for it to work.
5. On Windows, if it pops up saying `waiting for any device` it means the drivers have not assigned correctly. See [this video](https://youtu.be/8y6fDrXjEQ4) for instructions on manually assigning the bootloader driver. If you left FLASH_WIN running in the background it should start itself, else re-run it.
6. Once it's done, as long as no errors were reported on the terminal, your navdy should restart and come up on the computer as a flash drive like when plugging it in without holding power button.

*Now you can unplug it and try it in your car!*

**Note: The first time it starts up after flashing normally takes a long time (2 to 5 minutes) on the navdy boot screen. After that it should be back to normal.**

Shamelessly plagarized from [/u/coronafire's reddit posts](https://www.reddit.com/r/navdy/comments/8g6sdi/howto_update_your_display_firmware_and_hack_it/)!
