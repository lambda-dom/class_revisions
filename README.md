# Class Revisions.

A WeiDU mod for BG2:EE revising and tweaking classes, following the, now seemingly abandoned, [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions) mod.

For documentation see the [docs](./class_revisions/docs/readme.md).

Acknowledgement(s):

  * If you find anything worthwhile in the mod blame my predecessors, the authors of [Refinements](https://github.com/UnearthedArcana/refinements) and especially [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions). I am just a coding monkey and the only originality I can clain are the eventual bugs (but as everyone knows, any report of bugs in my mods is just slander propagated by my enemies).

# A. Installation.

## A. 1. Download.

Either download the latest release from the releases on the sidebar or `git clone`. If you download the mod by clicking the code button or `git clone`, the download will be missing the `weidu_library`, so it will not work correctly. This must be installed separately -- see instructions below.

## A. 2. Installation.

This is a standard [WeiDU](https://github.com/WeiDUorg/weidu) mod. Just copy the `class_revisions` folder (the one containing the `class_revisions.tp2` file) to your BG installation, and assuming you have WeiDU installed and in the executable path, drop down to the command line and:

```bash
weinstall class_revisions
```

note(s):

* See [A New Player’s Guide to Installing and Playing Mods](https://www.gibberlings3.net/forums/topic/33164-a-new-player%E2%80%99s-guide-to-installing-and-playing-mods) for more information on modding BG2.

## A. 3. Requirements.

This mod requires [Spell Revisions](https://github.com/Gibberlings3/SpellRevisions). While it technically does not require it, [Item Revisions](https://github.com/Gibberlings3/ItemRevisions) is recommended. Playing BG without [SCS](https://www.gibberlings3.net/mods/tweaks/scs/) installed is in my view, quite pointless, even though SCS is these days a massive mod with bugs that can take quite some time to iron out; the envisioned difficulty levels are core-hardcore. Insane *may* be doable but I have not tested or have any intentions of testing; even more so for Legacy of Bhaal.

# B. Current State and Future Plans.

The mod is in alpha stage, because while the basic design is set there are some details to be hashed out, especially around the Blackguard kit (which is why it is installed as a separate component).

In comparison with KR, for global components, the weapon styles component is in, but nothing else: no thac0, saves, xp, etc. changes. Some of these are taken care of by other mods, e.g. [Tweaks Anthology](https://github.com/Gibberlings3/Tweaks-Anthology), so *probably* they will not covered.

Currently, I prefer to leave thieves and bards to [Rogue Rebalancing](https://www.shsforums.net/files/category/62-rogue-rebalancing), as I think the mod has done a stellar job with them. Plus, it also has a bunch of other content. There are some changes planned to Fighters, Mages, Sorcerers, Clerics and Druids, but these are relatively low-key, as changes to these core classes have the potential to muck up [SCS](https://github.com/Gibberlings3/SwordCoastStratagems), which is a no-no for me. I like only one half of [Refinements](https://github.com/UnearthedArcana/refinements) changes to Sorcerer HLAs, so have to think what to do about the other half, at any rate SCS compatibility is a must.

This leaves Monks; I like both what KR and [Monk Overhaul](https://forums.beamdog.com/discussion/33618/mod-monk-overhaul) have done with monks but have no firm design yet.

## B. 1. Issues.

There are some unresolved issues. The ones I am aware of:

* Paladins and Rangers get trimmed down spellbooks with some unique additions, but these differences are not reflected in the character creation screens. I do not know how to do this, or even if it can be done, so for now have to suffer the jank.

* The way the spellbooks are updated at level up is by applying an ability with a spell removal opcode. The implementation was copied from KR and uses *delayed* timing; some early testing showed that with *instant* timing sometimes did not work. So should wait a couple of seconds after level up to get the updated spellbook.
