# Xon Compiling made easy

This is a tutorial on how to compile xon using windows! :D
Follow these steps ahead and its supposed to work.

* 1 We will be using Msys to do it, can be found here: https://www.msys2.org/

* 2 After Installing it, close the current MSYS2 shell and go to C:\msys64 folder, right click on MINGW64.exe and create a shortcut of it.

* 3 Using the shortcut u just made do the following command
`pacman --needed -S git curl zip unzip p7zip make automake autoconf libtool gcc gmp-devel mingw-w64-x86_64-{toolchain,gmp,SDL2,libjpeg-turbo,libpng,libogg}`

* 4 After installing the dependencies lets start cloning the git repo with following command:
`git clone https://gitlab.com/xonotic/xonotic.git`

* 5 Do: `cd xonotic`

* 6 Then: `./all update -l best`

Done downloading and updating now lets compile

* 1 Do: `./all compile -r`

* 2 And `./all run` to run the game

To run the game always open the mingw64.exe shortcut and do `./all run`

In case u have some missing textures followingthe next steps

* 1 You must be in xonotic folder, if u are not just do `cd xonotic`

* 2 Then just do `touch data/xonotic-nexcompat.pk3dir.yes`

* 3 Then `./all update -l best`

* 4 now to recompile the changes `./all compile -r`

