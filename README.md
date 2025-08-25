<img width="2560" height="1440" alt="Screenshot 2025-07-15 at 15 21 53" src="https://github.com/user-attachments/assets/93b97780-86f2-40cf-a051-66ab77afec58" />


## Aether's OpenCore AMD EFI folder


**This config applies for the following:**
 - AMD Ryzen 9 5900X
 - AMD Radeon RX 6600XT
 - ROG Strix B550-F Wi-Fi II
 - Intel I225-V Ethernet

The USB ports and AMD patches are tailored to my specific configuration. Be careful if you decide to use slightly different hardware.

**Compatible OS Versions:**
From Ventura 13 to Sequoia 15. macOS Tahoe 26 will not boot due to outdated AMD patches. I am currently working on a redone version of my EFI which features support for Tahoe. It is nearly complete but AppleIGC is causing issues relating to system hangs, crashes, and instability. I will most likely release this EFI soon as a pre-release but you might be stuck without any ethernet. It's up to the developer of AppleIGC or the AMD OS X community to release a functional version of AppleIGC.

You will need to use MacSerial in order to generate SMBIOS info if you want to use iServices.

**Known issues:**
 - Wi-Fi
 - Bluetooth
 - Virtualization (This is known on AMD hackintoshes)
 - Some features of certain Adobe Apps. (Like motion stabilizing in Premiere Pro)

~~**Solution I found for networking:** If you don't have access to a compatible network adapter or networking card, you can use an Android device to function as a USB Wi-Fi adapter. Using **[HoRNDIS](https://github.com/jwise/HoRNDIS)**, you can connect an Android phone for tethering on macOS. Keep in mind, this might not work on some devices (like carrier locked devices) and my device is a custom rommed Pixel. Using a Pixel 3 running Project Elixir, you can use it as a hotspot device using only Wi-Fi (similar to how hotspot sharing works on Windows devices). Obviously, due to this approach, you will not get iServices.~~

ps. If you have anything to contribute, please do <3.

**Thanks to the AMD OS X discord for providing a patched version of AppleIGC which works with my system.**

*Warning: For the current version ("Fixing I225-V Networking"), configurator tools were used. The upcoming version which works with Tahoe will feature a redone config from scratch.*
