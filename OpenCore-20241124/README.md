# OpenCore 1.0.2 for Qiyida X99-D4
## Working macOS version: Sequoia 15.0

## BIOS
### Warning
- STOCK BIOS STUCK AT **EXITBS**(KERNEL PANIC) AND WON'T BOOT.
- TO USE THIS EFI(OR USING OPENCORE), YOU MUST FLASH YOUR BIOS TO HUANANZHI X99-F8 BIOS.
- DUE TO (BIOS) DEVICE PATH DIFFERENTS, SOME DEVICES ARE NOT WORKING.

### DISCLAIMER
- FLASHING BIOS AT YOUR OWN RISKS.
- ALWAYS HAVE A BACK UP OF YOUR ORIGINAL BIOS AND BETTER HAVE A SPI PROGRAMMER(IN CASE YOU BRICKED YOUR BIOS).

### Build specs(setup):
- Qiyida X99-D4 (Chinese mobo: [Review – Qiyida X99-D4 – An Affordable chinese Motherboard for Xeon with White PCB](https://theoverclockingpage.com/2024/04/21/review-qiyida-x99-d4-an-affordable-chinese-motherboard-for-xeon-with-white-pcb/?lang=en))
- Intel Xeon E5-1630v3
- 3\*8GB + 1\*4GB 2133MHz REG ECC
- AMD RX570 4GB
- 512GB SATA SSD
- (optional) WDC-433SU2MBK USB 2.0 11ac\/n\/a(5GHz) WiFi

### WORKING
- SATA1, SATA3 Ports
- USB Ports(both USB2 and USB3)
- 5.1 AUDIO Ports
- M.2, NVME/NGFF Slot (Thanks @narcyzzo for confirmation [here](https://github.com/KD-MM2/Qiyida-X99-D4-OC/issues/1#issuecomment-2508994085))
- PCIE 1x slot

### NOT WORKING
- SATA2, SATA4 Ports
- Ethernet port(NIC)

### NOT TESTED
- P/S2 Ports

### [HOW TO FLASH BIOS & CONFIGURATIONS](./BIOS.md)

## OPENCORE
### Version: 1.0.2
### macOS Version: Sequoia 15.0

### PLEASE USE [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) TO EDIT CONFIG.PLIST
### GENERATE NEW SMBIOS, THEN LOOK FOR **ROM** FIELD, REPLACE FIRST 6 DIGITS WITH **0016CB**, EXAMPLE: A0B1C2001122 → 0016CB001122
### DON'T DISABLE OR REMOVE **Ethernet** in Settings > Network OR YOU WILL NOT ABLE TO USE APPLE SERVICES ↓
### SEE [Fixing iMessage and other services with OpenCore](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)

