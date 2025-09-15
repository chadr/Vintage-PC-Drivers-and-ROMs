AEC671X.dsk supports NetWare 386 v3.1x and v4.x IDE disk module .
ACARD Uttra IDE Netware driver have full support for standard IDE disk drives

AEC671X.dsk also contain a built-in ASPI manager.  This allows for other 
NetWare Loadable Modules (NLMs) to gain access to the IDE host adapter. AEC671X.dsk compatible with built-in SCSI driver which are CDROM.nlm, ASPITRAN.DSK and ASPICD.DSK.

 :load AEC671X
  

1. Install Netware 3.12 

Example <A>
  OS      : Netware 3.12(Diskette)
  System  : 486-66 with 8 MB memory
  Fdd     : 1.44 MB(Drive A)
  Hdd     : corner 1.2 GB IDE hard disk(Drive C)
  Lan card: NE2000 compatible Ethernet
  Install procedure
     1. 	Make a small DOS partiton(20 MB).
     2. 	Make a directory c:\server.312
     3. 	Copy ACARD IDE driver(AEC671X.dsk) to directory c:\server.312 .
     4. 	copy lan driver NE2000.lan to c:\server.312
     5. 	Insert Netware 3.12 Install Diskette and run Install from Drive A:
     6. 	Follow Netware 3.12 procedure then into Netware Command line prompt.
     7. Load AEC671X.DSK from Drive c:\netware.312\AEC671X.DSK .
         		:load c:\netware.312\AEC671X <Enter>
     8.	Load Lan driver NE2000.lan
         		:load c:\netware.312\NE2000
         		:bind ipx to NE2000
     9. 	Load Install
   	10.	Partiton a Netware partition.
     11.	Create a Netware SYS: volume  and mount SYS:.
     12.	Follow Netware Installation guide
     	Copy Netware System file and utility
     13.	Create file Startup.ncf and autoexec.ncf



1. Install Netware 4.x

Example <B>
  OS    	: Netware 4.00(CDROM)
  System  : 486-66 with 16 MB memory
  Fdd   	: 1.44 MB(Drive A)
  Hdd    	: WD 1.0 GB IDE (Drive C)
  CDROM	: SONY CDU-521(Drive D on ARTOP SCSI-2)
  Lan card	: NE2000 compatible Ethernet

1. Make a small DOS partiton(20 MB).
2. Make a directory c:\server.40
3. Install CDROM drive as a MSDOS drive D:
4. Insert Netware 4.0 CDROM diskette.
5. Copy ACARD IDE driver(AEC671X.dsk) to directory 
  c:\server.40
     6. 	load CDROM driver.(AEC671X.dsk)
     7. 	Change directory to \netware.40\english then run INSTALL.BAT
     8. 	Give server name and IPX number then follow install guide.
     9. 	Select Load another(different) driver then press <Ins>,<F3>
         	select directory c:\server.40
         	then select AEC671X.DSK  
     10. 	Then continue to install.
     11. 	Then Select automatically to install Hdd partition.
     12. 	Select <F10> to save Volume.
     13. 	Then you need insert [LICESE] floppy diskette.
     14. 	Select <Alt><F10> exit to Netware command prompt.
     15. 	Load and mount CDROM.
     16. 	Load c:\netware.40\instll
     17. 	Select Install a new V4.0 server.
     18. 	Select <F3> to enter Directory CDVOL01:\netware.40\english
     19. 	Follow Novell install guide to continue next procedure.

