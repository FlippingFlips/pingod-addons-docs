---
title: "Score Entry"
date: 2022-12-26T15:26:15Z
draft: false
weight: 10
---

Basic Score mode with charachter selection for players at end of game

## Scene Tree breadown

- ColorRect = Black background color
- SelectedChar
- Label = HI_SCORE_ENTRY
- CenterContainer = Shows selected char center screen
- ColorRect2 = used as red marker under a letter

## Exports (ScoreEntry.cs)

- _includeZeroToNine
- _nameMaxLength 
- _playerMessage
_selectCharMargin = space when changing between chars with flippers
_selectedChar

## Overrides

### _Ready

Sets `IsPlayerEnteringScore` to true quits the scene if no players or `MoveNextPlayer`

### _Input

If scene is visible and `IsPlayerEnteringScore` then `flippers` and `start` button actions are watched to then be able to select letter.


---
## Creating custom Score Entry scene"
1. Filter Godot files by `ScoreEntry`
2. Duplicate the `ScoreEntry.tscn` and move to your `res://autoload` directory
3. Add the packed scene location, replacing any existing in the `res:autoload/Resources.tscn`
4. Add the new scene into the `Game.tscn` so it knows where your version is
5. Edit away without effecting the `addons` and script. You can take it further than cosmetic from here with a script.

Things you can try in the scene:

1. Setting a theme on the top control `ScoreEntry`, which will set all in the scene, provided you have made custom theme entries like `Label` themes.
2. Changing the labels font and colors, sizes, outlines, shadows.
3. If you change the size you can `Select Char Margin` to adjust the distance between the characters.