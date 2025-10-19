# A. Technical side.

* Lots of updates needed to latest weidu_library.

# B. Bugs.

* Blackguard's Poison Weapon ability does not override the existing one and this leads to the old ability still being available. Overriding is not an option because the ability is also used by assassins, so one must discover first why exactly is the ability being added. Most likely it is because the cre files still reference the old ability so one has to patch them to point to the new version; the most straightforward way is to patch cre's with kit.ids "blackguard" to use the new one; may also have to patch the script. Sigh. 
