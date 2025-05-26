---
title: Path of the Warmage  
publishDate: 2025-05-26 00:00:00  
img: /assets/potw.webp  
img_alt: Path of the Warmage  
description: |
  Real-time tactical fantasy game made during a game jam. Grid-based combat, pathfinding, puzzles, and portals.  
tags:  
  - Game Jam  
  - Custom Engine 
  - Odin
  - Pathfinding  
  - Puzzle Design  
  - Level Design  
---

# Path of the Warmage

*Path of the Warmage* was a short but solid game jam project — a tactical top-down game where you guide a spell-slinging warmage through puzzle-filled levels using smart movement and environmental tricks.

I focused mostly on gameplay programming, but also did some design work along the way.

## My Contributions

### 🔍 Navigation & Movement

- Implemented **A\*** for grid-based pathfinding.
- Implemented path smoothing using a modified **Bresenham’s algorithm** to clean up jagged paths and make the movement look more fluid and intentional.

### 🎮 Gameplay Features

- Built the **key-and-lock puzzle system** to gate progression and add light puzzle elements.
- Added **teleportation portals** and other traversal mechanics to expand how players move through each level.
- Hooked up smaller gameplay elements like interactables, gates, triggers, etc.

### 🗺 Level Design

- Designed a few of the early levels to show off the mechanics and give the player a clean on-ramp to the puzzle logic.
- Focused on clarity, pacing, and giving the player a few fun “a-ha!” moments even in a short jam window.

## 🙌 Special Thanks

Big thanks to **Lucas Perlind** for building out the core engine and handling all the heavy lifting on low-level systems. The game wouldn’t have been possible without him.


---

[Play it on Itch.io →](https://perlind.itch.io/path-of-the-warmage)

