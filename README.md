Fork Readme

Build fltk on Window 10

#A Build with MinGW-w64 - for 32 and 64 bit Windows

A1. Download MinGW-w64 - for 32 and 64 bit Windows from here: https://sourceforge.net/projects/mingw-w64/files/Toolchains%20targetting%20Win64/
Under MinGW-W64 GCC-8.1.0, choose x86_64-posix-sjlj. As a result, file x86_64-8.1.0-release-posix-sjlj-rt_v6-rev0.7z is downloaded.
A2. Unzip with 7-zip
A3. After extracting, copy the mingw64 folder to C:\
A4. Add C:\mingw64\bin to the Path of the System Environment Variables.
A5. Browse to C:\mingw64\bin folder, make a copy of mingw32-make.exe and rename the copy as make.exe

A6. IF not installed cmake, please install cmake.

A7. AT the lower left corner of Windows desktop, in the search area where 'Type here to search' is shown, type in cmd, then press 'Enter' key to open Command Prompt Window. switch to fltk folder, run these commands

MKDIR build_MinGW
CD build_MinGW
cmake -DCMAKE_MAKE_PROGRAM=make -DCMAKE_CXX_COMPILER=g++ -DCMAKE_INSTALL_PREFIX=d:/3rd_MinGW -G "MinGW Makefiles" ..

A8. Run make
    Remeber to do step A5, otherwise you will get an error saying 'make is not found'.
    
A9. Run make install
A10. You can compile your own fltk application code now


#B Build with Fortran, C and C++ for Windows

B1. Download Fortran, C and C++ for Windows from http://www.equation.com/servlet/equation.cmd?fa=fortran
    Under DOWNLOAD: THREE LAST RELEASES section, choose one to download. Here we use gcc-10.2.0-
64.exe




Original Readme

# README - Fast Light Tool Kit (FLTK) Version 1.4.0

## WHAT IS FLTK?

    The Fast Light Tool Kit ("FLTK", pronounced "fulltick") is a
    a cross-platform C++ GUI toolkit for UNIX(r)/Linux(r) (X11),
    Microsoft(r) Windows(r), and MacOS(r) X. FLTK provides
    modern GUI functionality without the bloat and supports 3D
    graphics via OpenGL(r) and its built-in GLUT emulation. It
    was originally developed by Mr. Bill Spitzak and is
    currently maintained by a small group of developers across
    the world with a central repository in the US.

    For more information see README.txt:
    https://github.com/fltk/fltk/blob/master/README.txt
