# B660M-DS3H-DDR4 + i7-13700F + RX6600 Hackintosh-OpenCore

<p align="center">
  <img src="https://i.imgur.com/vg76lIJ.png" alt="Specs">
</p>

## Shopping list

 - [x] MBO: [GIGABYTE B660M DS3H DDR4 with BIOS Version F21](https://www.gigabyte.com/Motherboard/B660M-DS3H-DDR4-rev-10#kf)
 - [x] CPU: [Intel® Core™ i7-13700F 2.1 GHz Box with stock cooler included](https://www.intel.com/content/www/us/en/products/sku/230491/intel-core-i713700f-processor-30m-cache-up-to-5-20-ghz/specifications.html)
  - [x] GPU: [PULSE AMD Radeon™ RX 6600](https://www.sapphiretech.com/en/consumer/pulse-radeon-rx-6600-8g-gddr6)
  - [x] Wifi/Bluetooth	Asus AX3000 Dual Band PCI-E WiFi 6 / Bluetooth 5.0
  - [x] RAM: [Kingston FURY™ Beast DDR4 3200MHz, 2 x 32GB kits](https://www.kingston.com/en/memory/gaming/kingston-fury-beast-ddr4-memory)
  - [x] SSD: [WD_BLACK SN850X NVMe™ 1TB SSD](https://www.westerndigital.com/en-ap/products/internal-drives/wd-black-sn850x-nvme-ssd#WDS100T2X0E)
  - [x] PSU: [Aerocool LUX 80+ Bronze 750W](https://aerocool.io/product/lux-750w/)
  - [x] Case: [Segotep Halo 5 Black](https://www.segotep.com/En/product_show.aspx?id=183)
  - [x] Display: [SAMSUNG 34" Ultra WQHD Monitor with 21:9 Wide Screen](https://www.samsung.com/ca/monitors/ultra-wide/ultra-wqhd-monitor-with-21-9-wide-screen-34-inch-ls34j552wqnxza/)
  - [x] Keyboard & Mouse: [logitech MK220 Compact Wireless Keyboard and Mouse combo](https://www.logitech.com/en-eu/products/combos/mk220-compact-keyboard-mouse.920-003168.html)

## What's Working
 - [x] Audio & microphone jacks: front panel and motherboard
 - [x] CPU Speedstep (XCPM)
 - [x] Fully Functional QE/CI Enabled Graphics
 - [x] Ethernet + WiFi + Bluetooth
 - [x] HDMI + Audio
 - [x] Usb 3.0 + Usb 2.0 + Type C + Front panel case Usb
 - [x] Native hotkey support with Fn keys
 - [x] Sleep
 
## Kexts used

- **Audio** : Realtek `ALC897` with Revision Id `0x100402` It supported using `AppleALC.kext` and `layout-id 12`

- **CPU** : Working using `VirtualSMC.kext` and `Lilu.kext`

- **Graphics** : Working using `WhateverGreen.kext`

- **USBs** : Custom generated. Supported using `USBToolBox.kext` + `UTBMap.kext`

- **Ethernet** : 2.5 Gigabit Ethernet using `LucyRTL8125Ethernet.kext`.

- **HDMI** : Working using `WhateverGreen.kext`.

- **NVME** : Working using `NVMeFix.kext`.

## Installation

### Download link for macrecovery
python3 macrecovery.py -b Mac-7BA5B2D9E42DDD94 download

###  Basic Installation

- Create a Bootable USB for MacOS by using [USB Installation Guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/mac-install.html)
- Copy **ALL** the Contains of this Repo inside the EFI partition of USB

### Post Installation

- Copy **ALL** the Contains of this Repo inside the EFI partition of Hard Drive where you installed the OS
