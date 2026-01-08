# Class Revisions.

A WeiDU mod for BG2:EE revising and tweaking classes, following the, now seemingly abandoned, [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions) mod. For now, only Paladins and Rangers are covered in full, while Mage and Sorcerer have tweaks and revisions inspired from [Refinements](https://github.com/UnearthedArcana/refinements).

For documentation on each component start at the [docs](./class_revisions/docs/readme.md). They are, like the rest of the mod, still in alpha but it should give a decent idea of what my aim is.

Acknowledgement(s):

  * If you find anything worthwhile in the mod blame my predecessors, the authors of [Refinements](https://github.com/UnearthedArcana/refinements) and especially [Kit Revisions](https://www.gibberlings3.net/forums/forum/168-kit-revisions), from whom I have shamelessly stolen. I am just a coding monkey and the only originality I can claim are the eventual bugs -- although, quite emphatically, there are no bugs in the mod and any reports of such is just malicious slander spread by my enemies.

# A. Installation.

## A. 1. Download.

Either download the latest release from the releases on the sidebar or `git clone`. If you download the mod by clicking the code button or `git clone`, the download will be missing the [weidu_library](https://github.com/lambda-dom/weidu_library), so it will not work correctly. This must be installed separately -- see instructions below.

## A. 2. Installation.

This is a standard [WeiDU](https://github.com/WeiDUorg/weidu) mod. Decompress the zip and dump the contents (the folders `weidu_library` and `class_revisions` and the exe installer if on Windows; the other files, like `LICENSE`, etc. are not strictly needed for the mod to function) in the BG game directory, the one containing the `chitin.key` file. Assuming you have WeiDU installed and in the executable path, drop down to the command line and:

```bash
weinstall class_revisions
```

For Windows users who do not like the command line (seriously: learn to love the command line) an exe installer is provided. Double-click it and proceed as usual.

note(s):

* See [A New Player’s Guide to Installing and Playing Mods](https://www.gibberlings3.net/forums/topic/33164-a-new-player%E2%80%99s-guide-to-installing-and-playing-mods) for more information on modding BG2.

## A. 3. Requirements.

This mod is only for IWD EE, BG2 EE and EET. *Maybe*, the non-HLA components can also be used on BG1 EE but I have not kept track of what is needed or not from base, and I have not even checked whether it installs on bare BG1 EE. It also has [Spell Revisions](https://github.com/Gibberlings3/SpellRevisions) as a hard requirement -- it will *not* install if SR's main component is not present.

While it technically does not require it, [Item Revisions](https://github.com/Gibberlings3/ItemRevisions) is recommended. Playing BG without [SCS](https://www.gibberlings3.net/mods/tweaks/scs/) installed is in my view, quite pointless, even though SCS is these days a massive mod with bugs that can take quite some time to iron out; the envisioned difficulty levels are core-hardcore. Insane *may* be doable but I have not tested it or have any intentions of testing it; even more so for Legacy of Bhaal.

# B. Issues.

The mod is in alpha stage, because while the basic design is set there are some details still to be hashed out, especially around the Blackguard (which is why it is installed as a component separate from the main Paladin component) and the Beastmaster kits (e. g. summon stats). There is still room to add a couple more specialized spells to each kit and Inquisitors could maybe get a few more bennies -- if you have any good idea submit an issue, but be prepared to be rejected on flimsy grounds like "vibes" and "personal taste".

There are also some unresolved, or potentially problematic, issues. The ones I am aware of:

* Paladins and Rangers get trimmed down spellbooks with some unique additions, but these differences are not reflected in the character creation screens. I do not know how to solve this; most likely, if there is a solution, it will require UI patching which I have never done, so for now the user will have to suffer the jank.

* The way the spellbooks are updated at level up is by applying an ability with a spell removal opcode. The implementation was copied from KR and uses *delayed* timing by 1 second; some early testing showed that with *instant* timing sometimes it did not work correctly. So should wait a couple of seconds after level up to get the updated spellbook.

* Spellcasting changes to rangers entails all sorts of issues for dual and muticlasses; some early testing indicates that these have been solved but do not be surprised if there are some bugs lurking as the solution is moderately complex.

* All the new spells and items use vanilla icons, with one spell using an icon from SR; I have zero graphical talents, so barring a gentle soul making some nice icons for the mod, it will stay that way. I also have poor writing skills and English is not my native language, so any help in that department would be much appreciated. You know the drill -- submit patches.

* Balancing is an ever-present concern. I would say that in comparison to vanilla, all the classes and kits got more powerful, so the question is how much more powerful. As a general rule, I prefer underpowered to overpowered, but if a choice has to be made, fun over both.

* Modder issues: currently, to make use of `spell.ids` to manage resource references, we dump all spells in the `spcl` namespace via `ADD_SPELL`, crowding it out. If this proves to be problematic (especially relevant for megamod installs), we might consider switching to some other scheme like the extended naming scheme of SCS (this *may* also solve the first issue).

* Modding compatibility: my BG installs tend to be rather slim by megamod standards, so compatibility with other mods has not been extensively tested. Starting with the obvious: it is conceptually, if not technically, incompatible with any other mods that aim to do the same thing; install only the one you want or be prepared to suffer in purgatory and suffer alone.

The mod also does straight override, so it should be installed relatively early. Some things could be modified for patching (e. g. clab tables; will get there, eventually), but in most cases patching is so extensive that would be functionally equivalent to a straight override.

Unless there is some very cogent reason not to, I try to be as accomodating of other mods as possible, the only problem being determining who exactly is in the best place to ensure compatibility. The answer is, can only be: to be determined on a case by case basis.

* I am a linux user and I do not have a Windows or Mac available and do not intend to get one, so proper testing on those OS'es will have to rely on the lab ra -- uhh, the mod users. I do not foresee any problems but one never knows; at any rate, you know the drill -- submit patches.

# C. Future Plans.

In comparison with KR, for global components, the weapon styles component is in, but nothing else: no thac0, saves, xp, etc. changes. Some of these are taken care of by other mods, e.g. [Tweaks Anthology](https://github.com/Gibberlings3/Tweaks-Anthology), so *probably* they will not be covered.

Currently, I prefer to leave thieves and bards to [Rogue Rebalancing](https://www.shsforums.net/files/category/62-rogue-rebalancing), as I think the mod has done a stellar job with them. Plus, it also has a bunch of other content. Some tweaks to Mage and Sorcerer HLA's are implemented, and there are some changes planned to Fighters, Clerics and Druids, but these are relatively low-key, as changes to these core classes have the potential to muck up [SCS](https://github.com/Gibberlings3/SwordCoastStratagems), which is a no-no for me. This leaves Monks; I like both what KR and [Monk Overhaul](https://forums.beamdog.com/discussion/33618/mod-monk-overhaul) have done with monks but have no firm design in mind yet.
