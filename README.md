All of the cross compile toolchains for birdwing should live here.
This should be checked out automatically by Toolchain-Release
whenever you build a birdwing related toolchain.

## Cross-linaro

Cross-linaro is our preferred toolchain, and is used to build everything
that goes on the filesystem itself.  If you are adding something to the
filesystem, try to get it to build with this first.  Does not run on
64-bit linux.

## Angstrom

Angstrom (http://www.angstrom-distribution.org/) is used to build the
linux kernel and bootloaders.  May work on 64-bit linux.

## AVR

We currently use gcc-avr for all avr firmware on the birdwing platform.
