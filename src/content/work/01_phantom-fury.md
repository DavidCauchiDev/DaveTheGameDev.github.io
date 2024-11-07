---
title: Phantom Fury
publishDate: 2024-07-12 00:00:00
img: /assets/phantom_fury.webp
img_alt: Phantom Fury
description: |
  First Person Shooter developed by Slipgate Ironworks
tags:
  - Unreal Engine
  - C++
  - Gameplay
  - Tools
---

Shelly "Bombshell" Harrison is back in this highly interactive mix of first person action and road movie adventure. Embark on an adrenaline-fueled journey around the USA. Use an enormous arsenal of weapons and skills to battle treacherous soldiers and vile mutants, all while trying to save mankind.

[Learn More: 3D Realms Website](https://3drealms.com/games/phantom-fury/)

# My Contributions to Phantom Fury

I joined the Phantom Fury development team during the vertical slice phase, focusing primarily on interaction and combat systems. My role involved implementing a wide range of features across various game systems, adapting to the project's evolving needs, and refactoring systems to reduce technical debt.

## Weapon System

For Phantom Fury's weapon systems, I implemented a comprehensive selection of weapons that forms the core of the game's combat experience. My contributions include:

### Core Functionality
- Developed the core weapon system architecture, supporting a wide range of firearms and unconventional weapons capable of handling various fire modes (single shot, burst, automatic) and  a variety of projectile types
- Created a modular damage system allowing for different damage types (ballistic, explosive, energy, etc.) and environmental interactions

### Projectile and Throwable Weapons
- Developed a projectile system supporting behaviors such as:
  * Homing capabilities for certain weapon types
  * Ricocheting projectiles for trick shots and environmental puzzles
  * Area-of-effect explosions with customizable damage falloff
- Implemented throwable weapons such as the Bowling Bomb

### Weapon Variety
- Developed a diverse arsenal including but not limited to:
  * Traditional firearms (pistols, shotguns, assault rifles, SMGs)
  * Energy weapons with unique visual and gameplay effects such as the Photon Repeater
  * Exotic weapons like the bug-spitting Wasp Lung and the electrified foam-launching Foam Modulator
- Ensured each weapon felt unique and served a specific purpose in combat scenarios

### Upgrade System
- Designed and implemented the weapon upgrade system accessible through in-game Kiosks
- Implemented various upgrade types, such as increased damage, larger magazines, and special firing modes

This expanded weapon system laid the foundation for Phantom Fury's dynamic and engaging combat, providing players with a diverse and satisfying arsenal to tackle the game's challenges.
## Player Mechanics
- Designed and implemented the player upgrade system, including all individual upgrade functionalities available in the Kiosk
- Developed the Magnetic Shield and Punch arm features

## Interactive Elements
- Implemented the interactive terminal system, allowing designers to seamlessly script and control game flow and create some cool puzzles
- Implemented a fan-favorite feature: the old-school keypad requiring physical player interaction for code input
- I also implemented many smaller interactable elements

## Refactoring and Technical Debt Reduction
- Proactively refactored existing systems to improve code quality and maintainability
- Reduced technical debt by streamlining code from the vertical slice, enhancing performance, and simplifying future feature integration
- Worked closely with other developers to ensure refactored systems met project requirements without disrupting ongoing development

Throughout the development process, I demonstrated adaptability by moving between different systems, implementing features as required, and ensuring high-quality code through strategic refactoring efforts.