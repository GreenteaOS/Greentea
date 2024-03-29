### Running in VirtualBox

[VirtualBox](https://ru.wikipedia.org/wiki/VirtualBox) is used for running the system in an isolated environment.
With its help it is possible to install Greentea OS into any file on the computer with the existing system,
and changes within the virtual environment thus do not affect external files or devices.

To install in this case, you only need to have a computer with a preinstalled system and a sufficient amount of memory
(both disk and RAM).
You may also need to enable [the VT-x option in the BIOS or UEFI](https://www.shaileshjha.com/step-by-step-guide-to-enable-intel-vt-x-or-amd-v-in-bios-or-uefi-in-windows-10-and-windows-8/).

#### Installing the Virtual Machine

* Download and run the installer [for the main operating system](https://www.virtualbox.org/wiki/Downloads);
* There you also need to download the `VM VirtualBox Extension Pack` and open it (VirtualBox should start and suggest installing the extension).

#### Testing Greentea

You *must* configure the VM to support UEFI and multicore CPU.

The simplest way to achieve this is to choose **Mac OS X (64-bit)** preset.

Than, set CPU count to 2 or more cores, RAM to 2 or more GBs.
Changing other defaults is not recommended.


#### Linux user?

Try `virtualbox-dkms` instead of normal `virtualbox` in case of problems.
