# BIOS MOD

## FILES & BIOS INFO
- **stock.rom**: dumped from my mobo
    - `X99D4 Ver:001 07/22/2024 17:17:12`
- **stock-mcode-updated.rom**: stock with cpu microcode updated
- **stock-mcode-driver-updated.rom**: stock with cpu microcode and driver updated
```
Manufacturer   - INTEL
Model          - X99-D4
BIOS release   - 5.11 07/22/2024
BIOS version   - 00.01
BIOS platform  - AMI Aptio 5
```

- **qiyidax99d4.rom**: picked from here: https://github.com/Koshak1013/HuananzhiX99_BIOS_mods/issues/116
    - `X99D4 Ver:001 11/01/2023 17:17:12`
- **qiyidax99d4-mcode-updated.rom**: qiyidax99d4 with cpu microcode updated
- **qiyidax99d4-mcode-driver-updated.rom**: qiyidax99d4 with cpu microcode and driver updated
```
Manufacturer   - INTEL
Model          - X99-D4
BIOS release   - 5.11 11/01/2023
BIOS version   - 00.01
BIOS platform  - AMI Aptio 5
```

#### stock.rom cpu microcode
```
╔═══════════════════════════════════════════════════════════════════════════════════════════════════════╗
║                                                 Intel                                                 ║
╟───┬───────────┬───────┬────────────────────┬──────────┬────────────┬───────┬────────┬──────────┬──────╢
║ # │    Type   │ CPUID │     Platforms      │ Revision │    Date    │ State │  Size  │  Offset  │ Last ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 1 │ Microcode │ 306F1 │ EF (0,1,2,3,5,6,7) │ 80000013 │ 2013-10-02 │  PRE  │ 0x8800 │ 0xE938B0 │  No  ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 2 │ Microcode │ 306F2 │  6F (0,1,2,3,5,6)  │    3D    │ 2018-04-20 │  PRD  │ 0x8400 │ 0xE9C0B0 │  No  ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 3 │ Microcode │ 406F0 │ EF (0,1,2,3,5,6,7) │    14    │ 2015-07-02 │  PRD  │ 0x7C00 │ 0xEA44B0 │ Yes  ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 4 │ Microcode │ 406F1 │ EF (0,1,2,3,5,6,7) │ B000038  │ 2019-06-18 │  PRD  │ 0x7800 │ 0xEAC0B0 │  No  ║
╚═══╧═══════════╧═══════╧════════════════════╧══════════╧════════════╧═══════╧════════╧══════════╧══════╝
```

#### stock-mcode-updated.rom cpu microcode
```
╔═══════════════════════════════════════════════════════════════════════════════════════════════════════╗
║                                                 Intel                                                 ║
╟───┬───────────┬───────┬────────────────────┬──────────┬────────────┬───────┬────────┬──────────┬──────╢
║ # │    Type   │ CPUID │     Platforms      │ Revision │    Date    │ State │  Size  │  Offset  │ Last ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 1 │ Microcode │ 406F0 │ EF (0,1,2,3,5,6,7) │    14    │ 2015-07-02 │  PRD  │ 0x7C00 │ 0xE938B0 │ Yes  ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 2 │ Microcode │ 306F1 │ EF (0,1,2,3,5,6,7) │    14    │ 2014-01-10 │  PRD  │ 0x8800 │ 0xE9B4B0 │ Yes  ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 3 │ Microcode │ 306F2 │  6F (0,1,2,3,5,6)  │    49    │ 2021-08-11 │  PRD  │ 0x9800 │ 0xEA3CB0 │ Yes  ║
╟───┼───────────┼───────┼────────────────────┼──────────┼────────────┼───────┼────────┼──────────┼──────╢
║ 4 │ Microcode │ 406F1 │ EF (0,1,2,3,5,6,7) │ B000040  │ 2021-05-19 │  PRD  │ 0x8C00 │ 0xEAD4B0 │ Yes  ║
╚═══╧═══════════╧═══════╧════════════════════╧══════════╧════════════╧═══════╧════════╧══════════╧══════╝
```

#### stock-mcode-driver-updated.rom
```
EFI Intel RST RAID Driver   - 14.8.0.2377
EFI Intel RSTe for sSATA    - 4.5.0.1012 -> 5.5.5.1005
EFI Intel RSTe for SATA     - 4.5.0.1012 -> 5.5.5.1005
OROM Intel RSTe for SATA    - 4.5.0.1012 -> 5.5.5.1005
OROM Intel RSTe for sSATA   - 4.5.0.1012 -> 5.5.5.1005


EFI Realtek UNDI Driver     - 2.053 -> 2.068
EFI Realtek UNDI Driver     - 2.053 -> 2.068
EFI Realtek UNDI Driver     - 2.037 -> 2.068
OROM Realtek 2.5 Gb PXE     - 3.01 -> 3.04
OROM Realtek Boot Agent GE  - 2.66 -> 2.70
```
