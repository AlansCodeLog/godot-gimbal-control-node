# Gimbal Control Node

This is a gimbal node (for use with a camera, a light, or any other object) for Godot. It supports using keys, clicking and dragging, or mouse movement to look around. It also supports zooming, either with keys/mousewheel or with a toggle key (e.g. Joystick R3). And it doesn't have to be parented, it can track any target and even switch to targets with different rotations, and interpolated between them smoothly.

You can change any of the keys, set limits to the up/down rotation and distances, disable/emit right/left movements, and emit a first person signal.

The look_left/right signals are there so you can, for example, parent the gimbal (containing a camera) to a character then use the look left/right signal to rotate the character instead of the camera itself if you want to (see Demos).

The first person signal tells you when the camera has come within a certain range, so you can, for example, show a specific HUD element on screen.

### Note

I'm new to Godot and game development/programming in general (I didn't know what a Transform was when I started this), so there might be a few bugs. Everything seems to be working as I intended, but if you find any problems or you think there's a better way to do something, don't hesitate to file an issue.

## How to Install

You can download it from the AssetLib (search for Gimbal Control Node), or you can clone/download this repository then copy the addons folder to your project, or the folder inside that to your addons folder if you already have one.

From there you can enable it in `Project > Project Settings > Plugins`

The plugin requires certain `look_*` actions in the input map to work. If you want to use your own actions, you can specify them in the node. Or to quickly get started, you can copy them from the `project.godot` file in the demo project.

## Documentation

For now most of the documentation is in the actual script, including common issues to be aware of. I will eventually get around to formatting everything nicely here. If anything is unclear don't hesitate to file an issue.

## Demos

I have also made a project with various demo scenes for testing/demonstrating possible configurations, you can find it [here](https://github.com/AlansCodeLog/godot-gimbal-control-node-demos).
