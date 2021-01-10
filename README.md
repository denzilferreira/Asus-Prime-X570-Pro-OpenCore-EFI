# Asus-Prime-X570-Pro-OpenCore-EFI
This is a backup of my working *OpenCore 0.6.5* EFI folder.

Things to note:
- I'm using an AMD Radeon 5500 XT so I have in the config.plist boot-args: agpdmod=pikera. If you have Nvidia or using iGPU, remove this.
- This is kernel patched to run on 17th Ryzen AMD processors.
- I have this running with Big Sur 11.1 (latest).
- All working, including sleep.

# SMBios and serial number
You will need to use GenSMBIOS to edit the config.plist so that you have a valid serial number for your hackintosh (otherwise iCloud and others don't work). I've used MacPro6,1 for my SMBios and it works great with my graphics card. I recommend you use that if you are using a Radeon 5xxx series. Check OpenCore documentation on using GenSMBIOS to add the missing info into the config.plist.

Questions, use the issues and I'll try to help you.

# Disclaimer
This is provided AS IS. I'm not responsible for your hardware or headaches you may get if this doesn't work for you. It is working for my mobo + cpu (3600X) + gpu (Radeon 5500 XT) combo.
