## Roadmap and goals

The main idea of the project is to quickly and efficiently create a compatible environment for the existing software and provide the best user experience of a personal computer.

### Planned features and improvements

* CPU
 * [x] BIOS boot
 * [x] [x86-64-only mode (**dropping x86-32**)](x64.md)
 * [ ] Multicore HAL and scheduler
 * [x] UEFI boot
 * [x] USB boot fixes
* GPU
 * [ ] [Software Vulkan](../User-Guide/Vulkan.md)
 * [ ] Hardware Vulkan
 * [ ] OpenGL
 * [ ] D3D
* Kernel
 * [x] [New kernel in Hexa](../User-Guide/Hexa.md)
 * [x] Stable memory manager
 * [ ] GUI for OS installer
 * [ ] [Moving to a journaling filesystem](../User-Guide/Greentea-FS.md)
 * [x] LiveCD/USB
 * [ ] Stable networking
 * [x] Initial .exe support
 * [ ] Full .exe support
 * [ ] Linux subsystem (only software)
 * [ ] Android subsystem
 * [ ] [Easy system updates](../User-Guide/Rolling.md)
* Visuals
 * [x] New default theming and visuals
 * [ ] Theming engine
 * [ ] [New HTML5-alike theming engine and toolkit](../User-Guide/Web.md)
 * [ ] Overhaul of theming engine (GPU-accelerated, shadows, blurs, effects)
* Shell and UI
 * [x] Initial implementations of shell, tray, explorer, start button and others
 * [x] Greentea widgets and GUI elements
 * [ ] Stabilization of shell, tray, explorer, start button and others
 * [ ] [Shell overhaul to add modern features and look](../User-Guide/Control-Panel.md)
 * [ ] Customizable themes and widgets
 * [ ] Stable and finished user space software

---

### Not planned features

This project started as a controversy to undefined future (and past) of existing operating systems.
Our team decided to define precise list of *the most useful* features to the wide audiences.
Features, like ARM support, aren't really useful in any real manner *right now*, as already showed by other vendors.

**Update from 2023:** seems like M1 CPUs finally make ARM support valuable?

Features, like LPT printing, has so small applicability (LPT ports in 2018 anyone?),
so can't be considered in any manner real target for Greentea OS team and use case for our users.
Also, multiply that by a *enormous* number of bugs, hacks and workarounds, which we should fix now,
to at least make kernel non-academic project! And then improve implementations, **the real things**.
Otherwise it is a waste of time.

---

### Feature timings

Features are highly dependent of Kernel API version.
Also, the ecosystem defines it's own distribution rules.
For example: while it *is* possible to run Vulkan API over virtually any (even 20 years old) operating system,
no hardware or middleware (LunarG) distributors actually did it.
Some features also, like native Wi-Fi or BLE support, were non-existent on old versions.
So we need to declare timings and dependencies for each feature.
