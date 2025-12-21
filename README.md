# rtl8733bs-20250521

Linux Driver for RTL8731BS and RTL8733BS v5.15.17-113-g1924716b3.20250521, mainly modified for FPV  

Features: see [rtl8733bu-20230626](https://github.com/libc0607/rtl8733bu-20230626) (same chip, different package & interface)  
Installation: see [rtl88x2eu driver installation](https://github.com/libc0607/rtl88x2eu-20230815?tab=readme-ov-file#installation)  
Original driver: [rtl8733BS_WiFi_linux_v5.15.17-113-g1924716b3.20250521_COEX20241204-390f.tar.gz](https://github.com/user-attachments/files/20839055/rtl8733BS_WiFi_linux_v5.15.17-113-g1924716b3.20250521_COEX20241204-390f.tar.gz)  
Release note: [ReleaseNotes.pdf](https://github.com/user-attachments/files/20839065/ReleaseNotes.pdf)  

## Use with OpenIPC
See [Platform Compatibilities](https://github.com/libc0607/rtl8822cs-20240221?tab=readme-ov-file#platform-compatibilities) for hardware connection & driver installation.  
The output of `find /sys/bus/sdio/devices/* | xargs -I {} cat {}/uevent | grep "SDIO_ID=" | cut -d= -f2` (On OpenIPC SSC338Q) is `024C:B733`.  

## Open Source Hardware
Module datasheet: [BL-M8731BS3_datasheet_V1.0.1.0.pdf](https://github.com/user-attachments/files/20839077/BL-M8731BS3_datasheet_V1.0.1.0_231020.70004020.pdf)  
Buy from Taobao: [RTL8731BS modules](https://shop73266465.taobao.com/search.htm?keyword=8731bs) or [RTL8733BS modules](https://shop73266465.taobao.com/search.htm?keyword=8733bs)  
(RTL8733Bx = RTL8731Bx + Bluetooth; As Bluetooth is not used in FPV, both are OK)  
For reusing chips from dismantled Wi-Fi modules, check my schematic [here](https://github.com/user-attachments/files/24271068/SCH_RTL873xBS_demo_2025-12-20.pdf) (**USE IT AT YOUR OWN RISK -- It works in my test, but it's NOT the official design**)  
