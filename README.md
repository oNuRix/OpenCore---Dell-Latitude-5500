# OpenCore Dell Latitude 5500

<img width="324" height="588" alt="taheo" src="https://github.com/user-attachments/assets/528c1ef5-ee80-48e5-a08d-1fd8c1560f82" />

## Specs

| Specifications | Detail                                                  |
| ------------------- | ------------------------------------------- |
| Computer model      | Dell Latitude 5500     |
| Processor           | Intel Core i7-8665U   |
| Memory              | 32GB (2X16) 2666 DDR4 |
| NVME                | M.2 Nvme WD_BLACK SN770 500GB| 
| Integrated Graphics | Intel UHD Graphics 620 |
| Monitor             | FHD (15.6" 1920 × 1080) |
| Wireless Card       | Intel AX200 / BCM94360CS2|

## Wifi
- BCM94360 only bluetooth work on taheo. wifi/blueetoth/airdrop working on sequoi.
- ax200 only working with itlwm kext and bluetooth not stabel!
  
## Misc before install:

- Don't forget too change SMBIOS!
- [Gensmbios](https://github.com/corpnewt/GenSMBIOS) (better if you know MAC address for rom section in OC)
- [Unlock CFG ](https://dortania.github.io/OpenCore-Post-Install/misc/msr-lock.html#turning-off-cfg-lock-manually)

## BIOS Setting Recommended:
- General:
- UEFI Boot Path Security: Never
- System Configuration:
- Integrated NIC: Enabled (Not Enabled w/PXE)
- SATA Operation: AHCI
- SMART Reporting: Enable SMART Reporting
- Miscellaneous Devices: Enable Camera, Enable Secure Digital Card
- MAC Address Pass-Through: Disabled
- Secure Boot:
- Secure Boot Enable: Disable Secure Boot
- Power Management:
- Lid Switch: Enable Lid Switch
- USB Wake Support: Disable Wake on Dell USB-C Dock
- Wake on LAN: Disabled
- Virtualization Support:
- Virtualization: Enable Intel Virtualization Technology
- VT for Direct I/O: Enable VT for Direct I/O

## Trim
- For ssd healt you can typ " sudo trimforce enable " after macos installed.

## Not Wworking
- Dedicated brightness control keys (use Fn+S/Fn+B instead)
- HDMI coldplug (hotplug is OK)
- Audio (partiel)

## THANKS
- [msbence](https://github.com/msbence)

