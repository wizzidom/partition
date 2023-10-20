# partition
How to remove right protection
<br>
<br>
or 
<br>
<br>
How to fix a USB drive showing up as two drives (fragmented into multiple partitions) on Windows:
<br>
<br>
Hold the Windows key and press X, select PowerShell (Admin), select Yes to the pop-up. You can also use Command Prompt.

<br>
<br>
In the Powershell interface type diskpart to enter the disk partition tool.
<br>
<br>
Type list disk to see all disks listed.
<br>
<br>
Select the USB drive by typing select disk [NUMBER]. Be careful to select the correct drive.
<br>
<br>
Type clean. An error will occur if you have the drive folder open, close the window and repeat the command if this happens.
<br>
<br>
Type create partition primary.
<br>
<br>
Type format fs=ntfs quick to format the drive (you can also choose to set fs=fat32).
<br>
<br>
Type active.
<br>
<br>
Type assign.
<br>
<br>
Type list disk and confirm your drive looks healthy.
<br>
<br>
Type exit to exit.
<br>
You can get visual confirmation by typing ‘disk manager’ into the windows search bar in the bottom left. Select the USB to view.
