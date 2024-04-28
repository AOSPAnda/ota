## For clean flash/from MIUI/any other ROM

- Download the recovery zip
- Take a backup
- Connect phone to PC
- Reboot into fastboot:
`adb reboot bootloader`
- Flash the recovery image from [here](https://drive.usercontent.google.com/download?id=1MDQSRVFitD3KeL_RnBD5BnuQhGsyMD4z&export=download)
`fastboot flash recovery-aospa.img`
- Reboot phone to AOSPA recovery:
`fastboot reboot recovery`
- Select "Apply update via ADB" and run:
`adb sideload aospa-uvite-beta-miatoll-***.zip`
- If you're coming from stock or another ROM, wipe data/factory reset is required.
- Reboot to system.

## For updating to a newer build

- Download the recovery zip
- Connect phone to PC
- Reboot phone to AOSPA recovery, using button combo or `adb reboot recovery`
- Select "Apply update via adb" and run:
`adb sideload aospa-uvite-beta-miatoll-***.zip`

### Note:

- Flash latest available firmwares available for your specific models
(Warning: DO NOT FLASH OTHER DEVICE'S FIRMWARE!).
- Custom recoveries (twrp, orangefox etc.) and kernels are not recommended and not supported by me. Do not report issues or bricks to me after using them.
