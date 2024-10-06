## Custom-WSL-kernel-WiFi-USB
Custom WSL kernel with wifi and usb support

### Features:
- kernel Version: 6.6 compiled from microsoft [source code WSL kernel](https://github.com/microsoft/WSL2-Linux-Kernel)
- USB support
- WIFI support
- rfkill support
- Virtualization and KVN support
- NFC devices support
- Bluetooth support
- NVME and SSD support (may have some bugs open issue)
- Intel and AMD Drivers


#### How to use:
1. Install WSL last version from this [[link](https://github.com/microsoft/WSL/releases)] -- note: min version of WSL should be ```2.3.24```
2. Install last version of [usbipd](https://github.com/dorssel/usbipd-win/releases)
3. Copy kernel file from repository to a folder in windows
4. Open run(win + R) and enter: "C:\Program Files\WSL\wslsettings\wslsettings.exe"
5. Developer section
6. Custom kernel
7. Browse kernel and select the kernel
8. ```wsl --shutdown``` in cmd
9. ```wsl``` in cmd
10. Run cmd as administrator
11. ```usbipd list```
12. ```usbipd bind -b <your device BUSID>```
13. ```usbipd attach -w -b <your device BUSID>```
14. enjoy :) for make sure your device connected in wsl enter: ```sudo lsusb```
