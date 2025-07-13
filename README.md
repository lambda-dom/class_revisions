# Class Revisions.

A WeiDU mod for BG2:EE revising and tweaking classes, following the, now seemingly abandoned, [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions) mod.

# Current State and Future Plans.

In comparison with KR, for global components, the weapon styles component is in, but nothing else: no thac0, saves, xp, etc. changes. Some of these are taken care of by other mods, e.g. [Tweaks Anthology](https://github.com/Gibberlings3/Tweaks-Anthology), so *probably* they will not covered.

Currently, I prefer to leave thieves and bards to [Rogue Rebalancing](https://www.shsforums.net/files/category/62-rogue-rebalancing), as I think the mod has done a stellar job with them. Plus, it also has a bunch of other content. There are some changes planned to Mages, Sorcerers, Clerics and Druids, but these are relatively low-key, as changes to these core classes have the potential to muck up [SCS](https://github.com/Gibberlings3/SwordCoastStratagems), which is a no-no for me. I like only one half of Refinements changes to Sorcerer HLAs, so have to think what to do about the other half, at any rate SCS compatibility is a must.

This leaves:

* Rangers: a version is mostly finished, except the beastmaster kit.
* Ranger HLA's: initial implementation is done, but still not quite satisfied with it.
* Monks: I like both what KR and [Monk Overhaul](https://forums.beamdog.com/discussion/33618/mod-monk-overhaul) have done with monks.

# A. Installation.

## A. 1. Download.

Either `git clone` or download the latest release from the releases on the sidebar. If you download the mod, by clicking the code button, the downloaded zip will be missing the `weidu_library`, so it will not work correctly.

## A. 2. Installation.

This is a standard [WeiDU](https://github.com/WeiDUorg/weidu) mod. Just copy the `class_revisions` folder (the one containing the `class_revisions.tp2` file) to your BG installation, and assuming you have WeiDU installed and in the executable path, drop doen to a command line and do:

```bash
weinstall class_revisions
```

note(s):

* See [A New Player’s Guide to Installing and Playing Mods](https://www.gibberlings3.net/forums/topic/33164-a-new-player%E2%80%99s-guide-to-installing-and-playing-mods) for more information on modding BG2.

## A. 3. Mod order.

# B. Global components.

This group of components does not apply to any class in particular, and is instead global in nature.

## B. 1. Weapon Styles.

Changes the bonuses provided by style proficiencies by overriding [the table stylbonu.2da](./class_revisions/components/weapon_styles/resources/2da/stylbonu.2da). It is a modest attempt at buffing styles other than Two Weapons and give some incentive, even if a modest one, to pick them up.

# C. Class Revisions.

This group of components revises classes and their kits, from relatively minor ways to complete overhauls.

## C. 1. Paladin.

An overhaul of the Paladin class and its kits, generally following [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions). See [Paladin docs](./class_revisions/components/paladin/docs/readme.md) for more information.

requirement(s):

* intended to work alongside with [Spell Revisions](https://github.com/Gibberlings3/SpellRevisions), it requires it.

## C. 2. Blackguard.

# D. HLA's.

## D. 1. Paladin HLA's.

A new set of HLA's for Paladins, Blackguards included, borrowed in part from [Refinements](https://github.com/UnearthedArcana/refinements). See the [Paladin HLA's docs](./class_revisions/components/paladin_hlas/docs/readme.md) for more information.

requirement(s):

* intended to work alongside with [Spell Revisions](https://github.com/Gibberlings3/SpellRevisions), it requires it.

## D. 2. Blackguard HLA's.
