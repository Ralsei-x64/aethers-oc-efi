<img width="2560" height="1440" alt="Screenshot 2025-07-15 at 15 21 53" src="https://github.com/user-attachments/assets/93b97780-86f2-40cf-a051-66ab77afec58" />


## Aether's OpenCore AMD EFI folder



This config applies for the following:
 - AMD Ryzen 9 5900X
 - AMD Radeon RX 6600XT
 - ROG Strix B550-F Wi-Fi II
 - Intel I225-V Ethernet
 - macOS Sequoia 15


The following EFI folder applies for my AMD system. You will need to change the UUID and Serial in the config.plist.

At the current moment, some kexts and OpenCore itself is outdated. I will soon update these to the newest version when possible.

**Warning:** ~~I225-V networking on either the config or my system is completely f*cked. It will NOT boot if you have AppleIGC.kext or the networking enabled in BIOS. If it works for you, amazing. If you figure out a fix, I love you.~~ I225-V Networking is now fixed.

Tahoe will not boot. Please do not try to update or install it because you will waste a lot of time and potentially your data if you're upgrading from Sequoia.

I will try my best to keep this folder up to date if I learn it doesn't work with new macOS versions.

Known issues:
 - Wi-Fi (Obviously)
 - Bluetooth (Obviously)
 - Virtualization (This is known on AMD hackintoshes)
 - Some Adobe things.

~~**Solution I found for networking:** If you don't have access to a compatible network adapter or networking card, you can use an Android device to function as a USB Wi-Fi adapter. Using **[HoRNDIS](https://github.com/jwise/HoRNDIS)**, you can connect an Android phone for tethering on macOS. Keep in mind, this might not work on some devices (like carrier locked devices) and my device is a custom rommed Pixel. Using a Pixel 3 running Project Elixir, you can use it as a hotspot device using only Wi-Fi (similar to how hotspot sharing works on Windows devices). Obviously, due to this approach, you will not get iServices.~~

ps. If you have anything to contribute, please do <3.

**Thanks to AMD OS X for providing a patched version of AppleIGC which works with my system.**
