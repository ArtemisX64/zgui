# ZGUI v0.1
It contains a clone of [zgui](https://github.com/michal-z/zig-gamedev/tree/main/libs/zgpu) by [michal-z](https://github.com/michal-z) along with custom bindings inspired by michal-z's wgpu bindings.

## Getting Started
Clone this repo, copy it to `root` of your project(`root/lib` is more preferred)
In your build.zig file, add
```zig
exe.linkLibCpp(); // To compile imgui
zgui.link_imgui(exe);
exe.addPackage(zgui.zgui);
exe.addPackage(zgui.zgui_glfw); //Make sure to add glfw as dependency (Prefered binding is mach_glfw)
exe.addPackage(zgui.zgui_opengl); //Add OpenGL support for Imgui
exe.addPackage(zgui.zgui_vulkan); //Add Vulkan support for Imgui
```

## To run Examples
Please make sure the contents of this repository(excluding examples) are copied to examples/deps/zgui/

## Currently Supported
- OpenGL
- GLFW (mach-glfw)
- Vulkan (Experimental)

## Planned
- DirectX 10
- DirectX 11
+ more
