# A. Paladin.

This component tweaks the Paladin base class as well as its kits. The general class and kit changes were for the most part borrowed from [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions) (KR from now on), so all credit to the authors.

note(s):
* Spell Revisions is a requirement. This is a technical requirement (we rely on some features of SR; this can, and probably will, be lifted in some future version) and a conceptual one, balanced around it.
* Compatibility with other spell adding mods (like iwdification) will be added in a future version.

# B. Class changes.

The changes are divided in groups.

## B. 1. Spellcasting.

As with KR, spellcasting is gained at level 4 and on par with clerics as far as casting level[^1]. However, the progression table is changed in several ways. First and foremost, paladins now gain spells up to priest level 5. The progression is also different, basically, two spells per two levels -- see [mxsplpal.2da](../resources/2da/mxsplpal.2da).

In terms of total number of spell slots, this means +1 spell at levels 1 and 2, and +3 spells at level 5 in comparison with Kit Revisions, for a total of 21 spell slots. Versus KR, the real gains are the level 5 spells. These are gained through levels 18 - 24, already in HLA territory, at or post-Underdark depending on party composition and xp gains. Level 5 contains some powerful spells: Chaotic Commands, True Seeing, Mass Cure, Magic Resistance, Righteous Fury and Champion's Strength, all worthy additions to the spellbook, but nothing game-breaking.

The available Paladin's spellbook is trimmed down. Spells removed from the Paladin's spellbook [^2]:

Level 1:
* Cause Light Wounds
* Command
* Doom
* Magical Stone

Level 2:
* Cause Moderate Wounds
* Hold Person
* Find Traps
* Silence

Level 3:
* Cause Serious Wounds
* Contagion
* Rigid Thinking
* Animate Dead

Level 4:
* Cause Critical Wounds
* Cloak of Fear
* Mental Domination
* Poison

Level 5:
* Greater Command
* Flame Strike
* Slay Living
* Repulsion

In comparison with KR, Gust of Wind, Glyph of Warding, Free Action and Farsight are added back to the spellbook. Removed the full line of cause wounds (lower level entries were missing in KR) and Find Traps. This left Animate Dead and Miscast Magic, so we took the course of action of taking the KR blurb from the Undead Hunter's description and drop Miscast Magic from their spellbook, while other paladins loose Animate Dead. For the level 5 spells, we dropped the obvious candidates.

note(s):
* At the moment these spells appear in spell selection screens; and I do not know how, or if it is even possible, to hide them.

### B. 1. 1. From IWD.

From iwd (installed via SCS or iwidification):

Level 1:
* Curse

Level 3:
* Cause Disease
* Circle of Bones

Level 4:
* Cloud of Pestilence

Level 5:
* Mass Cause Light Wounds

## B. 2. Immunities.

The immunities gained by a Paladin and its kits are a little different. All Paladin variations gain disease immunity at level 1[^3]. Then each version gains two different stat immunities at levels 3 and 7. Base, trueclass paladins gain immunity to fear and confusion.

note(s):
* not completely satisfied with immunity to confusion, but have not found a better idea yet.

## B. 3. Abilities.

Paladins gain the following abilities:

* Detect Evil at will at level 1.
* Protection from Evil at level 1.
* Smite Evil at level 1.
* Lay on Hands at level 3.
* Gains Aura of Protection at level 11.

Detect Evil is self-explanatory.

### B. 3. 1. Protection from Evil.

An innate version of the same-name spell, lasting 24 hours.

### B. 3. 2. Smite Evil.

Two options for scaling Smite Evil present themselves. Scale damage and keep the duration fixed at 1 round: this is the micro-management intensive option, depends a lot on hight apr, but it is useful even unto the end game as 5d6 magic damage is very good, especially against powerful enemies like SCS stoneskinned mages. Scaling duration to 5 rounds is less dependent on apr, is more activate-and-forget, but tapers off in usefulness in the end game where battles are fast and furious. As with KR, have chosen the first option, but arguments could go either way. It has the advantage of powering up melee attacks while not stacking with the likes of Whirlwind.

### B. 3. 3. Lay on Hands.

