### Quick build guide

#### Downloading the source code repository

* Repository code itself will take **up to** 500 (five hundred) megabytes on the disk
* Make sure that you download the code to a folder **that does not contain spaces** in the path!
* Go to [the repository page](https://github.com/GreenteaOS/Kernel)
* If you *do not* use Git then download the archive of the code: <br/>![Image](https://cloud.githubusercontent.com/assets/3642643/19634448/d98f79fa-99c3-11e6-9d3e-009db22395e1.png)
* For Git users: `git clone --depth 10 --recursive https://github.com/GreenteaOS/Kernel.git`
* For users of [Github for Desktop](https://desktop.github.com): <br/>![Image](https://cloud.githubusercontent.com/assets/3642643/19634404/61125858-99c3-11e6-9c36-60f5a814fcc1.png)
* In the same folder, temporary files and disk images will be generated during the build process

#### Installing the Build Environment

* Download :fire: Flame :fire: by [direct link](https://github.com/GreenteaOS/Flame/archive/master.zip) or [on the repository page](https://github.com/GreenteaOS/Flame)
* Unpack to the recommended path `C:\Flame` or edit `environment.cmd` parameter `TOOLS` when unpacking to a non-standard path
* You should get the folder `C:\Flame` with file `version.txt` (archive version) and the rest (but not nested `C:\Flame\Flame`!)

#### Build, test and rebuild

* Before you start the build, make sure that you have **at least a gigabyte** of free disk space!
* The initial build takes approximately 40 (forty) minutes, depending on the configuration of the PC
* Run the script `build-bootcd.cmd` (double-click on the file) or `build-livecd.cmd` from the root of the Kernel repository to build the installation or live disk respectively
* To rebuild it is enough to repeat the same procedure again, it can take from five seconds to several minutes,
depending on the number of affected dependencies and configuration of the PC
* In the folder `output-MinGW-i386` in the case of successful build appears `livecd.iso` or `bootcd.iso`
