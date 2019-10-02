# Softy
Softy is a software renderer implementation written from scratch simply for educational purposes.

## Things implemented
At the moment the following things are implemented:
 * Depth buffer visualisation
 * Normal mapping
 * Parallax occlusion mapping
 * Flat/Gouraud/Phong shading models
 * Multisample anti-aliasing (4xmsaa)

## ScreenShots
Here are some screenshots from some of my demos
Shading Models:
![shadingModels](https://user-images.githubusercontent.com/30685457/66068443-48a17600-e556-11e9-89a2-858ecb7b0a0a.png)

Parallax mapping:
![parallax](https://user-images.githubusercontent.com/30685457/66069307-c4e88900-e557-11e9-8e00-4b32d2780758.png)

## Build instructions(from root directory)
In order to build renderer and examples you need to
pass the following flags to cmake:

```
cmake -BBuild -H. -DCMAKE_INSTALL_PREFIX=./
    -DSDL_ROOT=<Absolute_path_to_SDL_root_dir>
    -DCMAKE_BUILD_TYPE=Release
```
This will create bin direcroty with all examples inside.

Note > for Windows platform you also need to pass Visual Studio generator to cmake, for example (-G"Visual Studio 15 2017 Win64").

## Running examples
After examples are built you can run them from the project's root directory like so:

```
    <demo_install_prefix>\bin\<demo_name>.exe
```
