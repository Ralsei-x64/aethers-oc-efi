<img width="601" height="178" alt="GLG" src="https://github.com/user-attachments/assets/072d5e2a-93a2-4d47-a836-ac045e766e56" />




<img width="2560" height="1440" alt="Screenshot 2025-07-15 at 15 21 53" src="https://github.com/user-attachments/assets/93b97780-86f2-40cf-a051-66ab77afec58" />

This branch is for macOS Sequoia! If you're looking for Tahoe, use the Tahoe-Beta branch.

**This config applies for the following:**
 - AMD Ryzen 9 5900X
 - AMD Radeon RX 6600XT
 - ROG Strix B550-F Wi-Fi II
 - Intel I225-V Ethernet

The USB ports and AMD patches are tailored to my specific configuration. Be careful if you decide to use slightly different hardware.

**Compatible OS Versions:**
- macOS Sequoia 15 (Use this branch, stable.)
- macOS Tahoe 26 (Use the Tahoe-Beta branch, very much experimental.)

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

**Acknowledgements:**
- The [AMD OS X](https://discord.com/invite/EfCYAJW) for being insanely helpful and providing a patched version of AppleIGC
- [AMD Vanilla](https://github.com/AMD-OSX/AMD_Vanilla) for AMD patches
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/) for teaching me how to set up OpenCore
- [Apple](https://apple.com) for macOS

ps. If you have anything to contribute, please do <3.
