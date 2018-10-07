Slugfest

A mod written to satisfy my own desire for a "rail arena" game using hypothermia's UIE 
enhanced interface
written with generous help from http://www.planetquake.com/code3arena/tutorials/

Added Commands
 * reload		(reloads the clip of the current weapon)
 * +button5		(offhand grappling hook)


Features
 * No weapons or powerups are spawned or dropped.
 * Railgun is always spawned with player.
 * All Ammo is spawned as Slugs.
 * Variables for spawning other weapons (including Grapple), starting ammo, clip ammo
 * Armor/Health/Mega-Health/Flags spawn as normal.
 * Weapon clips, increased firing rate, longer clip reload
 * CVARS for weapon firing/loading rate, damage, etc. (just need a map_restart to take effect)
 * Bot support
 * Damage is increased by weights (CVARS) depending on the location hit
  - Foot/Leg damage reduces speed (until health pickup)
  - Arm damage increases reloading time (until health pickup)
  - head,face,shoulder,chest,groin,belly,
 * Falling damage incurs Leg damage
 * Excellent is awarded on 3 railshots in a row, Impressive on 5


CVARS
sf_mgun_ammoSize			Amount of bullets to start out with in pack
sf_mgun_clipSize			Amount of bullets that fit in one clip
sf_mgun_refireTime			MS delay between bullet fire
sf_mgun_reloadTime			MS delay while reloading clip
sf_mgun_enable				1: automatically acquire machine gun 0: dont
sf_mgun_dmg					Bullet damage amount

sf_rail_ammoSize			Amount of slugs to start out with in pack
sf_rail_clipSize			Amount of slugs that fit in one clip
sf_rail_refireTime			MS delay for slug reload
sf_rail_reloadTime			MS delay for clip reload
sf_rail_dmg					Slug damage amount

sf_grapple_enable			0 or 1
sf_grapple_offhand			0 or 1
sf_grapple_fireSpeed		Speed grapple moves at
sf_grapple_pullSpeed		Speed you move at while grappling

sf_gauntlet_enable			0 or 1
sf_gauntlet_dmg				default: 

sf_shotgun_enable			default: 0
sf_shotgun_dmg				default: "10"

sf_grenade_enable
sf_grenade_dmg				default: "100"
sf_grenade_splash_dmg		default: "100"
sf_grenade_splash_radius	default: "150"

sf_rocket_enable
sf_rocket_dmg				default: "100"
sf_rocket_splash_dmg		default: "100"
sf_rocket_splash_radius		default: "120"

sf_plasma_enable			default: "0"
sf_plasma_dmg				default: "20"
sf_plasma_splash_dmg		default: "15"
sf_plasma_splash_radius		default: "20"

sf_bfg_enable				default: "0"
sf_bfg_dmg					default: "100"
sf_bfg_splash_dmg			default: "100"
sf_bfg_splash_radius 		default: "120"

sf_fall_far_dmg				default: "10"
sf_fall_med_dmg				default: "5"

sf_dmg_face					All of these variables have a weight that is applied to the damage (1.0 = no change)
sf_dmg_head
sf_dmg_throat
sf_dmg_shoulder
sf_dmg_belly
sf_dmg_arms
sf_dmg_stomach
sf_dmg_groin
sf_dmg_leg
sf_dmg_foot
