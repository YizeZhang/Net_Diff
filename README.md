# Net_Diff

Net_Diff is a software for GNSS Download, Positioning and Analysis.

It supports functions of SPP/PPP/DSPP/DPPP/RTK/PPP-RTK, it can also applied in SPP/PPP with BeiDou augmentation information.

It supports data analysis, including coordinate plotting, positioning error comparison, satellite number, PDOP, satellite skyview, satellite visibility, cycleslip, troposphere, ionosphere, observation minus correction, positioning residuals and so on.
 
It provides IGS data and products download.

It also provides some useful tools such as time and coordinate system transfer, RINEX edit.


*****************************************************************************************************
## How to install:
 1. Install gzip
   
        Click gzip-1.3.12-1-setup.exe and install gzip. 
      
        For example, after install it, gzip.exe is under C:\Program Files (x86)\GnuWin32\bin\
  
 2. Instal Net_Diff
 
    *a) If you have installed MATLAB or MATLAB Runtime version 9.2 (R2017a) in your computer.*
   
        Open /for_redistribution_files_only/ and click Net_Diff.exe
      
    *b) If not.*
   
        Open /for_redistribution/ and click Net_Diff_Installer_web.exe to install MATLAB Runtime and Net_Diff.exe
     
        Please keep your computer connected to internet while installing.
        
        It will take a few minutes to download MATLAB Runtime, please be patient.
        
        After finish installing, you can find the execute file from the installed program directory, like C:\Program Files\Net_Diff\application\. 
      
        !!!!!!!If your Windows OS is under C:\, Net_Diff may can’t read and write files under C:\. In this case, it is recommended to copy C:\Program Files\Net_Diff\application\ to other drive!!!!!!!!!
      
  3. Complete Full Installation
  
    Copy C:\Program Files (x86)\GnuWin32\bin\gzip.exe to the directory of Net_Diff GUI.

***
* When use the software, please open it from execute file, not from Windows Start.    

* As for the use of Net_Diff, please refer to the guide document "A guide to use Net_Diff.pdf".

* Source code is under the src branch.

***
*If you have any questions or problems in using Net_Diff, please contact me: zhyize@163.com*


***

<br/>
<br/>  

## Revision History:


###    **V1.0**

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
   

---
###     **V1.1**

2018/09/13
   1. Fix bugs when there are too few satellites while cycle slip in RTK
   
   2. Support Doppler selection in GUI
   
2018/09/16
   1. Support RINEX editing in GUI, modify GUI 
   
2018/09/18
   1. Support Time and Coordinate Transfer in GUI.
   
   2. Support command line file input function for Net_Diff.
   

---
###     **V1.2**

2018/09/28
   1. Fix bugs in static SPP
   
   2. Fix bugs in GUI
   
   3. Support multi-GNSS tight combined RTK
   
   4. Support posfile output available for RTKPLOT.
   
   5. Support Coordinate.txt appended after Control.txt
   
2018/09/29
   1. Fix bugs in BDS WADS PPP mode
   
   2. Modify GUI
   
2018/10/12
   1. Fix bug in BeiDou PCO of C13 for gbm
   
   2. Modify tightly combined RTK
   
   3. Modify GUI   
   

---
###     **V1.3**
   
2018/10/17
   1. Support GLONASS AR in tightly or loosely combined RTK
   
   2. Modify tightly combined RTK
   
   3. Support Android raw data convert to RINEX
   
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
   

---
###     **V1.4**
    
2018/11/16
   1. Support mix-frequency combination on each satellite system (only available in GUI)
   
   2. Support mix-observation combination on each satellite system (only available in GUI)
   
   3. Support PPP-AR (only available in GUI)
   
   4. Support undifferenced uncombined PPP (only available in GUI)
   
   5. Add output of ionosphere correction in uncombined PPP
   
   6. Add phase windup correction in RTK
   
   7. Reduce matrix size to improve processing efficiency
   
   8. Changeable cycle slip detection threshold
   
   9. Fix bug in LAMBDA
   
   10. Fix bug of Galileo PCO correction
   
   11. Modify GUI
      
2018/11/19
   1. Support triple-frequency undifferenced uncombined PPP (only available in GUI)
   
   2. Change ionosphere initial value of undifferenced uncombined PPP
   
   3. Fix bug of ionosphere correction when frequency combination is L2L3
   
   4. Fix bug when cycle slip method is only LLI in RTK
       
   5. Modify GUI
   

---
###     **V1.5**
    
2018/12/14
   1. Support PPP-RTK (CLAS) (only available in GUI)
   
   2. Change output file name for better parallel computing
   
   3. Change threshold of outlier detection
   
   4. Fix bug of IRNSS frequency
   
   5. Modify GUI
      
2018/12/26
   1. Support triple-frequency ionosphere-free PPP (only available in GUI)
   
   2. Support Android dual-frequency multi-GNSS raw data converted to RINEX
   
   3. Fix bug of BDS PCO using new atx file in triple frequency PPP
   
   4. Turn off time restriction of BSX file
   
2018/12/27
   1. Change maximum BeiDou satellite PRN to 37
   
   2. Fix bug of satellite orbit value in sp3 file when it is 0.000
   

---
###     **V1.6**
    
2018/01/25
   1. Support new signal of BDS (B1c/B2a) and GLONASS (G3), Galileo(E6), QZSS(L6)
   
   2. Fix bug of doppler aided SPP/PPP
     
2018/02/04
   1. Support user self-named file selection in GUI
   
   2. Fix bug of GLONASS AR
   
   3. Speed up efficiency of matrix inversion and least square solution.
   
2018/02/14
   1. Add SNR depended stochastic model
   
   2. Change elevation depended stochastic model in RTK, change phase noise from 1cm to 3mm
   
   3. Fix bug of doppler aided RTK
   
   4. Modify GUI
   

---
###     **V1.7**

2018/02/25
   1. Support Net Solution  (Authorized)
   
   2. Support loosely coupled PPP/INS and RTK/INS (Authorized)
   
   3. Add threshold of success rate in AR
   
   4. Add data-based and model-based combined AR
   
   5. Fix bug of DCB correction for different frequency combination
   
   
   
