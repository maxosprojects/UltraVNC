# UltraVNC
UltraVNC Server and UltraVNC Viewer

Required compilers

Visual Studio 2017 or 2019

nasm assembler compiler (https://www.nasm.us/)


Load the project files vncviewer_vs2017.sln and winvncVS2017.sln to build server or viewer.


# Building vncviewer

1. Install NASM https://www.stefanobordoni.cloud/howto-integrate-nasm-with-vs2019/
2. Add NASM folder to env variable `PATH`
3. Install MFC for VS2019 if it's not yet installed (e.g. if running into problem with `afxres.h` not being found) https://stackoverflow.com/a/72723046
4. Open `vncviewer_vs2017.sln` with VS2019
5. Select `Release` and `x64` build target
6. In `vncviewer` project Properties, in `Build Events` > `Post-Build Event` disable `Use In Build` to prevent problem with signing the binary
7. Set `vncviewer` as Startup Project (in right click menu)
