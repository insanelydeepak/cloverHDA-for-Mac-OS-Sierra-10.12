
![HDA Icon](https://raw.githubusercontent.com/insanelydeepak/cloverHDA/master/cloverHDA.jpg)
# cloverHDA 

This cloverHDA.kext enables audio/sound on Mac OS Sierra 10.12


### Requirements : 
      1 - Vanilla/Native AppleHDA 
      2 - a good Kext Installer or [EastKextPro](http://www.insanelymac.com/forum/files/file/397-easykext-pro-a-minimal-and-super-fast-kext-installer/)
  
      3 - Property List Editors - Xcode or Property List Editor, PlistEdit Pro, TextEdit, etc.
      4 -  must have CLOVER/config.plist
           i. RtVariables/BooterConfig/0x28
            ii. RtVariables/CsrActiveConfig/0x3 


### Installation :

      1 - Download cloverHDA.kext as per your Audio ID's 
      2 - Install using EastKextPro or any Kext Installer to /S/L/E
      3 - Now apply patches from cloverHDA.plist to your Clover config.plist (You don't have to do this if using method HDAEnabler or HDEF Patch)
      4 - Add Layout_ID = 13 , 11 or 12 as described in ReadME.txt 
      5 - Restart 

#### Note : for Layout_ID you can use DSDT (HDEF Patch) or Clover (Clover/Config.plist/Devices/Audio/Inject=Audio_ID) or [HDAEnabler's kexts](https://bitbucket.org/insanelydeepak/hdaenablers-applehda-for-hackintosh/downloads)

### Layout_ID/Audio ID description :

    for Desktop's:
      1 - Layout_ID 11 = 5/6 ports supported (Pink, Green, Blue) (Note : without auto-switch , you have to manually select between output/input device's) 
      3 - Layout_ID 13 =   5/6 ports supported (Grey, Black, Laranja, Pink, Green, Blue)
      
    for Laptop's :
      1 - Layout_ID 13 =   3/5 ports supported (Black, Pink, Green, Blue)

### Supported Codec/DEVICE_ID :

  You must have one of the following DEVICE_ID/Codec name described below :
 
      1 - Realtek ALC to Desktop's: ALC887, ALC888, ALC891, ALC892
      2 - Realtek ALC to Laptop's: ALC255, ALC269, ALC269VC, ALC269VB, ALC270, ALC271, ALC272, ALC275, ALC282, ALC292, ALC298, ALC662, ALC665, ALC898 , ALC88
      3 - Conexant for laptop's: CX20590,CX20724 ,CX20752
      4 - IDT for Laptop's: IDT92HD71B7X,IDT92HD73C1X5, IDT92HD75B2X5, IDT92HD75B2X5, IDT92HD81B1X5, IDT92HD90BXX, IDT92HD91BXX, IDT92HD93BXX
      5 - VIA Laptop's: VT1802 
      6 - Cirrus Logic Laptop's: CS4213 and CS4210 

###  [Troubleshooting :](https://github.com/insanelydeepak/cloverHDA-for-Mac-OS-Sierra-10.12/blob/master/TroubleShoot/Troubleshoot%20Reporting.md)
       After installing repair permissions and rebuild caches use an application of your choice and Restart
       Recommended to Use EasyKexPro  
       Restart , if still not geting sound devices then :
       please report with Requested files 


This kext is based on  [PikeRAlpha's DummyHDA method](https://pikeralpha.wordpress.com/2013/12/17/new-style-of-applehda-kext-patching/) and Clover Patches on fly  method's
### Credits :
PikeRAlpha, Mirone, EmlyDinesh, The king, Master Chief, RevoGirl, toleda, bcc9, TimeWalker and many others who contributed to AppleHDA patching.

