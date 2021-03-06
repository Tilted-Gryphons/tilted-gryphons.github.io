---
title: pserver Addons and Macros
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---
**Classic Macros and Addons WILL NOT WORK on the old client!!!**

## Macros

### Giant Macro Database
[Huge list of Vanilla Macros](https://github.com/Meridaw/Vanilla-Macros)

### Useful Macros
Start Attack, does not show CDs or tooltip so I recommend using it on one ability you always use first, like Sunder Armor
```
/script if (not PlayerFrame.inCombat) then AttackTarget() end
/cast Maul
```
Max Zoom Camera, have to run each time you log in
```
/console CameraDistanceMaxFactor 5
```

## Addon Packs

### :fire: TG Addon Pack :fire:
[TG Addon Pack](https://drive.google.com/file/d/1RUKyIFiqlVsYhRpcENhBxyLBiNzpZdmn/view?usp=sharing)

Delete your addons folder if you have an older pack! This has improved versions of some addons! 
{: .notice--warning}

### elvUI-like Alternative
[pfUI](https://legacy-wow.com/vanilla-addons/pfui/)

## Other Resources

[Nice DB of Addons for 1.12.1](http://www.vanilla-addons.com/)

[List of Github-hosted Addons](https://forum.twinstar.cz/threads/github-list-of-vanilla-addons-1-12-1.123906/) 

Be sure to remove the '-Master' part of the file if you download a zip here! 
{: .notice--warning}

## Honorable Mentions

[Bartender2](https://legacy-wow.com/vanilla-addons/bartender-2/) - If you need a bar mod

## TG Addon Pack Usage

Feel free to disable addons your class does not need! 
{: .notice--info}

### AttackBar (Melee & Hunters)

```
# Menu
/abar
# Unlock
/abar unlock
# Disable Enemy Swing Timer
/abar mob
# Lock
/abar Lock
```

### BetterCharacterStats (All)
```
No menu, adds character sheet stats!
```

### BigWigs (All)
```
Boss Mod
Lots of options on the minimap

# Move Frames
Click minimap button
Plugins -> Bars -> Show Anchors
```

### BonusScanner (Healers)
```
Helper for NotGrid
```

### Cartographer (ALL)
```
Nothing to do here, better map
```

### Classic Snowfall (All)
```
Activates abilities on key-down instead of the default key-up!
```

### Clique (Healers)
```
Mouse-over healing
# Menu 
Open your spell book, it's a new, bottom tab with instructions!
```

### Cooldown Count (ALL)
```
Nothing to do here, shows cooldown timer on abilities and items
```

### CT_Unit_Frames (ALL)
```
Allows displaying numbers / percentages on blizz frames
# Menu
/uf
```

### DamageMeters (Optional)
```
Not sure what this does
```

### Decursive (You know Who You Are)
[Instructions](https://github.com/Zerf/Decursive)
```
Decurses?
```

### EnergyWatch v2 (Rogues/Druids)
```
Energy Tick Timer
# Menu
/ew
```

### Itemrack (All)
```
Useful for multiple gear sets (Nature res, etc)
Menu is on minimap, works like classic
```

### KLHThreatMeter (All)
```
yup.
```

### LagCast (Casters)
```
Configurable castbar for old client latency
# Menu
/lc
```

### MoveAnything! (All)
**Warning: moving bags causes lua errors!**
```
Move Blizzard unit Frames
# Menu
/move
```

### Natur ECB (Optional)
```
Tracks your debuffs on target and HoTs, takes some configuration
# Menu
/necb
```

### NotGrid (ALL)
```
Raid frames that work!
# Menu
/ng
Recommend:
  Highlight Target: On
  Show Power Bar: On
  Show Party in Raid: Off
  Show Blizz Frames: Off
```

### SUCC-ecb (All)
```
Enemy castbar, simpler than NECB and nice for melee/tanks
# Menu
/succecb
```

### Tank Buddy Enhanced (Melee/Tanks)
```
Taunt/Kick announcer
# Menu
/tb
```

