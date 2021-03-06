---
title: Private Server GM Commands
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---
**Make sure and preface macros with /ra otherwise they will fail when you are dead!**

### Basic

List commands you can access
```
.help
```

Disable GM mode
```
.gm off
```

Kill a mob/player/yourself
```
.die
```

Revive a player/yourself
```
.revive
```

Respawn mob
```
.respawn
```

Freeze a mob/player
```
.freeze
```

Unfreeze a mob/player
```
.unfreeze
```

Teleport to a named location
```
.tele <name>
.tele ironforge
.tele AQ
```

Teleport a player to your location
```
.namego <player>
```

Teleport yourself to a player's location
```
.goname <player>
```

### Helping Players

Give and item by targeting the player and using the item ID from wowhead (Quantity is optional)
```
.additem <item-id> <qty>
```

Spawn a mob for hunter to train, get mob ID form wowhead
```
.npc summon <npc-id>
```

Summon hunter a mob to tame - Tip: .freeze while they tame it
```
# Blackrock Worg
.npc summon 9696

# Brokentooth
.npc summon 2850

# Son of Hakkar
.npc summon 11357
```

Level and max hunter pet loyalty macro, 6 loyalty levels!
```
.npc changelevel 60
.pet loyalty 100000
.pet loyalty 100000
.pet loyalty 100000
.pet loyalty 100000
.pet loyalty 100000
.pet loyalty 100000
```

### Raid Commands

Reset an instance (takes ~5 mins)
```
.server resetallraids
```

Teleport entire raid to your location
```
.raid onme
```

Kill the entire raid (force wipe)
```
.raid die
```

Revive/Repair the entire raid on your location
```
.raid revive
```

Reset entire raid's cooldowns
```
.raid cooldown
```

Buff entire raid
```
.raid buff <combo>

# Raid buffs are additive so you can mix n' match buffs
1   Class Buffs
2   Elixirs/Food
4   Flasks
8   Ony / ZG
16  Tribute
32  Blasted Lands / Zanzas
64  Songflower
128 Darkmoon Faire

# Ex. 1: You want Class buffs(1) + Elixirs/Food(2) + Tribute buffs(16) = (19)
.raid buff 19

# Ex. 2: You want Class buffs(1) + Elixirs/Food(2) + Ony / ZG(8) + Songflower(64)
.raid buff 75

#Ex. 3: You want it all!
.raid buff 255
```

Change character models of the entire raid
```
.raid morph <model>

# Ex. 1: Make the entire raid Mr. Bigglesworth
.raid morph 16622
```

Reset entire raid's character models
```
.raid demorph
```

### My Raid Setup

I have macros for all the 'safe spots' in the raid
```
# Skeram
/ra .go -8203.744141 2138.245117 129.131927
# Bug Trio
/ra .go -8592.382813 2078.920898 -1.553985
# Sartura
/ra .go -8350.530273 1803.115967 -1.534063
# Fankriss
/ra .go -7986.662109 1234.879761 -69.375587
# Viscidus
/ra .go -7986.911621 1062.900513 -23.842262
# Huhuran
/ra .go -8616.300781 1575.261719 -80.751152
# Twin Emps
/ra .go -8974.216797 1320.926636 -104.251648
# Ouro
/ra .go -9050.949219 2020.871948 -59.579689
# C'Thun
/ra .go -8628.756836 1907.371826 108.565636
```

I macro a few common things togther
```
# Macro 1 (Die)
/ra .raid die

# Macro 2 (Revive/Repair)
/ra .raid revive

# Macro 3 (Buff/Reset CDs)
/ra .raid buff 7
/ra .raid cooldown
```

### Typical Order of Operation

*!!! Make sure GM Mode is OFF !!!*

1. teleport to AQ
  * ```.tele aq```
2. Bring the raid
  * ```.raid onme```
3. Buff everyone
  * ```.raid buff 7```
4. If we are not going to kill the boss, force wipe
  * ```.raid die```
5. Teleport myself to the safespot (still dead)
  * ```<tele macro>```
6. Revive the raid
  * ```.raid revive```
7. Buff and reset CDs
  * ```.raid buff 7```

### Known Issues and Workarounds

```
Sometimes the boss may not drop combat so you need to target boss and
.die

Then, respawn the boss by targeting his corpse and
.respawn
```

```
Bosses with Adds do not respawn correctly (Sartura, Bug Trio)

You need to force a wipe
.raid die

Then revive only yourself by targeting yourself with
.revive

Aggro the Boss in question, let yourself die. The boss should reset correctly
```

```
Adds in bug tunnel need to be killed before pulling Fankriss

Use the AoE clearing apility:
<need to remember>
```

```
Pulling Emps requires clearing the trash before Huhuran (Anubisaths)

.die them
```

```
Door to emps can stick closed if you have GM mode On

Use tele macro to pull raid through.
```


