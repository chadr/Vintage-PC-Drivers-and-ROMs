      --<< ACARD AEC-671X PCI Ultra/W SCSI Controller >>--


----------
Auto Setup
----------
Install Windows 95/98/NT4.0/2000 driver automatically.

    Windows 95/98/NT:
      1. Insert the SCSI card in PCI slot, then power on the computer.
      2. Insert disk1.
      3. Press [Start] --> [Run]
      4. Type "A:\setup32.exe", or press [Browse] to find the driver.
      5. Press [enter]
         then it will install SCSI driver, utility and "OnNow" function automatically.
      6. Reboot the computer.


------------------------
Interactive Installation
------------------------
Installing Windows 95 driver manually

      1. Power off the computer and then plug AEC-671X in PCI slot
      2. Power on the computer, Windows 95 would show "New Hardware Found"
      3. Insert the disk1
	
          If you want to use "Auto Setup" function, 
          --> choose [Cancel] to use "Auto Setup" to install driver automatically
          (follow Auto Setup steps 3,4,5)
      
      you can see "PCI SCSI Bus Controller"
      
      4. Choose [Other Location] or you may press [Browse] to find driver.
      5. Type " A:\WIN95", then press [Enter]
      6. It will show AEC671X model number. Press [Finish]
      7. Reboot the computer

      Please note ! When windows ask for "A870PROP.DLL" , type "A:\WIN95"


Installing Windows 98 driver manually.

      1. Power off the computer and then plug AEC-671X in PCI slot
      2. Power on the computer, Windows 98 would show "New Hardware Found"
      3. Insert the disk1
 
	   if you want to use "Auto Setup" function, 
           --> choose [Cancel] to use "Auto Setup" to install driver automatically
           (follow "Auto Setup" steps 3,4,5)

      you can see "PCI SCSI Bus Controller"

      4.  Choose [Next] 
      5.  Choose [Next]
      6.  Choose [Specify a Location]
      7.  Type "A:\WIN98" or press [Browse] --> "A:" --> click "Win98" Folder and press [OK]
      8.  Press [Next]
          WIN98 will find "AEC671X MODEL number"
      9.  Press [Next]
      10. Press [Next]
          Windows will copy driver to your hard disk
      11. Press [Finish]

      Please note ! When windows ask for "A870PROP.DLL" , type "A:\WIN98"

	
------------------------------
Installing DOS driver manually
------------------------------
      Run the "Install.exe" will modify the config.sys & autoexec.bat
      and copy driver specify directory.
      Then you can use the SCSI HDD, MO, ZIP, CD-ROM, etc..
      If you use the CD-ROM please check the parameter in autoexec.bat of "MSCDEX.EXE"
      is exist.


---------------------------     
Update Windows 95/98 driver
---------------------------

      If you want to update AEC-671X driver, refer to the following steps.

	    select items sequentially

	    [My Computer]
        [Control Panel]
        [System]
	    [Device Manager]
	    [Hard Disk Controller]
	    you can see "AEC-671X PCI Ultra/W SCSI Controller"
        [OK]
	    [Driver]
	    [Update Driver]

     At the moment, insert the newest AEC-671X driver diskette to drive A:
     press [Browse], then select directory "A:\WIN95" or "A:\WIN98"
     file AEC671X.INF would be selected.
     then press [OK]
     Windows 95/98 would install the newest AEC-671X driver to the system


------------------------------------------
Installing Windows NT 3.51 driver Manually
------------------------------------------
      1. Power off the PC, plug the card AEC-671X to the slot
      2. Power on the PC, do following steps.

	    Select items as following

	    [Main]
	    [Windows NT Setup]             -->  press  [Option]
        [Add/Remove SCSI Adapters]     -->  press  [Add], then [OK]
	    [Select SCSI Adapter Option]   -->  select [Other]
                                       -->  press  [Install]

     At the moment, insert the newest AEC-671x driver diskette 1 to drive A:
     then type in directory "A:\WINNT"

     then press [OK]
     Windows NT would install the newest AEC-671X driver to the system.


------------------------------------------
Installing Windows NT4.0 driver manually
------------------------------------------
      1. Power off the PC, and then plug AEC-671X in PCI slot
      2. Power on the PC, refer to following steps
      3. Insert disk1

	    Select items as following

	    [My Computer]
        [Control Panel]
	    [SCSI Adapters]
	    [Drivers]
        [Add]
        [Have Disk]
        type "A:\WINNT" or choose [Browse] to find driver
        [OK]
        choose "ACARD AEC671X PCI Ultra/W SCSI-3 Controller"
        [OK]
        if Windows NT ask the OEM SCSI file, type "A:\WINNT"
        press [Continue]
        [Reboot]

     Windows NT would install the newest AEC-671X driver to the system.
