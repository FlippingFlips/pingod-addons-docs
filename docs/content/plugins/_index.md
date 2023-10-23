---
title: "PinGod-Addons"
date: 2022-12-26T15:26:15Z
draft: false
weight: 10
---

Godot allows importing of `addons` into projects. Other addons can usually be found in Godot's `AssetLib` and installed through that. `addons` can also be imported to from a zip file or just copied into a project.

---
## pingod addons list

| Name | Autoload *  | Description
| --- | --- | --- |---|
| [pingod-core](core)  | no | Base classes for the modules 
| [pingod-assets](assets)  | no | Assets used by the modules. Localization for your game
| [pingod-controls](controls)  | no | Godot addin controls
| pingod-misc | no | Others scenes and layers | [link](./addons/pingod-misc) 
| [pingod-modes](modes) | no | Scenes and game modes, overlays
| [pingod-audio](audiomanager)  | yes | audio manager / player
| [pingod-game](pingodgame)  | yes | PinGodGame, Game and Main scenes. Demo uses the Main scene, which also uses the game and modes module
| [pingod-machine](machine) | yes | Machine manager for pinball machine items, events
| [pingod-memorymap-win](memorymap) | yes |Sharing machine states over memory mapping (**windows only**)
| [pingod-resources](resources) | yes | Resource loader, pre load scenes and `pck` files
| [pingod-windows](windows) | yes | Input handling and switch windows + custom windows

_* Autoload_ = plugin has an Autoload singleton. You can access these singletons from any script from the root. The main scenes can be overrided by duplicating the main scene for the Autoload and place into `res://autoload`, eg: `res://autoload/Resources.tscn`.
