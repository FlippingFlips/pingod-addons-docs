---
title: "Godot - Installation"
date: 2022-12-26T15:26:15Z
draft: false
weight: 10
---

*If you're on windows, to make life easier make sure you have [Chocolatey](https://chocolatey.org/install) installed. This guide will leave snippets for `choco install`.*

---
### Godot 4.1.1-Mono
PinGod is using Godot4 Mono (C#). Godot is portable (no installation required) just the download. Installing through `choco` will add `godot` to your paths so you can use it on the command line.

`choco install godot-mono --version=4.1.1` - after install you can run `godot` to open the Godot project browser.

*Note: You can force that to install 32bit if you wish `--forceX86`*

---
### Dotnet SDK
Cross platform framework. If you already have a recent `dotnet sdk` installed then you can probably skip this step.

`choco install dotnet-sdk` or 6.0 `choco install dotnet-sdk --version=6.0.415`

*Note: You can force that to install 32bit if you wish `--forceX86`*

---
### Git
Use Git to clone repositories from Github, you don't need a Github account just the software to do this.

`choco install git`


---
### Visual Studio Debugging
[godot-csharp-visualstudio/releases/tag/v2.0.0](https://github.com/godotengine/godot-csharp-visualstudio/releases/tag/v2.0.0)
