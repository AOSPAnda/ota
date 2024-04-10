## Fastboot installation

```
1. Unlock your bootloader(if not done before), and in bootloader mode follow the next command
2. fastboot update aospa-uvite-*-oneplus9-image.zip
3. After the reboot, factory reset the device (only required for the first time you flash Paranoid Android)
```

## Recovery installation

```
1. Reboot your device to recovery (adb reboot recovery)
2. Select "Apply update from ADB"
3. Pass the command "adb sideload aospa-uvite-*-oneplus9.zip
3. After flashing, factory reset the device (only required for the first time you flash Paranoid Android)
```

**Requirements**:

*Firmware version*: OOS 14 Stable. (14.0.0.202/14.0.0.211)
