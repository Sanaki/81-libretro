# 81-libretro

**81-libretro** is an *work in progress* port of the [EightyOne](http://www.chuntey.com/) (a.k.a. THE Sinclair Emulator) to [libretro](http://www.libretro.com/). It's being developed on Windows with MinGW (64 bits) and Debian 8, and tested on RetroArch 1.2 frontend.

## Emulated Machines

EightyOne emulates a number of ZX80, ZX81, clones, and other computers based on the same hardware:

* Sinclair ZX80
* Sinclair ZX81
* Timex TS1000
* Timex TS1500
* Lambda 8300
* Ringo R470
* MicroDigital TK85
* Jupiter ACE

However, **81-libretro** only emulates the Sinclair ZX81 with 16Kb RAM for now. Other machines will be added as time permits. Push requests are welcome.

The port correctly loads and runs ~~some~~ many games I have around in the `p` format. `tzx` format is not supported yet.

EightyOne also emulates some ZX Spectrum machines, but those were left out of this core on purpose. For a ZX Spectrum core for libretro, see the [Fuse core](https://github.com/libretro/fuse-libretro).

## Core Options

The only core option available on the frontend is:

* Video Presets (clean|tv|noisy): Change how the video is emulated

## Keyboard and Controllers

A keyboard and a cursor joystick are configured and should work out-of-the-box.

## Supported Formats

The only format supported is the `p` format. I wanted to support `tzx` tapes but the emulator refuses to load them. Push requests are welcome.

## Save States

Save states are supported.

## Setup

1. Compile **81-libretro** with `make -f Makefile.libretro`
1. Copy the resulting `81_libretro.dll` or `81_libretro.so` into the `cores` folder of your libretro frontend
1. Profit!

## Versions

Versions that are being used to build and test **81-libretro**:

* EightyOne version 1.0 (test a)

## TODO

See the open issues.

## Bugs

Many, probably. Open issues or send push requests.

## License

GNU GPLv3.0