In KR, Lay on Hands has different effects per kit gained at levels 6 and 9. This is not yet implemented; the true paladin version is used throughout and it cures poison and disease. This seems to me to be the best option, as with SR, paladins gain at spell level 3 (character level 10), Cure Disease, Remove Paralysis and Break Enchantment.

### B. 3. 4. Auras.

At level 11, paladins gain Aura of Protection, imposing a -1 penalty on enemies' attack rolls. At level 14, it imposes a -1 penalty to enemies' damage rolls and at level 17, allies gain a +1 to all saves.

Same-type auras do not stack, fire once a round, and require no concentration to activate. Comparing with Songs: the latter require concentration, have more powerful effects and are available right from the starting level 1.

[^1]: conceptually incompatible with [Tweaks Anthology](https://github.com/Gibberlings3/Tweaks-Anthology) component "Alter Paladin Spell Progression Table".

[^2]: the spellbook is based on the divine spells made available by [Spell Revisions](https://github.com/Gibberlings3/SpellRevisions).

[^3]: makes a similar [atweaks](http://www.shsforums.net/files/file/949-atweaks-platform-independent/) component redundant.

# C. Cavalier.

Considerable changes from vanilla. The Cavalier now acts more like a general with fighting prowess (e.g. can attain mastery in some weapon proficiencies) and immunities to fear and charm, in exchange for one less spell per level and no access to Lay on Hands. The spellbook is also made by more unique, by both tailoring the deleted divine spells and the spells added.

note(s):
* KR adds Challenge Evil abilitty, which I do not like and will *not* add. A version of Shield Other is added as a new spell.

## C. 1. Spellcasting.

In comparison with (true) paladins, cavaliers gain Command, Cloak of Fear and Greater Command, but lose Miscast Magic, Holy Smite and Raise Dead. For new spells, they gain Shield of Faith, Shield Other, Divine Retaliation, Heroism and Hold the Line.

Shield of Faith is a fighting self-buff and Shield Other is essentially Sanctuary Other. Heroism is a party buff inspired by similar named spells and Hold the Line continues the theme of physical mobility and anti-dragon fighting by giving immunity to wing buffet.

## C. 2. Immunities.

Cavaliers gain immunity to fear and paralysis.

note(s):
* The idea is Cavaliers are physical (paralysis) and Inquisitors are mental (Charm).

## C. 3. Abilities.

Cavaliers gain all the paladin abilities, except Lay on Hands. Cavaliers can also attain mastery in long swords, bastard swords, flails and maces, and gain Sword and Shield Style specialization at level 1.

# D. Inquisitor.

Not many differences versus vanilla and KR.

note(s):
* *still* not happy. Casting spells is very useful, even more so with more spell slots and access to level 5 spells, so one more ability to compensate would be good, but what?

## D. 1. Immunities.

Inquisitors gain immunity to fear and charm.

## D. 2. Abilities.

Dispel Magic is now Dispel Evil, an aoe Dispel Magic against evil enemies at 1.5 times the level of the caster, as in a similar SCS component [^4]. In addition they gain Banish Evil, a version of SR's banishment against evil enemies and Iron Will, a permanent bonus to save vs. spells. True Sight is also made undispellable.

[^4]: The [SCS](https://www.gibberlings3.net/mods/tweaks/scs/) component "Reduce the power of Inquisitors' Dispel Magic" is, quite obviously, incompatible.

# E. Undead Hunter.

Keeps the vanilla Paralysis and Level Drain immunities but looses the extra thac0 and damage against undead, function now played by a new spell. In exchange, looses one spell per level, Lay on Hands and Auras.

## E. 1. Spellcasting.

In comparison with paladins, undead hunters gain Animate Dead, but lose Miscast Magic and Holy Smite. The latter has now a version, Smite Undead, gained at spell level 4 (character level 17), that bypasses magic resistance. They also get the new spells Halt Undead, Undead Bane, Exorcism and, at level 5, Animate Skeleton Warrior. The latter (as well as keeping Animate Dead) is to lean on the duality expressed in KR's kit description of using the undead to fight the undead.

## E. 2. Immunities.

As with KR, undead hunters gain immunity to paralysis and level drain.

## E. 3. Abilities.

Undead Hunters lose access to the paladin auras. Beyond KR, we give a bonus of +2 to Turn Undead level, gained at level 3.
