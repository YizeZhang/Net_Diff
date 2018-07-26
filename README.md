# Net_Diff

Net_Diff is a software for GNSS Download, Positioning and Analysis.

It provides functions of SPP/PPP/DSPP/DPPP/RTK, it can also applied in SPP/PPP with BeiDou augmentation information.

It provides data analysis, including coordinate plotting, satellite skyview, satellite number, PDOP, satellite skyview, satellite number, omc, positioning residuals and so on.
 
It also provides IGS data and products download.

*****************************************************************************************************
How to install:
1. Click gzip-1.3.12-1-setup.exe and install gzip. For example, after install it, gzip.exe is under C:\Program Files (x86)\GnuWin32\bin\
 
2. a) If you have installed MATLAB or MATLAB Runtime version 9.2 (R2017a) in your computer.
   
      Open /for_redistribution_files_only/ and click Net_Diff.exe
      
   b) If not.
   
      Open /for_redistribution/ and click Net_Diff_Installer_web.exe to install MATLAB Runtime and Net_Diff.exe
      Please keep your computer connected to internet while installing.
      It will take a few minutes to download MATLAB Runtime, please be patient.
      After finish installing, you can find the execute file from the installed program directory, like C:\Program Files\Net_Diff\application\. 
      
      If your Windows OS is under C:\, Net_Diff may can’t read and write files under C:\. In this case, it is recommended to copy C:\Program Files\Net_Diff\application\ to other disk.
      
3. Copy C:\Program Files (x86)\GnuWin32\bin\gzip.exe to the directory of Net_Diff GUI.

As for the use of Net_Diff, please refer to the guide document "A guide to use Net_Diff.pdf".

Source code is under the src branch.     
****************************************************************************************************
If you have any questions or problems in using Net_Diff, please contact me:  zhyize@163.com


****************************************************************************************************
Revision Note:

2018/07/24 
   1. Modify GUI in Analysis panel 

   2. Modify RTK fix and hold mode

   3. Change GLONASS satellite number from 24 to 27
   
2018/07/25
   1. Modify ISB model in PPP
   
   2. Fix bugs of BeiDou PCO
   
2017/07/26
   1. Fix bugs in GUI
