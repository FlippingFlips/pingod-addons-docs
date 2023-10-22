---
title: "ScoreMode - Scene"
date: 2022-12-26T15:26:15Z
draft: false
weight: 5
---

Basic Score Mode for multi players. `Game/Modes/ScoreMode`

---
## Exports (ScoreMode.cs)
---

- _single_player_p1_visible 	= false . Show Player ones ScoreP1 label if set to true. Normally in a pinball the scorep1 would not display with main score unless multi-player
- _show_main_score_multiplayer  = true

Select NodePaths for the following export properties. A NodePath here should be a label that is added to your layout. If you have 8 players then create 8 labels and add them to the array in godot editor.

- _ballInfoLabel
- _playerInfoLabel
- _scoreLabel
- _score Labels

---
## Scene Tree breadown
---

- BackgroundColor = Simple green color
- CenterContainer with logo and `ScoreMain` label in center screen
- Score Labels
- PlayerInfoLabel
- BallInfoLabel
- CreditsLabel


---
## Creating / Modding your own ScoreMode
---

See [Create Custom Score Mode](./tips-guides/custom-score-mode/)