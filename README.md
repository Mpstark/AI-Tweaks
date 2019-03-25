# BetterAI - AI Behavior Variable Tweaks for HBS BATTLETECH
This is a ModTek mod to improve the tactical AI in combat.  The AI is allowed to reserve 'Mechs and execute "Double Turns," AI critical hit chance is on par with the player's, it now considers protecting their weakened side and exploits the damaged sides of the target to a greater degree.  The Pilot selections for AI Lances are constrained to put appropriate pilots in the right units, this has been limited to two 'Mechs or less per Lance to preserve encounter variety, all vehicles have had "useless" pilot abilities excluded.  This should be harder to fight than stock, but some bad choices are not fixable with .json edits.  

Better AI shouldn't cause any errors with save files, even saves in combat, or with version updates.  I've done extensive testing back and forth between stock and modded play without any errors.  It does not add any new items to the VersionManifest.csv.

##### Credits:
    Mpstark: For creating this inital git and ModTek support
    scJazz: The idea for Lance Pilot tuning
    Thanks to all who have provided feedback and bounced ideas around with me. 
    Team Banzai, Goons, discord modders and everyone since beta onward has helped shape this AI to be as robust as I can make it.

### Instructions:

    Copy Better AI folder in to Mods folder created for ModTek.  Remove older Better AI folder if present.

### Full change log can be found here:

https://forum.paradoxplaza.com/forum/index.php?threads/mod-release-better-ai-tweaks-for-deadlier-ai.1075322/

### Googledoc sheets with all stock + modded variables, unit_role and unit_lance tags:

https://docs.google.com/spreadsheets/d/1Q-Z0jSjb1rRd5-r0zYHwH_yES8cgVdmv-kE2WS_7lHE/edit#gid=0&range=A1

### Recommended Companion Mods

https://github.com/BattletechModders/cFixes/releases - Commuinity bug fixes, Better AI greatly benifits from the corrected NPC pilot traits fixes and integrates with that mod's 'Mech tag fixes.  NPC pilots are missing a lot of passive traits without cFixes.

#####  NOTE - Better AI has cFixes set as an Optional Dependency.  It will automatically load after cFixes changes.  Better AI does not need cFixes to work.

### ModTek
This mod needs ModTek to work:

https://github.com/BattletechModders/ModTek/releases

## Stock Files Edited:
#### StreamingAssets\data\behaviorVariables - AI variable edits
    global.json
    global_def.json
    global_sensorlock.json
    role_lastmanstanding.json
    role_meleeonly.json
    role_scout.json
    role_sniper.json
    role_vehicle.json
    role_vehicle_def.json

#### StreamingAssets\data\constants - AI Crit Chance
    CombatGameConstants.json

#### StreamingAssets\data\lance - LanceDef Pilot Optimizations (WIP)
    Planned - Remaining Dynamic Lances difficulty 5 - 10
    lancedef_mech_d1_dynamic_solo.json
    lancedef_mech_d2_dynamic_solo.json
    lancedef_mech_d3_dynamic_lightBattle.json
    lancedef_mech_d3_dynamic_lightCavalry.json
    lancedef_mech_d3_dynamic_lightFire.json
    lancedef_mech_d3_dynamic_lightScout.json
    lancedef_mech_d3_dynamic_lightSupport.json
    lancedef_mech_d3_dynamic_solo.json
    lancedef_mixed_d3_dynamic_lightBattle.json
    lancedef_vehicle_d3_dynamic_lightBattle.json
    lancedef_mech_d4_dynamic_lightMedBattle.json
    lancedef_mech_d4_dynamic_lightMedCavalry.json
    lancedef_mech_d4_dynamic_lightMedFire.json
    lancedef_mech_d4_dynamic_lightMedScout.json
    lancedef_mech_d4_dynamic_lightMedSupport.json
    lancedef_mech_d4_dynamic_smallLightMedBattle.json
    lancedef_mech_d4_dynamic_smallLightMedFire.json
    lancedef_mech_d4_dynamic_smallMedCavalry.json
    lancedef_mech_d4_dynamic_smallMedScout.json
    lancedef_mech_d4_dynamic_smallMedSupport.json
    lancedef_mech_d4_dynamic_solo.json
    lancedef_mixed_d4_dynamic_lightBattle.json
    lancedef_vehicle_d4_dynamic_lightBattle.json

#### StreamingAssets\data\mech - Role Tag Replacement
    mechdef_awesome_AWS-8Q.json
    mechdef_enforcer_ENF-4R.json
    mechdef_locust_LCT-1M.json
    mechdef_quickdraw_QKD-4G.json
    mechdef_quickdraw_QKD-5A.json
    mechdef_shadowhawk_SHD-2D.json
    mechdef_urbanmech_UM-R60.json
    mechdef_zeus_ZEU-6S.json
