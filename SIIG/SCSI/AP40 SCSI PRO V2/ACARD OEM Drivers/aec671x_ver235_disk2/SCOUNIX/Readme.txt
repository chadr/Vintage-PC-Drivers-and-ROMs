SCO UNIX Environment
ACARD AEC671X PCI Ultra SCSI Adapter SCO UNIX 3.2.x Device Driver

First, You need a installed SCO UNIX 3.2.x or SCO Open Desktop 3.x system.

1) Boot your SCO UNIX system.
2) Use doscp command to copy the file AEC671X.tar to your /tmp directory.
       e.g. if you are using floppy drive A, type
            doscp a:/scounix/AEC671X.tar /tmp
3) Insert a SCO UNIX-formatted empty diskette(EAFS file system).
4) Now, Mount floppy to directory /topfdd.
	 Type following commands mount /dev/fd0135ds18 /topfdd
	   (for 1.44MB diskette only,See follows)

      cd /topfdd
      tar xvf /tmp/aec671x.tar .
      cd /
      umount /topfdd

    Your floppy drive 0 device name could be:
      fd096ds15      -->   5.25 DSHD 
      fd0135ds18     -->   3.5  DSHD
      fd048ds9       -->   5.25 DSDD
      fd0135ds9      -->   3.5  DSDD

You are now ready to install the driver package for ACARD AEC671X
The ACARD driver diskette can use "custom"(UNIX shell) or "link"(boot time)
to install SCSI driver and rebuild UNIX kernel. Normally "link" is for boot
SCSI device or first time fresh installation.

Start the installation by Fresh installtion,You need use "link" as follows:

1) Insert SCO UNIX boot disk(N1 or P1) and power on
2) When system boot from N1 or P1 type "link" and press <Enter> key
   as follows :
   SCO UNIX System V/386 on 80486

   Boot
   :link <Enter>
3) SCO UNIX will ask you package name. You need type "ATP"
  and <Enter> as follows :
   What	packages do you need linked in the system,
   or q to quit?:ATP <Enter>
4) Then follow the SCO UNIX installation procedure until installed 
  complete.

If ACARD AEC671X is not a boot device. You can start the installation
by typing "custom" under UNIX shell as follows :
  %custom

You need relink the UNIX kernel and reboot your system for the new kernel.
