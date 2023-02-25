# i7-13700F + RX6600 Hackintosh-OpenCore

<p align="center">
  <img src="https://i.imgur.com/Iocdsfe.png" alt="Specs">
</p>

## Shopping list

 - [x] MBO: [GIGABYTE B660M DSH3 DDR4 with BIOS Version F21](https://www.gigabyte.com/Motherboard/B660M-DS3H-DDR4-rev-10#kf)
 - [x] CPU: [Intel® Core™ i7-13700F 2.1 GHz Box with stock cooler included](https://www.intel.com/content/www/us/en/products/sku/230491/intel-core-i713700f-processor-30m-cache-up-to-5-20-ghz/specifications.html)
  - [x] GPU: [PULSE AMD Radeon™ RX 6600](https://www.sapphiretech.com/en/consumer/pulse-radeon-rx-6600-8g-gddr6)
  - [x] RAM: [Kingston FURY™ Beast DDR4 3200MHz, 2 x 32GB kits](https://www.kingston.com/en/memory/gaming/kingston-fury-beast-ddr4-memory)
  - [x] SSD: [SAMSUNG 980 PRO PCIe® 4.0 NVMe™ SSD 1TB](https://www.samsung.com/us/computing/memory-storage/solid-state-drives/980-pro-pcie-4-0-nvme-ssd-1tb-mz-v8p1t0b-am/)
  - [x] PSU: [Aerocool LUX 80+ Bronze 750W](https://aerocool.io/product/lux-750w/)
  - [x] Case: [Segotep Halo 5 Black](https://www.segotep.com/En/product_show.aspx?id=183)
  - [x] Display: [SAMSUNG 34" Ultra WQHD Monitor with 21:9 Wide Screen](https://www.samsung.com/ca/monitors/ultra-wide/ultra-wqhd-monitor-with-21-9-wide-screen-34-inch-ls34j552wqnxza/)
  - [x] Keyboard & Mouse: [logitech MK220 Compact Wireless Keyboard and Mouse combo](https://www.logitech.com/en-eu/products/combos/mk220-compact-keyboard-mouse.920-003168.html)

## What's Working
 - [x] Audio & microphone jacks: front panel and motherboard
 - [x] CPU Speedstep (XCPM)
 - [x] Fully Functional QE/CI Enabled Graphics
 - [x] Ethernet
 - [x] HDMI + Audio
 - [x] Usb 3.0 + Usb 2.0 + Type C + Front panel case Usb
 - [x] Native hotkey support with Fn keys
 - [x] Sleep
 
## Kexts used

- **Audio** : It supported using `AppleALC.kext` and `layout-id 12`

- **CPU** : Working using `VirtualSMC.kext` and `Lilu.kext`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`Cpuid1Data` to `55060A00 00000000 00000000 00000000` or in TextEdit `VQYKAAAAAAAAAAAAAAAAAA==`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`Cpuid1Mask` to `FFFFFFFF 00000000 00000000 00000000` or in TextEdit `/////wAAAAAAAAAAAAAAAA==`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`ProvideCurrentCpuInfo` to `true`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`MinDate` and `MinVersion` to `-1`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`HideAuxiliary` to `false`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`DmgLoading` to `Any`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`SecureBootModel` to `Disabled`
- **Graphics** : Working using `WhateverGreen.kext`

- **USBs** : Custom generated. Supported using `USBToolBox.kext` + `UTBMap.kext`

- **Ethernet** : 2.5 Gigabit Ethernet using `LucyRTL8125Ethernet.kext`.

- **HDMI** : Working using `WhateverGreen.kext`.

- **NVME** : Working using `NVMeFix.kext`.

## Installation

###  Basic Installation

- Create a Bootable USB for MacOS by using [USB Installation Guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/mac-install.html)
- Copy **ALL** the Contains of this Repo inside the EFI partition of USB

### Post Installation

- Copy **ALL** the Contains of this Repo inside the EFI partition of Hard Drive where you installed the OS
