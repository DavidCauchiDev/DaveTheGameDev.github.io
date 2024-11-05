---
title: Unreal Shooter Weapon System
publishDate: 2024-07-18 12:55:00
img: /assets/blog/unreal_weapon_system.png
img_alt: Unreal Shooter Weapon System
category: Unreal Engine
description: |
  A shooter weapon system made for Unreal
tags:
  - Unreal Engine
  - C++
---

# Overview

If you are using Unreal Engine, you most likely have had a desire to make a shooter style game be that first person or third, maybe even top-down. 

The goal of this post is to showcase a weapon system I developed in hopes it may provide some insight on a good direction for you to head in.


## Why not use lyra?

Lyra is a massive project designed to be a modular learning environment to showcase how to make an online arena shooter.
The end result is quite a large codebase with many features you probably won't need. This tends to work against you and navigating the project in your IDE or in Editor tends to take far too long for those getting started with the engine.

## How is my way better?

In all honesty, it probably isn't. This is what works for me after several years of working on an FPS that was plagued with tech debt and overly generic systems, or worse some credit to me, overly hardcoded systems that make it a pain for designers to change things. 

At the end of the day, I reccomend whatever works well for you.

## The way I do things.

I decided on using an event based workflow that tells external listeners something has occured vs the weapon directly telling its owner it did something. This has solved two major issues I have previously run into. Coupling directly with the owners code, resulting in a large mess of several different actors being directly referenced when in reality, the weapon should not care who or what has it equipped. 

The second thing is now we can use a single weapon system for anything that requires a weapon to be attached. This means Players, AI, Turrets, or even your mum can get in on the action!

### The core code.

The actual weapon logic is kept barebones and is free of side effect code (VFX, SFX, Animations). All we need is a single C++ class that allows actors to invoke interactions.

```cpp

	UFUNCTION(BlueprintCallable)
	void StartFire();

	UFUNCTION(BlueprintCallable)
	void StopFire();

	UFUNCTION(BlueprintCallable)
	void Reload(bool bFastReload);

	UFUNCTION(BlueprintCallable)
	void SetFireMode(EFireMode FireMode);

	UFUNCTION(BlueprintCallable)
	void CycleFireMode();

	UFUNCTION(BlueprintCallable)
	void ChamberRound();
```
