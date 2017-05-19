# Changelog: #

* **v1.0.1**
  * A full shotgun blast now does 260 Damage instead of 280 (**ZoneMod:** 280 - **Vanilla:** 250)
  * Slight nerf to the Shotgun spread and range.
  * Damage for Uzi's set to 22. (**ZoneMod:** 21 - **Vanilla:** 20)

* **v1.0.2**
  * A damage nerf to the Shotgun (240 per Full Hit)
  * Jockeys can no longer be skeeted.
  * Added specrates.smx to reduce server load from within the config.
  
* **v1.0.3**
  * A slight increase of maximum Tank Slowdown (25% to 28%)
  * Pistols cause slightly more slowdown now.
  * Damage for Uzi's reverted to 20.
  * Uzi has received a damage buff against Tanks, doing a total of 15% more damage to Tanks per shot.
  * A final damage nerf to the Shotgun (220 per Full Hit)
  * Increased Shotgun Bonus Damage Range on Common back to 100 (was 60)
  * Infinite Hordes will be paused instantly during Tanks.
  * The Starting Saferoom Door has been removed to prevent Survivors from using it as a shield, leaving them vulnerable.

* **v1.0.4**
  * Decreased Maximum amount of Common Infected from 30 to 25.
  * Increased Maximum amount of Common Infected alive (no Boomer/horde) from 20 to 25.
  * Removed the chance of Common Infected sitting or lying down.
  * Removed the chance of Common Infected attacking eachother.
  * Removed Female Boomer Spawns.
  * Fixed the removed Saferoom Door blocking you from leaving on Dark Carnival Map 2+3 and The Passing 3.
  
* **v.1.0.5**
  * Fixed a Tank Spawn issue on No Mercy Map 3.
  * Removed the Death Toll Map 4 Event Tank
  * Shotguns have been set to 250 Damage per full shot, this will likely be the last change (Damage to Tank might be changed)
  * Increased the Maximum amount of pills found outside the Saferoom to 2 (was 1)
  * Increased the Maximum amount of Hunters to 3 (was 2)
  
* **v1.0.6**
  * Replaced the Director's method on deciding what SI the next spawn gets, with a Plugin.
	* The plugin will properly give you spawns based on what died first.
	* For example: if a Hunter dies first, he will be queued to spawn after the current queue has been spawned.
	* The reason for this plugin is simply because the Director seemed to act a bit strange, granting several quads after eachother or boomer setups when you killed him last.
	* **DO NOT** use the plugin in other configs, as it's not fully functional in every config as of yet.
	
* **v1.0.6a**
  * Fixed issues with the Sack Order Plugin.
    * Fixed Spectators affecting the Sack Order.
	* Fixed Despawning affecting the Sack Order.
	* Fixed the 2nd Team not having the same SI line-up for the first hit.
	
* **v1.0.7**
  * Added a final Safecheck for the Sack Order plugin.
  * Hunter Limit set back to a limit to 2.
  * Uzi Slowdown decreased slightly.
  * Maximum Tank slowdown decreased from 28% to 25%
  * Lowered the SI Bot kick Delay to 3 (from 10)
  * Due to popular demand, female boomers are back and now have a 50% chance of spawning instead of 25% (Vanilla)
	* **EQUALITY**	