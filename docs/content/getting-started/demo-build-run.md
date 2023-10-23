---
title: "Build and Run"
date: 2022-12-26T15:26:15Z
lastmod: 2022-10-26T15:26:15Z
draft: false
weight: 25
---

---
#### Build
The `Demo-PinGod.tscn` should be visible and you can build the project (top right `Build` button). 

This demo scene is instancing a pre made `MainScene`. The `MainScene` has `Modes` which scenes can be added to. With this MainScene the `Attract` scene is added when the window is launched and after resources have loaded (pre loading scenes).

---
#### Play

`F5` to run the game. You can use `F2` on the window to show border. The game can be launched with a switch window by enabling it from the `WindowActions.tscn` scene from the `pingod-windows` addon in the `Inspector` options.

*Tip:Search for the scene name in the Godot file explorer filter and add scene to favorites*

![image](../../images/demo/first-run.jpg)

---
#### Quit

`F8` or `ESC` (need pingod-windows plugin on) to exit the window.
