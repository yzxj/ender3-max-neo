# ender3-max-neo
Cura and firmware setup for Ender 3 Max Neo printer

## Cura Config
To get the configs I used for cura (Latest: AltTab N0.6)
1. Open Cura
2. In the top bar: Help > Show Configuration Folder
3. This folder should open with a structure like `AppData/Roaming/cura/5.6` where the last folder is your cura version (e.g. 5.6)
4. Close Cura so that changes will work
5. Copy all files/folders `cura/5.6` in this github. Paste it into your cura config
6. Open Cura and see that the printer config (Ender 3 Max Neo) and profile configs should appear
7. It's probably not a perfect config, but should be a good starting point

## Modified firmware
I forked [mriscoc's Ender3V2S1 config](https://github.com/mriscoc/Ender3V2S1):
1. Clone https://github.com/yzxj/Ender3MaxNeo
2. Checkout the ender3maxneo branch
3. In VSCode, set up the extensions "PlatformIO IDE" and "Auto Build Marlin"
4. Try out a build (I'm not sure what's the diff between RE and RC)
5. Put the bin file into your microSD card
   1. Make sure it's the only file there
   2. The name kind of matters, the machine will remember not update if the name repeats
6. Switch off your printer, plug the microSD card in, and switch on the printer. It should start updating.
7. You may need to update the screen firmware, guide [here](https://github.com/mriscoc/Ender3V2S1/wiki/How-to-update-the-display)
8. Troubleshooting tips can be found [here](https://github.com/mriscoc/Ender3V2S1/wiki/How-to-install-the-firmware)
9. If all else fails, you can reset the firmware using files from the [official website](https://www.creality.com/pages/download-ender-3-max-neo)

I've included a sample firmware build here as well. It should be my latest settings, but I don't remember whether the last commit was a working version so I can't be sure if it works 100%.