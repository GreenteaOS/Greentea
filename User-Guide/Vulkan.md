## Enhanced use of the Vulkan API

[Vulkan](https://en.wikipedia.org/wiki/Vulkan_(API)) - is a modern most advanced graphics [API](https://en.wikipedia.org/wiki/Application_programming_interface). It allows to get best of your [GPU](https://en.wikipedia.org/wiki/Graphics_processing_unit).

Greentea OS is going to use Vulkan as much as possible: [window composition](https://en.wikipedia.org/wiki/Compositing_window_manager), Direct 3D and OpenGL rendering, image and video decoding, WebGL and so on.

This would require Vulkan to be always present, so there should be at least software emulation of that graphics API.

## NjRAA

We will also investigate possibility of native D3D implementation in the project called [NjRAA](https://github.com/GreenteaOS/NjRAA) aka **Not just Renamed AMD API**.

## Case study

- OpenGL over Vulkan
  - [VKGL - Core OpenGL over Vulkan](https://github.com/kbiElude/VKGL)
  - [ZINK: OpenGL Over Vulkan](https://gitlab.freedesktop.org/kusma/mesa/commits/zink)
  - [GLOVE: OpenGL ES Over Vulkan](https://github.com/Think-Silicon/GLOVE)
  - [ANGLE's WebGL / OpenGL ES Over Vulkan](https://github.com/google/angle/tree/master/src/libANGLE/renderer/vulkan)
- Direct3D 9 over Vulkan
  - [VK9](https://github.com/disks86/VK9)
- Direct3D 9/10/11 over Vulkan
  - [DXVK](https://github.com/doitsujin/dxvk)
- Direct3D 9/10 over Gallium
  - [Gallium Nine Standalone](https://github.com/dhewg/nine)
- Vulkan over Metal
  - [MoltenVK is a Vulkan Portability implementation](https://github.com/KhronosGroup/MoltenVK)
