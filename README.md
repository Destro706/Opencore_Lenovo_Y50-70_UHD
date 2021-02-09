## OpenCore EFI for Lenovo Y50-70 (UHD 4K) updated for Big Sur

### For FHD Version go to https://github.com/GeekyCoder7/OpenCore-EFI-Lenovo-Y50-70
### For installing BigSur use PRE-EFI.
### After installation, use POST-EFI.



### Updated to OpenCore 0.6.6
### Updated kexts

**Specs:**
  - Intel Core i7-4710HQ
  - Intel HD4600 integrated GPU
  - Nvidia GTX 860M 4GB (unsupported)
  - 16GB DDR4 Ram
  - BCM94350ZAE (WiFi / Bluetooth)
  - Realtek Cardreader
 
 Before updating any kext create pendrive copy of actual EFI so if something wont
 work you can restore it.
 
 **What works:**
 
 - Dual Boot with Windows/Linux
 - built-in keyboard
 - built-in trackpad (multi gestures)
 - HDMI video/audio with hotplug
 - WiFi through BCM94350ZAE
 - Bluetooth through BCM94350ZAE
 - Handoff
 - Airdrop
 - AirPlay mirroring to AppleTV
 - native USB3
 - Realtek Cardreader
 - native audio with AppleHDA
 - built-in mic
 - built-in camera
 - native power management
 - battery status
 - backlight controls with smooth transitions, save/restore across restart
 - accelerated graphics for HD4600 (4K)
 - wired Ethernet
 - retina scaling
 - Sleep/Wake
 - Auto Brightness Sensors
 - iMessage & Facetime
 - Brightness keys on keyboard
 - Filevault 2
 
 


Notes: 
- In order to use iMessage and Facetime you need to change your SMBIOS, with GenSMBIOS.<br>
Link: https://github.com/corpnewt/GenSMBIOS <br>
- updated SMBIOS to macbookpro11,4, Thanks to geekycoder7
- added BCM94350ZAE as it was cheap (round about 5€ at ebay), fully working, need unlocked BIOS for whitelisting and needed to set ASPM for PCI Express Slot 2 to L0 in BIOS to solve Quirks
- DVMT prealloc has to be set to 128mb
- after updating to OC 0.6.6 you need to reset NVRAM
  I needed to rename bootmgfw.efi in EFI/MICROSOFT to bootmgfw1.efi once, so that OC is detected. After that I renamed back and with new OC it shouldn't be the case in future

