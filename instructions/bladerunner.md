## Fastboot installation

```
1. Unlock your bootloader(if not done before), and in bootloader mode follow the next command
2. fastboot update aospa-uvite-*-bladerunner-*-image.zip
3. After the reboot, factory reset the device (only required for the first time you flash Paranoid Android)
```

## Recovery installation

```
1. Unlock your bootloader(if not done before)
2. Reboot your device to TWRP recovery (adb reboot recovery)
3. Select "Install" and choose the corresponding rom zip
4. After flashing, select "Wipe", then "Format data" to factory reset the device (only required for the first time you flash Paranoid Android)
```

**Requirements**:

*Firmware version*: realmeUI 3.1 Stable. (RMX2071_11_F.20/RMX2075_11_F.17/RMX2076_11_F.17)
