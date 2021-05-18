# PianoFromAbove for ARM

This is a ARM build of <a href="https://github.com/brian-pantano/PianoFromAbove">PianoFromAbove</a>.

## Binaries

https://github.com/archeYR/PianoFromAbove-ARM/releases

## How to build

This is unfortunately very tricky. Hopefully I will simplify this in the future.

* clone this repo
* Download and install VisualStudio 2017
* Download and install Direct X SDK
* Download and extract Google Protocol Buffers 3.13
  * Build with Visual Studio using CMake, it might not be fully complete but it should generate a needed libprotobuf-lite.lib
* Download and extract Boost 1.76.
* Open the .sln and edit the VC++ Directories from the project properties so that the Include Directories and Library Directories point to the location of your boost and protocol buffers downloads
* Cross fingers
* Build! (Release, ARM)

Once that's done, there should be a Release\PFA-1.1.0-ARM.exe that you can run on any Windows ARM version (RT 8.0 onwards).

There's an optional .nsi script that you can run if you want to build an installer. 

## What about ARM64 build?

Maybe someday...
