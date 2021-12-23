# Opencore-HP-Omen-15-2020
## Working with macOS 12.1 (21C52)
Opencore config files for HP Omen 15 2020 10750H

~~Battery life the best I can get for this machine is around 1h and 20 min~~

Battery life now has been fixed, backup your serial number if you are using your iMessage/Facetime service

## Specs
* CPU: i7-10750H (~~Emulated as 9750H~~)
* GPU: Intel UHD Graphics + RTX2060

***For other CPU models such as 10300H, 10500H, etc. Go to `DeviceProperties` and replace the old iGPU properties with the following iGPU properties instead (Not guaranteed to work, but worth a try)***

### PciRoot(0x0)/Pci(0x2,0x0)

| Key | Type | Value |
| ------ | ------ | ----- |
| AAPL,ig-platform-id | Data | 0500A63E |
| device-id | Data | A63E0000 |


* Ram: 8gb+8gb
* Audio: ALC245 (layout-id 13)
* Trackpad: Synaptics (syna32a4)
* SSD: PM981a (Replaced with WD Black SN750) ***Hey, this is very important, replace this SSD(PM981a) as it may cause various problem even with [NVMeFix.kext](https://github.com/acidanthera/NVMeFix)***
* WiFi: Intel® Wi-Fi 6 AX201

## What's working
* Everything works except video output since all video ports are connected to nVidia 
* Built-in Mic not working cause it uses Intel® Smart Sound Technology

## CinebenchR23
![Image of Cinebench](https://raw.githubusercontent.com/lunjielee/Opencore-HP-Omen-15-2020/master/cinebench.png)
