# ZGUI v0.3
This repo contains custom zig bindings for imgui

## Getting Started
Clone this repo, copy it to `root` of your project(`root/lib` is more preferred)
In your build.zig file, add
```zig
exe.addPackage(zgui.zgui(exe));
exe.addPackage(zgui.glfw(exe)); //Make sure to add glfw as dependency (Prefered binding is mach_glfw)
exe.addPackage(zgui.opengl(exe)); //Add OpenGL support for Imgui
exe.addPackage(zgui.vulkan(exe)); //Add Vulkan support for Imgui
```

## To run Examples
Please make sure the contents of this repository(excluding examples) are copied to examples/deps/zgui/

## Currently Supported Backends
- OpenGL
- GLFW (mach-glfw)
- Vulkan

## Planned
- DirectX 10
- DirectX 11
+ more

## Special Thanks
[Michal-z](https://github.com/michal-z) : For inspiring me with [zgui](https://github.com/michal-z/zig-gamedev/tree/main/libs/zgpu) bindings for wgpu.
[SpexGuy](https://github.com/SpexGuy) : For imgui bindings for Zig.
