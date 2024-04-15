## Firmware

[Download Android 12 BSP lnxbuild](https://t.me/Edward_ROMs/138)

- If you get hard brick, you can use Android 12 lnxbuild EDL firmware to unbrick.
- Install Android 12 lnxbuild as firmware.

## First time install AOSPA

#### WARNING
I will recommand use "Fastboot installation" to install Paranoid Android
because Qualcomm Reference Devices slot b are always be empty when you using lnxbuild.

1. Download AOSPA images ROM on Our website.
2. Open terminal / cmd / powershell ...etc on your PC.
3. Place fastboot platform tools in same folder.
4. Reboot to bootloader via `adb reboot bootloader` (if you're not already in it).
5. Execute this command: fastboot update aospa-_lahaina_-image.zip
6. Reboot to recovery via fastboot reboot recovery.
7. Select Wipe data/factory reset & confirm.
8. Reboot to system via adb reboot.

## OTA in AOSPA

1. Download AOSPA recovery ROM on Our website.
2. Install Copy-partitions in AOSPA Recovery. [Download Here](https://mirrorbits.lineageos.org/tools/copy-partitions-20220613-signed.zip)
3. select Apply Update from ADB.
4. Execute this command: `adb sideload aospa-*lahaina*.zip`
5. After the installation is completed, reboot to system via adb reboot.
