# A. Paladin.

This component tweaks the Paladin base class as well as its kits. The general class and kit changes were for the most part borrowed from [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions) (KR from now on), so all credit to the authors.

note(s):
* Spell Revisions is a requirement. This is both a technical requirement (we rely on some features of SR) and a conceptual one, as the mod is balanced (or what in my head passes for balance -- the reader must make his judgment) around it.

# B. Class changes.

The changes are divided in groups.

note(s): all tables can be edited *before* installing the mod, but do not complain if you mess things up:
* the spell progression table is [Paladin spell progression](../resources/2da/paladin_spell_progression.2da).
* the list of deleted spells can be found in [Paladin spellbook](../resources/2da/paladin_spellbook.2da).
* the proficiencies can be found in [Paladin proficiencies](../resources/2da/paladin_proficiencies.2da).
* the abilities can be found in [Paladin abilities table](../resources/2da/paladin_abilities.2da).

## B. 1. Spellcasting.

As with KR, spellcasting is gained at level 4 and on par with clerics as far as casting level[^1]. However, the progression table is changed in several ways. First and foremost, paladins now gain spells up to priest level 5. The progression is also different, basically, two spells per two levels -- see [Paladin spell progression](../resources/2da/paladin_spell_progression.2da).

In terms of total number of spell slots, this means +1 spell at levels 1 and 2, and +3 spells at level 5 in comparison with KR, for a total of 21 spell slots. Versus KR, the real gains are the level 5 spells. These are gained through levels 18 - 24, already in HLA territory, at or post-Underdark depending on party composition and xp gains. Level 5 contains some powerful spells: Chaotic Commands, True Seeing, Mass Cure, Magic Resistance, Righteous Fury and Champion's Strength, all worthy additions to the spellbook, but nothing game-breaking.

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

### B. 1. 1. From IWD.

From iwd (installed via SCS or iwidification), the following spells are removed:

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

In KR, Lay on Hands has different effects per kit gained at levels 6 and 9. In this mod, the true paladin version is used throughout and it cures poison and disease. This seems to me to be the best option, as with SR, paladins gain at spell level 3, Cure Disease, Remove Paralysis and Break Enchantment. This is subject to revision and I may end up implementing it, if only I can gather enough willpower to do it.

### B. 3. 4. Auras.

At level 11, paladins gain Aura of Protection, imposing a -1 penalty on enemies' attack rolls. At level 14, it imposes a -1 penalty to enemies' damage rolls and at level 17, allies gain a +1 to all saves.

Same-type auras do not stack, fire once a round, and require no concentration to activate. Comparing with Bard's songs: the latter require concentration, have more powerful effects and are available right from the start at level 1.

# C. Cavalier.

Considerable changes from vanilla. The Cavalier now acts more like a general with fighting prowess (e.g. can attain mastery in some weapon proficiencies) and immunities to fear and charm, in exchange for one less spell per level and no access to Lay on Hands. The spellbook is also made more unique, by both tailoring the deleted divine spells and the spells added.

note(s):
* KR adds Challenge Evil abilitty, which I do not like and will *not* add. A version of Shield Other is added as a new spell.

note(s): all tables can be edited *before* installing the mod, but do not complain if you mess things up:
* the list of deleted spells can be found in [Cavalier spellbook](../resources/2da/cavalier_spellbook.2da).
* the proficiencies can be found in [Cavalier proficiencies](../resources/2da/cavalier_proficiencies.2da).
* the abilities can be found in [Cavalier abilities table](../resources/2da/cavalier_abilities.2da).

## C. 1. Spellcasting.

In comparison with (true) paladins, cavaliers gain Command, Cloak of Fear and Greater Command, but lose Miscast Magic, Holy Smite and Raise Dead. For new spells, they gain Shield of Faith at spell level 1, Shield Other and Divine Retaliation at spell level 2 and Heroism and Hold the Line at spell level 3.

Shield of Faith is a fighting self-buff and Shield Other is essentially Sanctuary Other. Heroism is a party buff inspired by similar named spells and Hold the Line continues the theme of physical mobility and anti-dragon fighting by giving immunity to knockback.

## C. 2. Immunities.

Cavaliers gain immunity to fear and paralysis.

note(s):
* The idea is Cavaliers are physical (paralysis) and Inquisitors are mental (Charm).

## C. 3. Abilities.

Cavaliers gain all the paladin abilities, except Lay on Hands. Cavaliers can also attain mastery in long swords, bastard swords, flails and maces, and gain Sword and Shield Style specialization at level 1.

# D. Inquisitor.

Not many differences versus vanilla and KR.

note(s):
* *still* not happy. Casting spells is *very* useful, even more so with more spell slots and access to level 5 spells, so one more ability to compensate would be good, but what?

## D. 1. Immunities.

Inquisitors gain immunity to fear and charm.

## D. 2. Abilities.

TODO:
* Add a Shield of the Archons innate ability scaling with level.
* Add immunity to confusion? Instead of fear or along with charm?

Dispel Magic is now Dispel Evil, an aoe Dispel Magic against evil enemies at 1.5 times the level of the caster, as in a similar SCS component [^4]. In addition they gain Banish Evil, a version of SR's banishment against evil enemies and Iron Will, a permanent bonus to save vs. spells. True Sight is also made undispellable.

# E. Undead Hunter.

Keeps the vanilla Paralysis and Level Drain immunities but looses the extra thac0 and damage against undead, function now played by the new Undead Bane ability. Protection from Evil and Smite Evil become anti-undead dedicated abilities, with the latter now becoming an aoe magic damage bypassing mr. Differently from vanilla and KR, the Undead Hunter regains Lay on Hands. In exchange, looses one spell per level, Lay on Hands and Auras.

note(s): all tables can be edited *before* installing the mod (do not complain if you mess things up):
* the list of deleted spells can be found in [Undead Hunter spellbook](../resources/2da/undead_hunter_spellbook.2da).
* the proficiencies can be found in [Undead Hunter proficiencies](../resources/2da/undead_hunter_proficiencies.2da).
* the abilities can be found in [Undead Hunter abilities table](../resources/2da/undead_hunter_abilities.2da).

## E. 1. Spellcasting.

In comparison with Paladins, Undead Hunters gain Animate Dead, but lose Miscast Magic and Holy Smite. Holy Smite has its counterpart in the Smite Undead ability -- see above.

For new spells, they get Halt Undead at spell level 1 (bypasses mr), Magic Circle against Undead at spell level 2, Exorcism at spell level 3 and Animate Skeleton Warrior at spell level 4. The latter (as well as keeping Animate Dead) to lean on the duality expressed in KR's kit description of using the undead to fight the undead.

## E. 2. Immunities.

As with KR, Undead Hunters gain immunity to paralysis and level drain.

## E. 3. Other abilities.

Beyond KR, we give a bonus of +2 to Turn Undead level, gained at level 3.

[^1]: conceptually incompatible with [Tweaks Anthology](https://github.com/Gibberlings3/Tweaks-Anthology) component "Alter Paladin Spell Progression Table".

[^2]: the spellbook is based on the divine spells made available by [Spell Revisions](https://github.com/Gibberlings3/SpellRevisions).

[^3]: makes a similar [atweaks](http://www.shsforums.net/files/file/949-atweaks-platform-independent/) component redundant.

[^4]: The [SCS](https://www.gibberlings3.net/mods/tweaks/scs/) component "Reduce the power of Inquisitors' Dispel Magic" is, quite obviously, incompatible.
