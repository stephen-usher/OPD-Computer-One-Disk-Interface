# The recreated Computer One floppy disk interface for the ICL One Per Desk.
## Version 1.0: 14th July, 2024.

This is a reverse engineered version of the Computer One floppy disk interface for the ICL One Per Desk.

The circuitry has been simpified by replacing a great deal of discrete logic with a single GAL to handle the address decoding and the clock circuit has been replaced by a crystal oscillator.

The included ROM image also has beenmodified to add a BPB to the boot sector on the floppy disk format so that MSDOS PCs and Atari STs can read it. Unfortunately if PCs try to write to the disk it will corrupt the format. In tests Atari STs can correctly write to the disks.

It should be noted that using the OPD Microdrive Utilities copy is hit and miss with Gotek drives for some reason. With real floppy disks it's fine.

If you wish to use EPROMs larger than a 27C128 use bodge wires to connect pins 1 and 27 of the ROM to ground or put multiple copies of the image onto the EPROM.