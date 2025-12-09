# Ranger Tweaks.

This component tweaks the Ranger base class as well as its kits. The general class and kit changes were for the most part borrowed from [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions).

# A. Class changes.

The base class's spellcasting is changed: spellcasting is gained at level 4 and on par with druids as far as casting level. The progression table changed to gain spells between levels 4 and 18 and the available spellbook is trimmed down. More precisely, the ranger's spellbook is trimmed of weapon, debuffs and elemental damage spells. The following spells from base SR are removed:

Level 1:
* Magical Stone
* Sunscorch
* Shillelagh

Level 2:
* Know Opponent
* Flame Blade
* Fire Trap
* Charm Person or Animal

Level 3:
* Call Lightning
* Icelance
* Contagion
* Rigid Thinking

Level 4:
* Ice Storm
* Call Woodland Beings

note(s):
* the function of Know Oponent is played by Hunter's Quarry.
* the function of Flame Blade is now played by Blades of Fire.
* the function of Fire Trap is now played by Snare.
* Rangers have access to Animal Empathy, so Charm Person or Animal is dropped.
* Call Woodland Beings is a powerful summon, so I prefer to leave it to druids and beastmasters.

Rangers gain:

1. Animal Empathy at will at level 1.
2. Hunter's Quarry once per turn at level 2.
3. Gains Woodland Stride at level 5.
4. Gains new spells to complement the spellbook: Blades of Fire (level 1), Snare (level 2) and Swift Haste (level 3).

note(s): all tables can be edited *before* installing the mod, but do not complain if you mess things up:
* the spell progression table is [Ranger spell progression](../resources/2da/ranger_spell_progression.2da).
* the list of deleted spells can be found in [Ranger spellbook](../resources/2da/ranger_spellbook.2da). This is also used for archers and stalkers; beastmasters have a specialized table.
* the stealth progression table is [Ranger skills](../resources/2da/ranger_skills.2da).
* the table of added spells is [Ranger new spells](../resources/2da/ranger_new_spells.2da).
* the proficiencies can be found in [Ranger proficiencies](../resources/2da/ranger_proficiencies.2da).
* the abilities can be found in [Ranger abilities table](../resources/2da/ranger_abilities.2da).

note(s):
* KR Tracking not implemented yet; for now, the HLA will have to do.

## A. 1. Dual and multiclasses.

The changes to spellcasting imply that some care is needed to handle dual and multi rangers. Specifically:

* Abilities must be added to the cleric ability table (`clabpr01.2da`) to (1) remove ranger casting level bonus (this handles the case Ranger -> Cleric) and (2) add protection from spells (this handles the case Cleric -> Ranger and also the multi Cleric + Ranger, although the latter was already handled in the way the abilities are doled out)

* A row must be added to the cleric ability table (`clabpr01.2da`) to trim the Cleric + Ranger spellbook on cleric level ups. The trimming must take into account the per level gains.

For this to take full effect (namely for Cleric + Rangers to get their level 4 spells), the gameplay option to limit Cleric + Rangers to level 3 spells *must* be disabled.

note(s): implementation note:
* we crawl through `spell.ids` and grab the references of non-deprecated, priest, druid-exclusive spells. Tested against SR, this seems to work, although there are a few spurious entries (but this is harmless).

# B. Kits.

## B. 1. Archer.

Trades melee for superior ranged fighting. An archer gains:

1. Called Shot: gained new effects Disarm and Trip.
2. Bow Mastery: +1 to ranged thac0 and damage at level 1 and then every 4 levels, to a maximum of +5 at level 16.
3. Evasion Archer: +1 ac vs. missiles every 4 levels to a maximum of +4 at level 16.
4. Ranger spells replaced by Feather Step, Fashion Arrows and Falcon's Eye.

note(s):
* the proficiencies can be found in [Archer proficiencies](../resources/2da/feralan_proficiencies.2da).
* the abilities can be found in [Archer abilities](../resources/2da/archer_abilities.2da).
* the table of added spells is [Archer new spells](../resources/2da/archer_new_spells.2da).

## B. 2. Stalker.

Vanilla stealth bonus and backstab ability retained. Ranger spells replaced by wizard's Invisible, Non-Detection, Improved Invisible and Shadow Door, suitably renamed.

note(s):
* the backstab bonus can be found in [Stalker backstab progression](../resources/2da/stalker_backstab.2da).
* the proficiencies can be found in [Stalker proficiencies](../resources/2da/stalker_proficiencies.2da).
* the abilities can be found in [Stalker abilities](../resources/2da/stalker_abilities.2da).
* the table of added spells is [Stalker new spells](../resources/2da/stalker_new_spells.2da).

## B. 3. Beastmaster.

Changed into a Conjurer with a special bond with his animal companion.

1. Spellbook: Has access to Call Woodland Beings and single-target elemental damage (Sunscorch, Icelance, etc.).
2. Special animal buffs: Animal Harmony, Animal Fang, Animal Growth and Animal Fury.
3. One innate casting of Animal Summoning I - IV.
4. Animal Companion: summons an increasingly powerful panther, starting at level 3. Each panther is an 1d6 HP pather with the thac0 and saves of a ranger of the same level and an ac of 7 with a +1 bonus per 2 HD.

Cumulative bonuses:
* Level 3: 3 HD, immunity to charm
* Level 6: 5 HD, +1 thac0, +2 movement rate
* Level 9: 7 HD, magical claws with base damage 1d8, 3/2 apr, immunity to sleep
* Level 12: 9 HD, +1 enchantment claws, 2 apr, +4 movement rate, immunity to fear
* Level 15: 11 HD, +1 damage bonus on the claws, 5/2 apr, immunity to death effects
* Level 18: 13 HD, claws crit on a 19, 3 apr, immunity normal weapons, regeneration 1 hp round

note(s):
* the list of deleted spells can be found in [Beastmaster spellbook](../resources/2da/beastmaster_spellbook.2da).
* the proficiencies can be found in [Beastmaster proficiencies](../resources/2da/beastmaster_proficiencies.2da).
* the abilities can be found in [Beastmaster abilities](../resources/2da/beastmaster_abilities.2da).
* the table of added spells is [Beastmaster new spells](../resources/2da/beastmaster_new_spells.2da).
