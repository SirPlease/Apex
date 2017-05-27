# Apex #

**LINUX SERVERS ONLY**

This config is based upon [ZoneMod](https://github.com/SirPlease/ZoneMod) and will have changes from there.
People may consider this the harder config, with a reflux-ish feel.

- - - -
### Server Admins! ###

**DISCLAIMER: Using the plugins provided with the download in other configs is at your own Risk as they're designed around Apex and are likely to be unstable in other configs or general usage.**

* Requirements:
  * Clean Servers:
	* [Sourcemod](https://www.sourcemod.net/downloads.php?branch=1.7-dev) (1.6 or 1.7), [Metamod](https://www.metamodsource.net/), [Stripper:Source](http://www.bailopan.net/stripper/#install).
	* [Extensions, Gamedata, Main Competitive Plugins, etc](http://sirftp.com/Left4Dead2/ZoneModRequirements.zip)
	* These simple Steps also setup your Server's base for other configs, so you'll only need the optional plugins that other configs require.
  * Competitive Servers:
	* None, modify your matchmodes file to add the config to the Match menu and you're set. :)

* Admin simplicity:
  * To make sure none of your precious plugins get overwritten, all plugins have their seperate folder (optional/apex)
    * If you have a prefered edition of a Plugin, you are able to simply replace the file in optional/apex.
	* Make sure the Plugin you're overwriting doesn't have a feature added that's required for proper Apex play!
  * To make it easy for personal configuration for certain plugins, there's an added "server_preference.cfg" in the cfg/cfgogl/apex folder.
    * This is to prevent Admins from messing with crucial variables.
	* Keep in mind that this is a shared cfg, so it'll only contain shared cvars.
	* These cfgs are very useful for Admins wanting to load 1v1~4v4 supported plugins on top of the Configs.
  * Server_Namer is added to this package, useful for a clean Hostname.
	* Everything is explained in the Server Preferences.
	* It is not loaded by default, needs uncomments.
	* The .txt file will ask permission for an override, this should be fine.

* Admin Tips:
  * bequiet.smx is a very useful plugin to keep chat clean, if you decide to load it in other configs, make sure it's loaded before other plugins.
	* Keep in mind that it comes with a "Spec-Listening Feature", this might collide with other plugins.
	* Simply unload the other plugin, or set bequiet's "bq_show_player_team_chat_spec" cvar to 0.
  * TickRateFixes now also fixes Slow Doors and Pistol Scripts, useful for use with other configs.
	* Make sure you're not loading l4dpistoldelay if you're using this Plugin.
	* Make sure you don't have any adjustments to prop_rotating and prop_rotating_checkpoint speeds in your cfg/stripper folder.
  * Specrates is a useful plugin to reduce server load causes by spectators.
    * This will send less updates to Spectators whilst maintaining a pleasant viewing experience.

- - - -
### Gameplay / Balance Changes ###
* Health Bonus is used instead of Hybrid DB+HB.
  * Holdout Bonus is not used.

* Maximum amount of pills you can find outside the saferoom is 2.
* Common Infected wandering in the background has been set to 30 (**Vanilla:** 20)
* You can only find one more set of pills outside of the saferoom.
* Finite Hordes are disabled, returning the infinite horde events.
  * Infinite Hordes will be paused instantly during Tanks however.

* Special Infected
  * Quad Caps are enabled.
  * Sack Order is now handled by a plugin, rather than the AI Director.
	* This will keep the sack order working functioning properly at all times (Boomer dies 3rd or 4th, Quad Cap guaranteed)
	* This prevents getting the same SI several times while the Tank is up.
	* Do NOT use this plugin outside of Apex, it's in its early stages.
  
  * Tanks
	* Tanks can be slowed down upto a maximum of 25% by Uzis, Pistols, and Deagles.
	* Speed is reset back to its default value (210, was 200)
  * Hunter
	* You can now have a maximum of 2 Hunters at the same time.
  * Jockey
    * The Jockey can no longer be skeeted.
  * Spitter
	* The Spitter has been removed.
  * Boomer
    * The Boomer will now spawn 10 common infected per biled Survivor (was 15)

* Melee Weapons
  * Melees are now all converted to pistols, ensuring you're always stocked on dualies whilst enjoying the sight of some floating/clipped pistol spawns.

* Weapon Adjustments:
  * All Chrome Shotguns have been replaced by Pump Shotguns.
  * All Silenced Uzis have been replaced by Smgs.
  * Reload Speed:
	* Uzi: 1.82 (**Zonemod**: 1.74 - **Vanilla**: 2.23)
  * Damage:
	* Uzi: 20 (**Zonemod**: 21 - **Vanilla**: 20)
	* Shotgun: 250 Total per shot. (**Zonemod**: 280 - **Vanilla**: 250)
  * Tank Damage Multiplier:
    * Uzi: 15% more damage on Tank.
  * Ammo:
	* Shotgun: 8/120 (**Zonemod**: 8/96)
  * Spread:
	* Pumpshotgun has reduced spread and decreased damage drop-off, making it a powerhouse again.
	
- - - -
### Miscellaneous ###
* The Starting Saferoom Door has been removed to prevent Survivors from using it as a shield, leaving them vulnerable.
* Alarm cars will have their alarm turned off after a Tank punches another hittable against it.
* Common Infected no longer lay down, sit, or fight eachother.
* Lowered the SI Bot kick Delay to 3 (from 10)