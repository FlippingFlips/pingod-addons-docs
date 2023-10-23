---
title: "Logging Games"
date: 2022-12-26T15:26:15Z
draft: false
weight: 25
---

In the appdata directory under the game name. `%AppData%\Godot\app_userdata\PinGod-AddOns\Logs`.

They are built in Godot rolling logs with the `godot.log` always being the latest.

---
## Log location
*Image shows the users game save directory open in Sublime Text.*
![image](../../images/basicgame/basicgame-userdata-sublime.jpg)

---
#### Log example:

```
Godot Engine v3.4.2.stable.mono.official.45eaa2daf - https://godotengine.org
OpenGL ES 3.0 Renderer: Radeon RX 570 Series
OpenGL ES Batching: ON
 
PinGodGame:_EnterTree. getting cmd args
PinGodGamecmd line available: 0
GameSettings:loaded:Ok
PinGodGame:_EnterTree. log level: Debug
PinGodGame:window: size:766x478 pos:403,221, onTop: True
PinGodGame:window: project settings size: 1024x600
PinGodGame:looking for game patches. res://patch/patch_{patchNum}.pck . From 1. patch_1.pck, patch_2.pck
```

---
## Script Usage
---

[Game logging Class Reference](/pingod-addons/html/interfaceIPinballLogger.html)

Use from a pinGod reference or the static Logger in script like Logger.Debug

```
void Debug(params object[] what);

void Info(params object[] what);
	
void Warning(string message = null, params object[] what);

void Error(string message = null, params object[] what);

PinGodLogLevel LogLevel { get; }
```