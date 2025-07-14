## Aether's OpenCore AMD EFI folder

<img width="2560" height="1440" alt="x11rhgg86t9f1" src="https://github.com/user-attachments/assets/b8140c69-d0eb-4348-afbf-262f15d6a22b" />


A screenshot of it running on my system. Yes, I love Ralsei.



This config applies for the following:
 - AMD Ryzen 9 5900X
 - AMD Radeon RX 6600XT
 - ROG Strix B550-F Wifi II
 - Intel I225-V Ethernet (Non-Functional Atm)
 - macOS Sequoia 15 (Might work with Tahoe)

The following EFI folder applies for my AMD system. You will need to change the UUID and Serial in the config.plist.

**Warning:** I225-V networking on either the config or my system is completely f*cked. It will NOT boot if you have AppleIGC.kext or the networking enabled in BIOS. If it works for you, amazing. If you figure out a fix, I love you.

I will try my best to keep this folder up to date if I learn it doesn't work with new macOS versions.

Known issues:
 - Networking (Expected)
 - Wi-Fi (Obviously)
 - Bluetooth
 - iServices (Due to missing proper networking)
 - Virtualization (This is known on AMD hackintoshes)
 - Some Adobe things.

**Solution I found for networking:** If you don't have access to a compatible network adapter or networking card, you can use an Android device to function as a USB Wi-Fi adapter. Using **[HoRNDIS](https://github.com/jwise/HoRNDIS)**, you can connect an Android phone for tethering on macOS. Keep in mind, this might not work on some devices (like carrier locked devices) and my device is a custom rommed Pixel. Using a Pixel 3 running Project Elixir, you can use it as a hotspot device using only Wi-Fi (similar to how hotspot sharing works on Windows devices). Obviously, due to this approach, you will not get iServices.

ps. If you have anything to contribute, please do <3.
