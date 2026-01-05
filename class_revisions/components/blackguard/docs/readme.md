# A. Blackguard.

KR does not do anything to Blackguards. This is something of an experimental component, as I have gone way way beyond the lore, especially in the unique spellbook -- see below for details. He is now a frontline fighter with debuffs and a few specialized self buffs, concentrating on the necromancy and conjuration schools, in the fire and poison elements.

note(s): all tables can be edited *before* installing the mod, but do not complain if you mess things up:
* the list of deleted spells can be found in [Blackguard spellbook](../resources/2da/blackguard_spellbook.2da).
* the proficiencies can be found in [Blackguard proficiencies](../resources/2da/blackguard_proficiencies.2da).
* the abilities can be found in [Blackguard abilities table](../resources/2da/blackguard_abilities.2da).
* the table of added spells is [Blackguard new spells](../resources/2da/blackguard_new_spells.2da).

## A. 1. Immunities.

Gain immunity to fear at level 3 and immunity to poison at level 7, the latter replacing level drain.

## A. 2. Abilities.

Receives specialized auras, similarly to paladins, but entirely offensive and working on enemies. The rest of the debuffs is moved to specific Blackguard spells. Both Absorb Health and Poison Weapon receive appropriate versions and Protection from Evil becomes Protection from Good.

note(s):
* for parity, add detect non-evil at will?

issue(s):
* Poison Weapon is a *new* ability so cre files of Blackguards must be patched to make the swap, and their scripts must be patched as well. Currently this is done in the main component but it will be separated into a different component to be installed after all cre adding mods. Script patching is not done yet either.

## A. 3. Spellcasting.

This is where the most dramatic changes are made. About 20 spells are dropped from the spellbook, including all healings and party buffs. Five single-target buffs receive remakes, from minor to complete overhauls. On top of this, new spells are added, that concentrate on debuffs that complement the auras -- see below. It is probably easier to just list what is left from SR's divine spellbook.

Level 1:

* Cause Light Wounds
* Command
* Doom
* Resist Fear

Level 2:

* Cause Moderate Wounds
* Hold Person
* Know Opponent
* Resist Elements
* Silence

Level 3:

* Animate Dead
* Cause Serious Wounds
* Contagion
* Dispel Magic
* Glyph of Warding
* Gust of Wind
* Invisibility Purge
* Miscast Magic
* Rigid Thinking
* Strength of One
* Unholy Blight

note(s):
* Undead-theme is inappropriate so remove Animate Dead?
* Bring back Break Enchantment and Remove Paralysis?

Level 4:

* Cause Critical Wounds
* Cloak of Fear
* Death Ward
* Farsight
* Free Action
* Mental Domination
* Negative Plane Protection
* Neutralize Poison
* Poison

Level 5:

* Flame Strike
* Greater Command
* Magic Resistance
* Protection from the Elements
* Repulsion
* Slay Living
* True Seeing

Changed self-buffs:

* Abyssal Armor, level 1: changes Armor of Faith; magic damage resistance is turned into fire resistance.
* Aid from Hell, level 1: replaces Aid. Moved to level 1 since Blackguards loose Bless. Long duration, long casting time.
* Dark Power, level 2: replaces Draw upon Holy Might. Long casting time.
* Abyssal Fury, level 4: replaces Righteous Fury; +4 strength, +4 movement speed, +20 hps and a fire damage melee effect.

Entirely new spells:

* Hellscorch, a version of Druid's sunscorch at level 1.
* Aura of Fear, level 1: a spell version of Wizard's Horror.
* Evil Chant, level 2: a debuff on enemies. Fast casting time.
* Evil Prayer, level 4: an improved Evil Chant, it is cumulative with it. Fast casting time.
* Miasma Cloud, level 4: a version of Wizard's Stinking Cloud, doing poison damage, disease attribute damage and half movement speed.
* Flaming Shield, level 4: a version of Wizard's Fire Shield.
* Abyssal Rage, level 5: essentially a spell version of berserk, replacing Champion's Strength.


Possible Additions:
* Abyssal Pact: add Death Knight (or something similar) at level 5? Better as an HLA?

Possible borrowings from IWD into EE:
* Curse: Evil Chant already exists.
* Cause Disease: Contagion already exists.
* Cloud of Pestilence: Miasma Cloud already exists, but could borrow projectile and animations?
* Blood Rage: Abyssal Rage already exists.
