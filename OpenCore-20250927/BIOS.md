# HOW TO FLASH BIOS

## DISCLAIMER

FLASHING BIOS AT YOUR OWN RISKS. ALWAYS HAVE A BACK UP OF YOUR ORIGINAL BIOS.

## STEP 1: BACKUP YOUR STOCK BIOS

- Go to the `FPT` folder.
- Run `dump.bat` with administrator privileges.
- This will create a file named `stock.rom`. Keep this file in a safe place.

## STEP 2: FLASH THE NEW BIOS

- Make sure you are in the `FPT` folder.
- Run `flash.bat` with administrator privileges.
- This will flash the `BOOTSECURE-TPM-152-QD4C612SPSJWAGNERVAZ.rom` file.
- Wait for the process to complete, and then reboot your system.

## STEP 3: BIOS CONFIGURATION (FOR OPENCORE)

After flashing the BIOS, you need to configure it for OpenCore to work correctly.

- **Advanced**

  - **Trusted Computing** > **Security Device Support**: `Disable`
  - **Super IO Configuration** > **Serial Port**: `Disable`
  - **CSM Configuration** > **CSM Support**: `Enable`, **Boot option filter**: `UEFI only`
  - **USB Configuration** > **XHCI Hand-off**: `Enable`, **EHCI Hand-off**: `Enable`
  - **PCI Subsystem Settings** > **Above 4G Decoding**: `Enabled`, **Re-Size BAR Support**: `Disabled`
    - _Note: Re-Size BAR Support depends on your GPU. If you encounter panics during boot, try enabling this option._

- **IntelRCSetup**

  - **Processor Configuration** > **MSR Lock Control**: `Disable`
  - **IIO Configuration** > **Intel VT for Directed I/O (VT-d)**: `Disable`

- **Security**
  - **Secure Boot menu** > **Secure Boot**: `Disabled`, **Secure Boot Mode**: `Standard`

When you have configured these settings, save the changes and reboot. You are now ready to boot the OpenCore installer.
