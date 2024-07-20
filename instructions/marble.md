## For clean flash/from MIUI/HyperOS/any other ROM

- Take a backup
- In your PC, download and extract the flashing kit from [here](https://github.com/adithya2306/aospa-flashing-kit/archive/refs/heads/marble.zip)
- Follow the steps given in `README.md`, or read [here](https://github.com/adithya2306/aospa-flashing-kit#steps)
- Once all the steps are completed, enter recovery mode
- If you're coming from stock or another ROM, factory data reset is required. Otherwise skip this step if you're coming from Topaz or Uvite Unofficial.
- Reboot to system.

## For updating to a newer build
- Download the fastboot zip and reuse the flashing kit according to the previous steps. Do not wipe data/factory reset.
- Installing firmware again is not mandatory, but you can always update to the latest firmware.

OR

- Download the recovery zip
- Connect phone to PC
- Reboot phone to AOSPA recovery, using button combo or `adb reboot recovery`
- Select "Apply update via adb" and run:  
`adb sideload aospa-uvite-beta-marble-***.zip`

## Note:

- Firmware flash is required only for the first time flashing Uvite. But you can always update to the latest available firmware if you wish to.
- Custom recoveries (twrp, orangefox etc.) are not recommended and not supported by us. Do not report issues or bricks to us after using them.
