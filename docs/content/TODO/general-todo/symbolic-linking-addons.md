---
title: "Symbolic - Linking addons"
date: 2022-12-26T15:26:15Z
lastmod: 2022-10-26T15:26:15Z
draft: false
weight: 45
---

TODO: remove basic game guide, add for new projects and how to reuse same code

To run the `pingod-basigame` project in the examples folder you will need the `addons` directory linked or copied.

These `addons` contain base files and pinball framework that a game will use.

---
#### Link the AddOns
---

You can copy the `addons` directory to your project (`pingame-basicgame` in this example), but it's better to use a `symbolic link` to the addons so we are not duplicating files and you can keep the same addons across projects.

---

1. Running the `_link_addons.bat` launcher file will symbolic link the `addons`. A shortcut `addons` folder will be added in the Godot project.

2. This will just flash up and disappear, but you will see a new folder shortcut created called `addons`

![image](../../images/basicgame/basicgame-project-files.jpg)

---
#### Opening shortcut
---

If you open the new `addons` shortcut it will show you the files that are in `pingod-addons\addons`.

![image](../../images/basicgame/basicgame-addons.jpg)


*This shortcut can be removed without harming the files where the directory is linked from.*