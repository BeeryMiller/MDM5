MDM5 Source Code

Write-up: Beery Miller, August 15, 2020

This zip file contains what is believed to be latest source code known for MDM5.

The software has been successfully assembled with the GenPROG package on the
Geneve 9640.  This program requires GenASM and GenLINK to properly assemble.
Other assemblers may be able to assemble the pieces should a user desire to use
a TI-99/4A to assemble.  The GenLINK control file (LINK1) contains the
necessary details on how the pieces are put together.

When assembling everything, the file MDM5 and MDMV are identical copies of the
same source file that MDM5 requires to save the configuration settings when
modifying the setup within MDM5.

If the file and directory structure is maintained, one can use the program ASS
that is a MDOS batch file, to assemble and launch the assembly process prior to
launching the LINK1 file with GenLINK (program name LINK).  The GenPROG package
can be obtained elsewhere.

MDM5 compiled programs are placed in the PGM folder and should be copied to DSK1
to run the program.  The file MDMFV60 is the hard drive format portion of the
program and can only be executed from within MDM5 when the file is on DSK1 and
the Utility Format command is executed.

There are some files in the root level of this zip file that end in a "1".  It
is believed these were work in progress files when John Birdwell was working
on the program.  It is unknown what change(s) these programs have.  In the
folder MODULES, there are 4 files. MCB/MCR and MDB/MDR.  These are the backup
and restore utilities for the hard drive within MDM5. The MDB/MDR modules are
the ones used for the compilation process as the MCB file contains a missing
label.  It appears the "C" and "D" within the MCB/MCR and MDB/MDR names
designate a revision.

Future Updates

Should someone desire to update MDM5, my suggestion is a modification to the
MDB/MDR modules to allow backup and restoration to files on a TIPI.

While the TIPI does not allow direct sector writes within its DSR, one can use
DIS/FIX 255 files to contain a full sector.  This is only a suggestion should
someone want to pursue this direction.

In the source code, I have changed the version number of this compiled program
to be Version 1.60 to separate this compiled image from all others.  There are
several source files that must be modified if you wish to change the version
number.  When doing this, the files created by GenLINK should have the digits
modified to reflect the two digits after the decimal.

Anyways, I hope individuals find this zip archive useful.

Beery Miller

