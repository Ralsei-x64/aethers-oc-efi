<img width="601" height="178" alt="GLG" src="https://github.com/user-attachments/assets/072d5e2a-93a2-4d47-a836-ac045e766e56" />




<img width="2560" height="1440" alt="Screenshot 2025-09-04 at 17 25 40" src="https://github.com/user-attachments/assets/ba039a79-991a-4117-a7be-f9e5bec4673c" />

This branch is for macOS Tahoe! If you're looking for Sequoia, use the Sequoia-Stable branch.

**This config applies for the following:**
 - AMD Ryzen 9 5900X
 - AMD Radeon RX 6600XT
 - ROG Strix B550-F Wi-Fi II
 - Intel I225-V Ethernet

The USB ports and AMD patches are tailored to my specific configuration. Be careful if you decide to use slightly different hardware.

**Compatible OS Versions:**
- macOS Sequoia (Works, use the Sequoia-Stable branch)
- macOS Tahoe (Currently testing, use this branch)

You will need to use MacSerial in order to generate SMBIOS info if you want to use iServices.

**How to add to a USB flash drive:**
1. Format it to FAT32 with GPT.
2. Add the files to the flash drive's EFI directory.
3. Use **[MacSerial](https://github.com/acidanthera/OpenCorePkg)** to add SMBIOS info to plist.
4. Add macOS recovery files to boot to an installer.
6. Boot into the USB drive.

Please refer to the Dortania AMD guide for important settings you might need to change.

**Known issues:**
 - Wi-Fi
 - Bluetooth
 - Virtualization (This is known on AMD hackintoshes)
 - Some features of certain Adobe Apps. (Like motion stabilizing in Premiere Pro)
 - Joining calls on the official Discord app. (Might just be a personal issue, but Vesktop does not suffer from this issue.)
 - Motherboard Audio (AppleALC is currently broken. Use DisplayPort/HDMI audio or a USB audio device to negate this)

If you're updating macOS, disable WhateverGreen. WhateverGreen will cause crashes during the update process! It's okay to re-enable it after you're done updating.

**Acknowledgements:**
- The [AMD OS X](https://discord.com/invite/EfCYAJW) discord for providing a patched version of AppleIGC which works with my system.
- [AMD Vanilla](https://github.com/AMD-OSX/AMD_Vanilla/tree/beta) for AMD patches
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/) for teaching me how to set up OpenCore
- [Apple](https://apple.com) for macOS
