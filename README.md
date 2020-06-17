# Asus-Prime-X570-Pro-OpenCore-EFI
This is a backup of my working OpenCore 0.5.9 EFI folder.

Things to note:
- I'm using an AMD Radeon 5500 XT so I have in the config.plist boot-args: agpdmod=pikera. If you have Nvidia or using iGPU, remove this. I used to have a 3200G with this and it will work without acceleration if you remove the agpdmod=pikera too.
- This is kernel patched to run on 17th Ryzen AMD processors.
- I have this running with Catalina 10.15.5 (latest).
- I have enabled the GUI for selecting the bootable OS as I have both Windows 10 and macOS on my machine.
- Audio is working properly for non APU processors. All APU Ryzen still don't have proper audio due to kernel. I switched CPU because of this.

# SMBios and serial number
You will need to use GenSMBIOS to edit the config.plist so that you have a valid serial number for your hackintosh (otherwise iCloud and others don't work). I've used MacPro6,1 for my SMBios and it works great even with 3200G. I recommend you use that. Check OpenCore documentation on using GenSMBIOS to add the missing info into the config.plist.

Questions, use the issues and I'll try to help you.

# Disclaimer
This is provided AS IS. I'm not responsible for your hardware or headaches you may get if this doesn't work for you. It is working for my mobo + cpu (3600X) + gpu (5500 XT) combo. Can't Dockerize the hardware :o)
