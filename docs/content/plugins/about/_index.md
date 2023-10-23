---
title: "About Plugins"
date: 2022-12-26T15:26:15Z
draft: false
weight: 1
---

---
## Plugins / Autoload
Some `pingod-addons` have a plugin that you can enable or have an `AutoLoad` singleton when the plugin is enabled. These should work in any order you enable them.

*Open the project settings to view Plugins and Autoload*

![image](../../images/plugins/plugins-pingodaddons.jpg)

---
## AutoLoad
When some plugins are enabled they also have an Autoload class and they will be in this view. You can access these by the name in any scene script like `root/PinGodGame`.
![image](../../images/plugins/autoload-pingodaddons.jpg)

You can edit these Autoload scenes however you wish but you can also override them by duplicating any as needed. When the plugin is enabled it will look in the `res://autoload/` for the matching scene name to override. If you made a copy of `Resources.tscn` to `res://autoload/Resources.tscn` then your scene will override the default scene.

---
## How to override autoload scenes
If you wanted to edit and add more switches to the plugin then you could have your own copy of `Machine.tscn`. In Godot you can duplicate the default `Machine.tscn` like so:

*Note:It is better to do this kind of thing duplicating and moving files inside Godot. Godot will update any references as needed*

1. In the `FileSystem` pane filter files. Filter it for `machine`
2. The one we want is `Machine.tscn`. There will be just a few results.
3. Right click and Move/Duplicate To

![image](../../images/godot4-newproject/filter-and-duplicate.jpg)

4. Create and select `autoload` folder and copy the file here

![image](../../images/godot4-newproject/filter-and-duplicate-1.jpg)

5. Disable, then Enable the plugin in for the plugin to pick up your new AutoLoad scene. You will see a console message that your scene was found in the autoload.