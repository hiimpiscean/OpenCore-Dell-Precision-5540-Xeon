# OpenCore Dell Precision 5540

## Images

![Screen Shot 2023-06-22 at 21 43 15](https://github.com/hiimpiscean/OpenCore-Dell-Precision-5540-Xeon/assets/106610508/a3bdbaef-b0e2-4610-b0ac-3b0fb316e3a9)

![Screen Shot 2023-06-22 at 21 44 59](https://github.com/hiimpiscean/OpenCore-Dell-Precision-5540-Xeon/assets/106610508/ad94e39d-e5fb-4892-98ef-72256582d06e)

## Configuration

| Specifications | Details                                                  |
| ------------------- | ------------------------------------------- |
| Computer model      | Dell Precision 5540      |
| Processor           | Intel Xeon E-2276M, 6 cores  |
| RAM                 | 16GB (1x16GB) 2666MHz, upgradable to 64GB |
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
- **Apple TV+ not working due to dGPU not supported**
- Everything else works, except Airdrop.
- Audio patched and working correctly.
- Ensure to edit the **config.plist** and add valid  **PlatformInfo Generic** and **SMBIOS** values.
- Find your's screen IODisplayEDID in ioreg and add AAPL00,override-no-connect in deviceProperties.

## To-do

- Check TB3 port (no device to test)
