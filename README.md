## OpenCore EFI for Lenovo Y50-70 (SHD-1080p or UHD 4K) updated for Big Sur

### For FHD Version go to https://github.com/GeekyCoder7/OpenCore-EFI-Lenovo-Y50-70
### For installing BigSur use PRE-EFI.
### After installation, use POST-EFI.



### Updated to OpenCore 0.6.4
### Updated Whatevergreen.kext
### Edited Config.plist to match new Whatevergreen.kext and enable UHD Screen
### enabled Filevault 2

**Specs:**
  - Intel Core i7-4710HQ
  - Intel HD4600 integrated GPU
  - Nvidia GTX 860M 4GB (unsupported)
  - 16GB DDR4 Ram  
 
 Before updating any kext create pendrive copy of actual EFI so if something wont
 work you can restore it.
 
 **What works:**
 
 - Dual Boot with Windows/Linux
 - built-in keyboard
 - built-in trackpad (multi gestures)
 - HDMI video/audio with hotplug
 - AirPlay mirroring to AppleTV
 - native USB3
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
 - Brightness keys on keyboard (Fixed by migrating from ApplePS2SmartTouchPad.kext to VoodooPS2Controller.kext)
 
 
 


Notes: 
- In order to use iMessage and Facetime you need to change your SMBIOS, with GenSMBIOS.<br>
Link: https://github.com/corpnewt/GenSMBIOS <br>
- For those having issues with the display color, for some users the display color have a light brownish tint. <br>
In order to fix this you need to calibrate your display colors, by going into display settings from system preferences, then click calibrate from the color tab.
- If UHD still have Minor Glitches, rename Config UHD 2.plist to Config.plist and try that one
- DVMT prealloc has to be set to 128mb

