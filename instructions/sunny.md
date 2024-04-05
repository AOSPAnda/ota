## Firmware installation

1. Download MIUI firmware version V14.0.8.0.SKGMIXM and extract it.
2. Reboot to bootloader via `adb reboot bootloader`.
3. Open a terminal / command prompt in firmware-update directory and execute the following commands to flash the firmware:
```
fastboot flash abl_a abl.img
fastboot flash abl_b abl.img
fastboot flash aop_a aop.img
fastboot flash aop_b aop.img
fastboot flash bluetooth_a bluetooth.img
fastboot flash bluetooth_b bluetooth.img
fastboot flash cmnlib64_a cmnlib64.img
fastboot flash cmnlib64_b cmnlib64.img
fastboot flash cmnlib_a cmnlib.img
fastboot flash cmnlib_b cmnlib.img
fastboot flash devcfg_a devcfg.img
fastboot flash devcfg_b devcfg.img
fastboot flash dsp_a dsp.img
fastboot flash dsp_b dsp.img
fastboot flash hyp_a hyp.img
fastboot flash hyp_b hyp.img
fastboot flash imagefv_a imagefv.img
fastboot flash imagefv_b imagefv.img
fastboot flash keymaster_a keymaster.img
fastboot flash keymaster_b keymaster.img
fastboot flash modem_a modem.img
fastboot flash modem_b modem.img
fastboot flash qupfw_a qupfw.img
fastboot flash qupfw_b qupfw.img
fastboot flash tz_a tz.img
fastboot flash tz_b tz.img
fastboot flash uefisecapp_a uefisecapp.img
fastboot flash uefisecapp_b uefisecapp.img
fastboot flash xbl_a xbl.img
fastboot flash xbl_b xbl.img
fastboot flash xbl_config_a xbl_config.img
fastboot flash xbl_config_b xbl_config.img
```

## Fastboot installation

1. Click on the Fastboot Option to download the Fastboot ROM of AOSPA.
2. Reboot to bootloader via `adb reboot bootloader` (if you're not already in it).
3. Execute this command: `fastboot update aospa-*sunny*-image.zip`
4. Reboot to recovery via `fastboot reboot recovery`.
5. Select Wipe data/factory reset & confirm.
6. Reboot to system via `adb reboot`.

## Recovery installation

1. Click on the Recovery Option to download the Recovery ROM of AOSPA.
2. Download the recovery zip from [here](https://drive.google.com/file/d/1NjU0L4q-O5jvWR-Qu3Mw5YyLdssSz7R6/view?usp=sharing).
3. Execute this command: `fastboot update recovery-AOSPA-*.zip`
4. Ignore `fastboot: error: could not load ’system.img’: No such file or directory`
5. Reboot to recovery via `fastboot reboot recovery`.
6. Select Wipe data/factory reset & confirm.
7. Go back and select Apply Update from ADB.
8. Execute this command: `adb sideload aospa-*sunny*.zip`
9. After the installation is completed, reboot to system via `adb reboot`.


## Requirements
1. Android USB drivers installed via Windows Update.
2. Platform Tools r31.0.3 from [here](https://dl.google.com/android/repository/platform-tools_r31.0.3-windows.zip). (Replace -windows with -linux or -darwin to get platform tools for linux or macOS)
3. Unlocked bootloader.

## Keep in mind
1. DO NOT try to change the included kernel unless it is an update to the kernel that is shipped.
2. Dynamic partitions (system,system_ext,vendor,odm,product) are Read-Only (restricts making changes to overlays, system APKs, etc).
3. DO NOT USE any other recovery than AOSPA recovery which is included.
4. YOU MUST format data with provided AOSPA recovery.
5. YOU MUST CLEAN FLASH if coming from any other ROM or MIUI.
6. If you face issues like poor RAM management or storage issues, you have not followed the instructions and/or have changed the kernel/recovery. STRICTLY follow the provided instructions again before reporting any issues.
7. Formatting with AOSPA recovery (yes, I mean AOSPA recovery ONLY) is a MUST when you clean flash.
