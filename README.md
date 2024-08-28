# Dell XPS 8930 - Opencore

![Screenshot 2024-08-28 at 13 29 37](https://github.com/user-attachments/assets/66cd4079-cead-4538-9a3a-eb2a0801a80d)


<p align="center">
  <strong>Status: Active</strong>
  <br />
  <strong>Version: </strong>1.0
  <br />
</p>
<br />

## 📔 Notes
This configuration would probably only work on Dell branded PCs with 8th or 9th Gen Intel Core CPU only. Feel free to download or fork this repository to make your own version from this configuration.

> All ACPI Patches are made from following Dortania's OpenCore ACPI Patching Guide with Manual Method found here: [Link](https://dortania.github.io/Getting-Started-With-ACPI/)

> I am not going to support any beta version of MacOS. So, Released Version Only!

> I've removed the dedicated NVIDIA GPU as Dell motherboards tend to disable their display ports when there's a GPU plugged in.

## 🛠️ Hardwase
I've changed the internal WiFi & Bluetooth Card to a compatible Intel WiFi Card for compatibility and future-proofing as Broadcom Cards are less-preferred going forward from Sonoma.

| Hardware     | Description                                    |
|--------------|------------------------------------------------|
| CPU          | Intel Core i7-8700                             |
| GPU 1        | Intel UHD Graphics 630                         |
| GPU 2        | NVIDIA GTX 1060 6 GB (Removed)                 |
| SSD          | Toshiba KXG50ZNV256G 256GB NVMe                |
| Memory       | 16GB DDR4 2400Mhz                              |
| Network Card | Intel 8265-AC Dual Band                        |
| Ethernet     | Qualcomm Atheros Killer E2400 Gigabit Ethernet |

## ✅ What's Working?
- WiFI & Bluetooth (itlwm)
- Audio (AppleALC)
- USB Ports (USBMap)
- QE/CI
- Power Management / Sleep
- DisplayPort, HDMI, and DisplayPort over USB Type-C Video Output
- OS Updates
- USB Type-C
- DVD Drive
- Audio and Display AirPlay

## ❌ What's Not Working?
- NVIDIA GTX 1060 Discrete GPU (Last working version is 10.13.6 High Sierra)
- DRM Content over Safari (DRM Content over Chromium & Firefox Powered Browser works just fine)
- AirDrop, Continuity, Wireless Sidecar, Apple Watch Unlock (Limitations of Intel WiFI Card)
- HDMI Audio (Will try to fix on next release)

## ⚠️ Untested
- iServices (I have no Apple ID Account available atm)
- Wired Sidecar (I don't have an iPad to test)
