
```bash
[iocuser@ip5-33 gitsrc]$ lspci -nmn |grep 1180
01:09.0 "Signal processing controller [1180]" "PLX Technology, Inc. [10b5]" "PCI9030 32-bit 33MHz PCI <-> IOBus Bridge [9030]" -r01 "Unknown vendor [1a3e]" "Device [20dc]"

[iocuser@ip5-33 gitsrc]$ git clone https://github.com/jeonghanlee/pciids
Cloning into 'pciids'...
remote: Counting objects: 296, done.
remote: Total 296 (delta 0), reused 0 (delta 0), pack-reused 296
Receiving objects: 100% (296/296), 960.09 KiB | 835.00 KiB/s, done.
Resolving deltas: 100% (98/98), done.

[iocuser@ip5-33 gitsrc]$ cd pciids/

[iocuser@ip5-33 pciids]$ bash replace-pciids.bash 
centos was determined.

[iocuser@ip5-33 pciids]$ lspci -nmn |grep 1180
00:1f.6 "Signal processing controller [1180]" "Intel Corporation [8086]" "82801H (ICH8 Family) Thermal Reporting Device [284f]" "" ""
01:09.0 "Signal processing controller [1180]" "PLX Technology, Inc. [10b5]" "PCI9030 32-bit 33MHz PCI <-> IOBus Bridge [9030]" -r01 "Micro-Research Finland Oy [1a3e]" "CPCI Event Generator 220 [20dc]"
[iocuser@ip5-33 pciids]$ 
```
