# OpenCore for Qiyida X99-D4

## Working macOS version: Sequoia 15.x

## BIOS

This EFI is designed to work with a modified stock BIOS. This BIOS is based on the original, but with microcodes, drivers updated and some tweaks to allow OpenCore to boot without issues.

### Credit

The modified BIOS is provided by [jwagnervaz](https://github.com/jwagnervaz). For more details on the BIOS, please visit the repository: [jwagnervaz/QIYIDA-X99-D4-V2.0](https://github.com/jwagnervaz/QIYIDA-X99-D4-V2.0).

### Build specs (setup)

- Qiyida X99-D4 (Chinese mobo: [Review – Qiyida X99-D4 – An Affordable chinese Motherboard for Xeon with White PCB](https://theoverclockingpage.com/2024/04/21/review-qiyida-x99-d4-an-affordable-chinese-motherboard-for-xeon-with-white-pcb/?lang=en))
- Intel Xeon E5-1660v3
- 64GB = 4\*16GB DDR4 2400MHz
- AMD RX570 4GB
- 512GB SATA SSD

### WORKING

- All SATA Ports
- All USB Ports (both USB2 and USB3)
- Onboard Ethernet (Realtek RTL8111)
- Onboard Audio
- M.2 NVME Slot
- Sleep/Wake

### NOT TESTED

- P/S2 Ports (But should works)

### [HOW TO FLASH BIOS & CONFIGURATIONS](./BIOS.md)

## OPENCORE

### PLEASE USE [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) TO EDIT CONFIG.PLIST

### GENERATE NEW SMBIOS, THEN LOOK FOR **ROM** FIELD, REPLACE FIRST 6 DIGITS WITH **0016CB**, EXAMPLE: A0B1C2001122 → 0016CB001122

### SEE [Fixing iMessage and other services with OpenCore](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)
