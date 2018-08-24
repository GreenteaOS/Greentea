### Quick guide to build a system with WineHQ

> Information is out of date

Builds within other operating systems are performed using the [WineHQ](https://www.winehq.org) project.
It is assumed that the reader is familiar with the utilities **WineHQ** and **winetricks**, set them up and they are ready to work.

The process is radically no different from
[a common guide](Build-Native.md),
except for a few nuances.

#### Downloading the source code repository

Perform the procedure identical to [the article](Build-Native.md).
The repository may be placed into the home folder (in WineHQ this is the path `Z:\home\username\`).

#### Installing the Build Environment

Set the environment as in [the article](Build-Native.md).

#### Build, test and rebuild

Before executing this procedure, you need to find the `configure.cmd` file in the sources folder, and edit it with gedit:

* Comment out the line following after `REM Detect presence of cmake`, adding the word` REM` at the beginning of the line:
<br/>`REM cmd /c cmake --version 2> .....rest of the line`
* Find the line following after `if "%BUILD_ENVIRONMENT%" == "MinGW"`
* At the end of the line, the parameter `"%SOURCE_DIR%"` must be replaced with the path to the repository (in the WineHQ format), for example:
<br/>`"Z:/home/username/Greentea/Kernel"`

Now you can open a WineHQ shortcut on the desktop and execute `configure`, and then, completely the same as in the [article](Build-Native.md).
