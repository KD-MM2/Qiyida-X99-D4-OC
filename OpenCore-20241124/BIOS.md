# HOW TO FLASH BIOS

## STEP 1: DISABLE BIOS (FLASH) LOCK
- Reboot, then enter BIOS setup using F11 or DEL key
- Navigate to IntelRCSetup > PCH Configuration > Security Configuration > Disable all settings
- Reboot, then download [FPT.zip](./FPT.zip) and extract it
- Bios file already in FPT folder, so don't need to find or download
- Run `flash.bat` with admin privilege
- Wait until done then reboot

## STEP 2: BIOS CONFIGURATION(FOR OPENCORE)
- SATA Mode	AHCI
- Secure Boot	Disabled	
- Serial/COM Port	Disabled
- Compatibility Support Module (CSM):
```
Boot option filter: UEFI Only
Storage: UEFI
Video: UEFI
Other PCI devices: UEFI
```
- Intel Virtualization Technology for Directed I/O (VT-d)	Disabled
- Above 4G Decoding / Above 4G memory	Enabled
- Execute Disable Bit	Enabled
- EHCI/XHCI Hand-off	Enabled
- MSR Lock Control	Disabled

When done, reboot and you are ready to boot the Installer.