# OpenCore-Dell-Precision-5540-Xeon


## Configuration

| Specifications | Detail                                                  |
| ------------------- | ------------------------------------------- |
| Computer model      | Dell Precision 5540      |
| Processor           | Intel Xeon E-2276M 6-core  |
| RAM                 | 16GB (1x16gb) 2666MMHz upgradable to 64GB |
| SSD                 | M.2 SATA 256GB WD Blue
| OS                  | macOS Catalina 10.15.7 + Windows 10, Grub bootloader included|
| Integrated Graphics | Intel UHD Graphics 630 / NVIDIA Quadro T2000 (Disabled)      |
| Monitor             | FHD 1920x1080 non-touchscreen (15.6") |
| Sound Card          | Realtek ALC3266 (ALC298)          |
| Wireless Card       | Intel AX201 + Bluetooth |

## Misc before install:
- Unlock CFG: From GRUB: set_var_3 0x6ED 0x00, **will kernel panic if not set**

## Current Status

- OpenCore version: 0.9.3
- **Fingerprint sensor not working**
- Everything else works, except Airdrop.
- Ensure to edit the **config.plist** and add valid  **PlatformInfo Generic** and **SMBIOS** values.
- Find your's screen IODisplayEDID in ioreg and add AAPL00,override-no-connect in deviceProperties.

## To-do

- Fix battery drain issues (not sure if it's battery-related problem)
- Check TB3 port (no device to test)
- Check microphone output port
