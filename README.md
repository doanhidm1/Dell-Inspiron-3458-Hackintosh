# <div align="center">Dell Inspiron 3458 Hackintosh</div>

<div align="center">

![Screenshot](https://cdn.discordapp.com/attachments/636786976556711946/1105794008476815460/image.png)
   
</div>

## Thông tin cơ bản
|Danh mục|Phiên bản|
|:---:|:----:|
|OpenCore| 0.9.2|
|macOS|12.6.5 Monterey|


## Thông Tin Laptop
 
|Danh mục| Thông số kĩ thuật | Kext |
| - | - | - | 
| `CPU`| Intel Core i3-4005U Haswell | - VirtualSMC <br> - SMCProcessor <br> - SMCDellSensors <br> - SMCSuperIO | Lilu |
| `RAM`| 1 x 4GB + 2 x 8GB DDR3| Không cần |
| `GPU`| Intel HD Graphics 4400 | WhateverGreen | Lilu
| `Storage`| SSD WD SATA 2.5 500GB | Không cần |
| `Card Reader`| Realtek Card Reader | ? |
| `Ethernet`| RJ45 RTL8106E Realtek | RealtekRTL8100 |
| `WiFi`| Intel(R) Dual Band Wireless-AC 3160 | AirportItlwm |
| `Bluetooth`| Intel(R) Wireless Bluetooth |  - IntelBluetoothFirmware <br> - BlueToolFixup
| `Âm thanh`| Realtek ALC255 (ALC3234) | AppleALC (86) |
| `Bàn phím + Chuột`| PS/2 Mouse/Keyboard |VoodooPS2Controller |
| `Touchpad`| Synaptics Dell Touchpad | VoodooI2CSynaptics |
| `Pin`| 40Wh Lithium-ion | SMCBatteryManager |
| `USB` | 2x USB 2.0 + 1x USB 3.0 | - USBToolBox.kext <br> - UTBDefault|

## Những gì hoạt động ?

| Danh mục | Hoạt động ?| Ghi chú|
| - | :-: | - |
| `Wifi`|✅| Chỉ có wifi, không có Airdrop. Chưa test các chức năng khác |
| `Loa`|✅| Cả loa ngoài và jack 3.5 đều hoạt động|
| `Bàn Phím`|✅|Phím Windows -> Command, Alt -> Control. Điều chỉnh độ sáng bằng Fn+B / Fn+S|
| `Mic`|✅|Cả loa ngoài và jack 3.5 đều hoạt động|
| `Đồ hoạ`|✅|Tăng tốc phần cứng đầy đủ|
| `Pin`|✅|Có đọc được nhưng độ chính xác ko rõ|
| `Đầu Đọc Thẻ`|❌|Chưa có thẻ để test|
| `Webcam`|✅|
| `Touchpad`|✅|Bị ngược chiều|
| `Chuột`| ✅ | Bị ngược chiều | 
| `Webcam`|✅||
| `USB Port`|✅|Nên map usb|
| `Sleep`|❌|Map usb rồi tự kiểm tra|
| `Ethernet`|✅||
| `Bluetooth`|✅|Khi kết nối với Iphone thì không hỗ trợ, các thiết bị khác ok|


## Thiết lập cần thiết
- BIOS: <br>
    1. Bootmode: UEFI
    2. Storage Controller: AHCI
    3. Update lên BIOS A21
    4. Tắt CFG-lock
- Ổ cứng
    1. Chuẩn: GPT
    2. Đã tắt Raid
    3. \>=200 MB phân vùng EFI (FAT32) và >= 30gb phân vùng trống cho MacOS 

## Dùng EFI Thế Nào ?

## Cảm Ơn

