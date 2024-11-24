# opencore(hackintosh) work for Qiyida X99-D4 motherboard
## SEE (OpenCore-20241124)[./OpenCore-20241124] folder instead
~~
# currently nothing works
### more details
- huananzhi x99-f8 bios booted(current efi)
- stock bios doesnt(stuck at exitbs while csm disabled and bootloop while csm is set to uefi only)
- since x99-f8's bios have the different device(pci) path, causing nic, sata, nvme ports are not working properly
- tried some bios modify tools like MMTools, AMIBCP,... to compare different bios settings between x99-f8 but they are same
- 
### what to do now?
- search for solution if device path can be modify -> modify x99-f8's bios device path to match the stock bios
- using the stock bios, try apply some kernel patches
~~
