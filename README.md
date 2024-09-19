# Gigabyte-B760M-DS3H-Hackintosh

# Specifications

- CPU: Alder-lake Intel i7-12700F (A 13th gen CPU will work as well as long as it's an F type. If it has an IGPU, you'll need to switch SMBIOS.)
- GPU: Biostar RX6800 (other variants such as Sapphire or MSI should work fine, as well as variants of the 6600.)
- Motherboard: Gigabyte B760M DS3H DDR4
- Wi-Fi/Bluetooth: MSI M.2 Adapter + Intel Wireless 3168AC (AirportItlwm + IntelBluetoothFirmware)
- Storage: SP 1TB NVME Gen 3
- RAM: 32GB (2x16GB) SK Hynix DDR4 3200MT/s

# Set-up/how-to

Follow the [dortania guide](https://dortania.github.io/OpenCore-Install-Guide/), then come back here and use diff or FileMerge (available in Xcode tools) to check for differences. 

Make sure to fill out PlatformInfo->Generic!

# What works and doesn't work

- Rear USB 2.0 ports are disabled. Rear USB3.0 ports are functional.
- Internal USB3.0 header (for front panel USB ports) is functional.
- On-board display outputs are untested, and will likely need more work.
- First internal USB2.0 header is functional, second is disabled. (To connect PCIE->USB bluetooth)
- Sleep, wake, power idling, etc work fine. Custom CPUFreq kext is used with CPUFriend to achieve 4.8GHz CPU clocks.

