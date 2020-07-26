# Fixing Dual Booting Windows 10 with Ubuntu 19.04: Grub not Showing and Machine Booting Straight to Windows
 open cmd as administrator
  bcdedit /set {bootmgr} path \EFI\ubuntu\grubx64.efi
