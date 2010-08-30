INTRODUCTION
============

TehRipper is a simple command-line program to do batch ripping and burning of audio CDs or data CDs/DVDs. Great for ripping box sets, etc. Set it to go and it will rip your disc, eject it, and wait for you to put the next one in. Burning works the same way. 

The program relies on the following command line utilities, as well as Ruby and Ruby gems. It should work across Linux/Unix platforms, and on Windows with a little modification. If you have these installed, you should be good to go.

* cdrecord (cdrtools)
* cdrdao
* dd
* commander gem

USING IT
========

`tehripper` - gives you a list of available commands  
`tehripper help <command>` - gives you help on the options for a specific command

TODO LIST
=========

Critical:

* Add a command-line argument for specifying the drive device. Currently hard-coded for /dev/sr0 and scsi id 0,0,0.

Cool additions:

* Re-factor the individual command options out to universal options, since they're all the same
* Read CDDB database (cdrdao may be able to do this), and name the files accordingly
* Rip to FLAC option (or mp3, if you care for lossy music...)
* More compact command line syntax, like `tehripper read-audio 1:14 schmorgtunes`  
  which would be the same as the current `tehripper read-audio --start 1 --end 14 --prefix schmorgtunes`

