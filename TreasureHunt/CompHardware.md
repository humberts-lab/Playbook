1. Faulty or unplugged power supply (PSU), or failed motherboard, or bad power button connection
2. Commonly indicates RAM failure (depends on BIOS manufacturer).
Next step:
Reseat or replace the RAM modules and test again.
(Optionally consult the motherboard manual for specific beep codes.)
3. Hardware causes:
Loose or disconnected SATA/NVMe cable
Failed storage drive (SSD/HDD)
Software fix:
Repair or reinstall the bootloader using Windows Recovery (e.g., bootrec /fixmbr).
4. Component/feature:
CPU fan or heatsink with thermal paste; BIOS temperature monitoring or automatic thermal shutdown feature.
Monitoring:
Use Task Manager → Performance tab, HWMonitor, or BIOS hardware monitor to check CPU temps.
5. Command:
ping (e.g., ping 8.8.8.8) or ipconfig to verify IP setup.
Physical issue:
Damaged Ethernet cable, bad port, or cable not rated for Gigabit speeds (Cat 5 vs Cat 6).
6. Hardware causes:
Loose or damaged video cable (HDMI/DisplayPort)
Failed GPU or motherboard video output
Test:
Connect monitor to another system or try integrated graphics to isolate the problem.
7. File type:
.VHD / .VHDX (Hyper-V) or .VMDK (VMware) virtual disk files.
Possible corruption reason:
Unexpected shutdown, insufficient storage, or manual deletion of the VM directory.
8. Tool/setting:
Device Manager → Uninstall/Reinstall device driver, or Printers & Scanners → Remove device → Add again.
9. Advantage:
Accessible from anywhere, supports collaboration and automatic backups.
Risk:
Data breaches or downtime if cloud service is compromised or unavailable.
10. <img width="839" height="460" alt="image" src="https://github.com/user-attachments/assets/e8be180c-87da-4607-96d8-2bf70183be95" />

Reflection: In this lab, I applied A+ Core 1 troubleshooting concepts to realistic PC hardware and OS issues. I practiced diagnosing power, memory, and storage problems, tested network and display connections, and explored virtualization and driver troubleshooting. This exercise reinforced systematic problem-solving using both software tools and physical inspection.
