> Steps to Install MiThoriumSSI ROM

## Install directly to the system via Twrp-Recovery:

1. Download a MiThoriumSSI ROM build in ZIP format.
2. Download Vendor-MiThoriumSSI ZIP for the target device used, find it here: [MiThoriumSSI-Vendor-Archive](https://github.com/Mika-Releases/MiThoriumSSI-Vendor-Archive/releases).
3. Download los_recovery for the target device used, find it here: [Recovery_Archive](https://github.com/Mika-Releases/Recovery_Archive/releases).
4. Extract the MiThoriumSSI ROM ZIP, and find `system.img`.
5. reboot into twrp_recovery
6. wipe system/vendor
7. install Vendor-MiThoriumSSI ZIP.
8. install image `system.img` ,select system
9. install image `los_recovery.img` select recovery
10. reboot to los_recovery & Select `Factory reset` --> `Format data/factory reset`. Your phone will display a message that /data, /cache, and /metadata have been formatted.
11. Reboot and enjoy.

> [!NOTE]
> los_recovery is required to load partition/metadata

## Install directly to the system via bootloader/fastboot:

1. Download a MiThoriumSSI ROM build in ZIP format.
2. Download Vendor-MiThoriumSSI ZIP for the target device used, find it here: [MiThoriumSSI-Vendor-Archive](https://github.com/Mika-Releases/MiThoriumSSI-Vendor-Archive/releases).
3. Extract the MiThoriumSSI ROM ZIP, and find `system.img`.
4. reboot into los_recovery & select "Apply update/install update" --> "choosen from Internal storage"
5. install Vendor-MiThoriumSSI ZIP.
6. reboot to bootloader/fastboot.
7. Connect your phone to a computer.
8. run `fastboot flash system "system.img path"` in your cmd/powershell/terminal and wait until it finishes.
9. Reboot recovery & Select `Factory reset` --> `Format data/factory reset`. Your phone will display a message that /data, /cache, and /metadata have been formatted.
10. Reboot and enjoy.

## Steps to use with Dynamic System Update feature:

1. For devices except Mi439: Flash FDE Encryption Disabler
2. Download a MiThoriumSSI build in ZIP format
3. Install it with "DSU Sideloader" app
4. Click "Restart" on Dynamic System Updates notification
