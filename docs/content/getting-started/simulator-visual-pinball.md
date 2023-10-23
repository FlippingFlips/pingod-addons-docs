---
title: "Run with Visual Pinball"
date: 2022-12-26T15:26:15Z
draft: false
weight: 26
---

The [pingod-addons/simulators](https://github.com/FlippingFlips/pingod-addons/tree/main/simulators/visual-pinball) directory contains an example table and script which is wired to work with the demo `project.godot`.

---
## Setup

A few steps are needed to make this possible so that Visual Pinball can launch the game and get machine changes from the game.

See [How To install and Run](https://github.com/FlippingFlips/pingod-addons/tree/main/simulators/visual-pinball#how-to-install--run)

---
## Running with VP
The game can be launched with `Visual Pinball` after the setup is completed for the `PinGod.VP.Controller`.

If you launch from the repository as is then the project will be loaded relative `../../` from the script.

*Note: To recieve changes from game make sure the `pingod-memorymap-win` plugin is enabled and MemoryMapping is enabled*

---
## Visual Pinball Player
Add credits and start the game to pulse a ball from the Trough.