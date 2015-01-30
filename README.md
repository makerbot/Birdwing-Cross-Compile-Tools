All of the cross compile toolchains for birdwing should live here.
This should be checked out automatically by Toolchain-Release
whenever you build a birdwing related toolchain.

## Cross-linaro

Cross-linaro is our preferred toolchain, and is used to build everything
that goes on the filesystem itself.  If you are adding something to the
filesystem, try to get it to build with this first.

[BW-SCons-tools](https://github.com/makerbot/bw-scons-tools) will automatically
select the correct cross-linaro to build with: cross-linaro-osx on OS X,
cross-linaro64 on 64-bit linux, and cross-linaro on 32-bit linux.  All three
toolchains are built with the same config, and should be functionally identical.

## Angstrom

Angstrom (http://www.angstrom-distribution.org/) is used to build the
linux kernel and bootloaders.  May work on 64-bit linux.

## AVR

We currently use gcc-avr for all avr firmware on the birdwing platform.
Avr-osx will automatically be used by bw-scons-tools when compiling on osx.
Although the version of gcc-avr in the avr-osx and avr folders is the same,
it's not recommended to compile production firmware on OS X.
