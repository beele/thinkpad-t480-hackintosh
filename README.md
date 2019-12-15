# T480 Hackintosh

This EFI folder contains everything to get a working copy of Mac OS Mojave running on a Lenovo T480.

Please fill in the correct values in the config.plist under EFI/Clover/config.plist as the `BoardSerialNumber`, `SerialNumber` and `SmUUID` have been redacted.
Please also correct the boot options under GUI/SCAN/LEGACY and GUI/HIDE in the config.plist file.
Please also correct the disabled port for the internal bluetooth under BOOT/ARGUMENTS/uia_exclude.

Laptop specs:

- CPU: Intel I5 8350u
- GPU: Intel HD 620
- RAM: 16GB DDR4 2400MHz
- 1080P display
- 512GB NVME SSD

What's working:

- GPU acceleration
- USB ports, even the USB-C port (disabled internal BT port - HS07)
- Webcam
- With correct `BoardSerialNumber`, `SerialNumber` and `SmUUID` => App Store, iCloud, iMessage, FaceTime
- Trackpad, red mouse pointer in keyboard
- Same drive Windows 10 dual boot with Mac OS Mojave

What's not working:

- TB3 display out (instant kernel panic)
- HDMI out (instant kernel panic)
- Battery indicator (don't know why...)

Resources used:

- [The Vanilla Laptop Guide](https://fewtarius.gitbook.io/laptopguide/)
- [Thinkintosh T480 EFI](https://gitlab.com/jjasonlam/thinkintosh_t480)
- [P52s-hackintosh](https://github.com/kk1987/P52s-hackintosh/blob/master/config.plist)
- [Success - Lenovo T480 running MacOS Mojave!](https://www.reddit.com/r/hackintosh/comments/9z7wia/success_lenovo_t480_running_macos_mojave/)
- [HACKINTOSH DUAL BOOT WINDOWS 10 AND MACOS HIGH SIERRA](https://hackintosher.com/guides/hackintosh-dual-boot-windows-10-and-macos-high-sierra/)
- [Bcm94352z | dw1560 causes Windows 10 Lockup / Freeze](https://www.tonymacx86.com/threads/bcm94352z-dw1560-causes-windows-10-lockup-freeze.256456/)
- [Belgian (Non-Apple) Keyboard Layout](https://github.com/remko/be-non-apple/)
