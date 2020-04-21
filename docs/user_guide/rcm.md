# RCM {docsify-ignore-all}

RCM (short for ReCovery Mode) is a mode for the switch that allows nintendo to send the switch commands to do various things. People found out that on unpatched switches, you could send a payload, and then quickly copy it into the memory buffer behind the stack, overflowing the memory buffer into the stack, meaning you smash the stack and get full access to everything on the system. We use it here to launch atmosphere.

> [!TIP|label:emuNAND vs emuMMC vs sysNAND]
>	- sysNAND stands for System NAND, meaning the internal storage in your actual Switch.
>	- emuNAND stands for emulated NAND, this means that your entire NAND (system memory) will run off your microSD card with Custom Firmware (CFW). This NAND's contents (games, applications, saves, etc.) are *completely separate* from your sysNAND.
>	- emuMMC is the name for the currently used implementation of emuNAND on Switch. It has no difference from emuNAND besides name.

----

### emuMMC CFW (**Recommended**)

> [!TIP|label:What's needed for emuMMC]
>	- A microSD card that's 64GB or larger
>
>	#### Pros of using emuNAND over sysNAND CFW:
>	
>	- Using homebrew applications such as save editors, or cheating in games offline without "dirtying" or affecting sysNAND, allowing sysNAND to be used online without ban risk.
>	- Allowing users on patched Switches using Caffeine to update their emuNAND to latest and use it online, keeping sysNAND at a lower vulnerable version.


### [Continue to Entering RCM <i class="fa fa-arrow-circle-right fa-lg"></i>](user_guide/emummc/entering_rcm.md)
-----


### sysMMC CFW (**Not Recommended**)

This is for the people who don't have an 64GB microSD card or larger, or who don't want an emuMMC for whatever reason. 

> [!NOTE]
>	If you set up an emuNAND you may still have CFW on your sysNAND if you choose to use it. You do not have to follow the guide linked below; all the files are the same, you simply select "sysNAND CFW" from Hekate/Nyx.


#### [Continue to SD preparations (sysNAND CFW) (**Not Recommended**) <i class="fa fa-arrow-circle-right fa-lg"></i>](user_guide/sysnand/sd_preparation.md)
