# Introduction #

The EiBotBoard (used in the initial Egg-Bot Kit contains a Microchip PIC 18F46J50 microcontroller. This page describes the steps necessary to build that firmware.

# Tools Needed #

  * Windows PC, Linux PC, or Mac OS PC (anything that can run MPLAB X and the C18 conpiler)
  * Latest version of MPLABZ (v2.0 or above) free from http://www.microchip.com/MPLABX
  * Latest version of Microchip's MPLAB C Compiler for PIC 18 MCUs (formerly "C18") , v3.35 or above free from http://www.microchip.com/C18 - the free versions (LITE or standard-eval) work just fine
  * Latest version of EiBotBoard source - https://eggbotcode.googlecode.com/svn/trunk/EBB_firmware
  * To reprogram your EiBotBoard, you need the HIDBootloader.exe application http://eggbotcode.googlecode.com/svn/trunk/EBB_firmware/BootloaderPCapp/BootloaderPCapp.zip (Or download the latest MLA from www.microchip.com/MLA, install it, and then look at the path C:\microchip\_solutions\_v2013-06-15\USB\Device - Bootloaders\HID\Software Windows Executable - also note that there is a cross platform executable in the HID directory one levell up.)

# Details #

  * Install MPLABX and C18
  * Check out the EBB\_firmware folder from this project's SVN repository
  * Open MPLAB X
  * From the File->Open Project menu in MPLAB X, go to the EBB\_firmware folder and double click on the app.X folder, which will open up the firmware project.
  * You also need to open the bootloader project at the same time, so to File->Open Project and double click on bootloader.X. You should now have both app ("EBF\_EBBv13\_and\_above") and bootloader ("EBBv11\_BL") projects open in MPLAB X.
  * For the EBF\_EBBv13\_and\_above project, make sure to choose the EBBv13\_with\_bootloader configuration, and for the EBBv11\_BL project, make sure you have selected the 46J50 configuration.
  * Right click on the EBF\_EBBv13\_and\_above in the Projects window and select "Build".
  * It should build with just one warning. (Even the free version of C18, without any optomizations, should still allow the code to fit just fine.)
  * In \EBB\_firmware\app.X\dist\EBBv13\_with\_bootloader\production you will find a file called app.X.production.hex which is the HEX output file from the build for the application. This is what you'll program into the EBB using the bootloader.
  * With your EiBotBoard connected to your PC, press and hold the PRG button while pressing and releasing the RESET button. This will put the board into bootloader mode. The two LEDs (red/green) should be blinking back and forth when it's in bootloader mode.
  * Run the HIDBootloader.exe application. It should say "Device attached."
  * Click Open Hex File and navigate to the HEX file you just created.
  * Click Program/Verify, and wait until it is complete (only about 2 seconds)
  * Click Reset Device, and enjoy your fresh-built firmware!
  * One thing to try is to change the version number (in UBW.c, about line 137), recompile, download, and use the "V" command to see if your new version number has taken effect.