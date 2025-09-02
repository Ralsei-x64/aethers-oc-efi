<img width="614" height="224" alt="Logo" src="https://github.com/user-attachments/assets/7c6032d0-51f0-4b01-a036-14700149fe98" />



<img width="2560" height="1440" alt="Screenshot 2025-07-15 at 15 21 53" src="https://github.com/user-attachments/assets/93b97780-86f2-40cf-a051-66ab77afec58" />

#For AMD only!#

**This config applies for the following:**
 - AMD Ryzen 9 5900X
 - AMD Radeon RX 6600XT
 - ROG Strix B550-F Wi-Fi II
 - Intel I225-V Ethernet

The USB ports and AMD patches are tailored to my specific configuration. Be careful if you decide to use slightly different hardware.

**Compatible OS Versions:**
Only macOS Sequoia 15 is tested. Your luck with anything newer or older will vary.
EFI for macOS Tahoe will be available soon.

You will need to use MacSerial in order to generate SMBIOS info if you want to use iServices.

**How to add to a USB flash drive:**
1. Format it to FAT32 with GPT.
2. Add the files to the flash drive's EFI directory.
3. Use MacSerial to add SMBIOS info to plist.
4. Add macOS recovery files to boot to an installer.
6. Boot into the USB drive.

Please refer to the Dortania AMD guide for important settings you might need to change.

**Known issues:**
 - Wi-Fi
 - Bluetooth
 - Virtualization (This is known on AMD hackintoshes)
 - Some features of certain Adobe Apps. (Like motion stabilizing in Premiere Pro)

~~**Solution I found for networking:** If you don't have access to a compatible network adapter or networking card, you can use an Android device to function as a USB Wi-Fi adapter. Using **[HoRNDIS](https://github.com/jwise/HoRNDIS)**, you can connect an Android phone for tethering on macOS. Keep in mind, this might not work on some devices (like carrier locked devices) and my device is a custom rommed Pixel. Using a Pixel 3 running Project Elixir, you can use it as a hotspot device using only Wi-Fi (similar to how hotspot sharing works on Windows devices). Obviously, due to this approach, you will not get iServices.~~

ps. If you have anything to contribute, please do <3.

**Thanks to the AMD OS X discord for providing a patched version of AppleIGC which works with my system.**

*Warning: For the current version ("Fixing I225-V Networking"), configurator tools were used. The upcoming version which works with Tahoe will feature a redone config from scratch.*

Do not upgrade to Tahoe yet. From my testing, it does not boot. I'm currently working on a new EFI which will boot Tahoe.
