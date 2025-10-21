# A. Technical side.

* Lots of updates needed to latest weidu_library.

# B. Bugs.

* Should Cleric + Ranger access to Fire Trap? Yes, but the levels at which they access is screwy, meaning they access it earlier than they should. We can simply let this slide for the simplified implementation.

* Blackguard's Poison Weapon ability does not override the existing one and this leads to the old ability still being available. Overriding is not an option because the ability is also used by assassins. The ability is being added because the cre files still reference the old ability so one has to patch them to point to the new version; the most straightforward way is to patch cre's with kit.ids "blackguard" to use the new one; may also have to patch the script. Also have to change cre's spellbooks. Sigh.
