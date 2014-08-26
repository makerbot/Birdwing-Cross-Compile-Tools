All of the cross compile toolchains for birdwing should live here.
This should be checked out automatically by Toolchain-Release
whenever you build a birdwing related toolchain.


## Cross-linaro

Cross-linaro is the toolchain that is now used to build everything that goes
on the filesystem itself as of about September 2014.  It is built off of
linaro gcc version 4.8.3 20140106 using crosstool-ng.  If you are adding
something to the filesystem, try to get it to build with this first.
Built to run on 32-bit hosts.

## Cross-linaro-host64

Same as the Cross-linaro toolchain, except built to run on 64-bit hosts.

## Cross-linaro-deprecated

Cross-linaro-deprecated is the toolchain that was used to build everything
that goes on the filesystem itself up until about September 2014.  It is built off of
gcc version 4.8.1 20130401, which has some bugs (it's unable to build qt5.3.1).
It has been deprecated in favor of a newer version of linaro gcc.

## Angstrom

Angstrom (http://www.angstrom-distribution.org/) is used to build the
linux kernel and bootloaders.  May work on 64-bit linux.

## AVR

We currently use gcc-avr for all avr firmware on the birdwing platform.
