# Net_Diff

Net_Diff is a software for GNSS Download, Positioning and Analysis.

It supports functions of SPP/PPP/DSPP/DPPP/RTK, it can also applied in SPP/PPP with BeiDou augmentation information.

It supports data analysis, including coordinate plotting, satellite skyview, satellite number, PDOP, satellite skyview, satellite number, omc, positioning residuals and so on.
 
It provides IGS data and products download.

It also provides some useful tools such as time and coordinate system transfer, RINEX edit.


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
      
      !!!!!!!If your Windows OS is under C:\, Net_Diff may can’t read and write files under C:\. In this case, it is recommended to copy C:\Program Files\Net_Diff\application\ to other disk.!!!!!!!!!
      
3. Copy C:\Program Files (x86)\GnuWin32\bin\gzip.exe to the directory of Net_Diff GUI.

As for the use of Net_Diff, please refer to the guide document "A guide to use Net_Diff.pdf".

Source code is under the src branch.     
****************************************************************************************************
If you have any questions or problems in using Net_Diff, please contact me:  zhyize@163.com


****************************************************************************************************



Revision History:



************************************************************************
*****************************      V1.0    *****************************

2018/07/24 
   1. Modify GUI in Analysis panel 

   2. Modify RTK fix and hold mode

   3. Change GLONASS satellite number from 24 to 27
   
2018/07/25
   1. Modify ISB model in PPP
   
   2. Fix bugs of BeiDou PCO
   
2018/07/26
   1. Fix bugs in GUI
   
2018/08/09
   1. Modify GUI
   
   2. Change selecting reference satellite method
   
   3. Change settings in long baseline RTK
   
2018/08/17
   1. Use traditional KF algorithm in long baseline RTK and change some settings
   
   2. Modify Galileo F/Nav and I/Nav broadcast ephemeris selection
   
   3. Add GLONASS in RTK float solution
   
2018/08/21
   1. Change default ratio from 3 to 2
   
   2. Fix bug of static long baseline RTK

2018/08/22
   1. Fix bugs in GUI
   
2018/08/24
   1. Change coordinate variance to 60m, modify outliers detection
   
   2. Change troposphere constraint in long baseline RTK

2018/08/26
   1. Modify partial AR
   
2018/08/27
   1. Change settings for long baseline RTK
    
2018/08/30
   1. Change selection of reference satellite in RTK
   
   2. Improve outlier detection in RTK
   
   3. Change Galileo max satellite number from 31 to 36
    
2018/09/03
   1. Modify GUI
   
2018/09/06
   1. Fix bugs in GUI
   
   2. Add GPS L2C observation
   




************************************************************************
*****************************      V1.1    *****************************

2018/
09/13
   1. Fix bugs when there are too few satellites while cycle slip in RTK
   
   2. Add Doppler selection in GUI
   
2018/09/16
   1. Add RINEX editing in GUI, modify GUI 
   
2018/09/18
   1. Add Time and Coordinate Transfer in GUI.
   
   2. Add command line file input function for Net_Diff.
   



************************************************************************
*****************************      V1.2    *****************************

2018/09/28
   1. Fix bugs in static SPP
   
   2. Fix bugs in GUI
   
   3. Add multi-GNSS tight combined RTK
   
   4. Add posfile output available for RTKPLOT.
   
   5. Support Coordinate.txt appended after Control.txt
   

2018/09/29
   1. Fix bugs in BDS WADS PPP mode
   
   2. Modify GUI
   

2018/10/12
   1. Fix bug in BeiDou PCO of C13 for gbm
   
   2. Modify tightly combined RTK
   
   3. Modify GUI   
   



************************************************************************
*****************************      V1.3    *****************************
   
2018/10/17
   1. Add GLONASS AR in tightly or loosely combined RTK
   
   2. Modify tightly combined RTK
   
   3. Add Android raw data convert to RINEX
   
   3. Modify GUI
   
   
   
2018/10/20
   1. Fix bugs in non-L1L2 combination when using clock from sp3 file
   
   2. Fix bugs tightly combined RTK
   
   
   
2018/11/08
   1. Fix bugs of single system SPP when ISB setting is true
   
   2. Fix bugs of SPP for outlier detection
   
   3. Fix bugs of PCV correction for Galileo and QZSS
   
   4. Fix bugs of loosely combined GLONASS RTK
   
   5. Change maximum time difference of RTK to 30s
   
   6. Modify GUI
   
   
   
2018/11/09
   1. Support mixed frequency combination for multi-GNSS (only supported in GUI)
   
