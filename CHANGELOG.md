# 2.7.0 Release

## What's changed?
**Added**
- Target pistol
   └ Weapon steel tier pistol that holds 15 rounds and shoots .22 LR
   └ Accepts silencers
- NCR Ranger Power Armor
   └ Legendary set, like the remnants power armor
   └ Stats are largely similar, but has a speed boost when sprinting
   └ Red room exclusive
   └ Comes with the power armor - melee controller item 
      └ If the full set is equipped, the melee controller allows for powerful melee attacks
      └ Left click does two rapid swings, right click causes both arms to swing at once
      └ The NCRPA's blades are armor-piercing and gib enemies on death
      └ The blades do 250% damage on large enemies, i.e. ones with 100 or more max health
   └ And also the power armor - ranged controller
      └ Allows the NCRPA to fire rockets straight from the inventory
      └ Left click fires guided rockets and right click unguided ones
      └ Only does 25 damage max, but has no reload and a fire rate of 120 per minute
- Heavy duty electricity connector
   └ Upgraded version of the standard model
   └ Two times as chunky, ten times as powerful
   └ Ideal for custom pylon designs
- Two new expensive mode items
   └ Ultra fine gold dust, which can be combined with ferric schrabidate in the particle accelerator to create degenerate matter
   └ Degenerate matter, which is used instead of regular ferric schrabidate in the exposure chamber to create DNT



**Fixed**
- Fixed #49
- Fixed proxy tiles that do not use electricity at all visually connecting to cables
- Fixed missing texture for canned horse slime
- Fixed incorrect ore dictionary key used by enriched naquadah watz pellet recipe
- Fixed out of bounds light level for the RTG blast furnace
- Fixed the recipe configs now allowing NBT data for output items, rendering the precision assembler and annihilator configs useless
- Fixed the PWR waiting a whole second for the fluid reconnect after the game is paused or loaded
- Fixed chemical factory internal tank sharing ignoring tank pressure
- Fixed the NCR ranger power armor missing most protection stats
- Fixed LPS pipes not properly connecting to the new industrial turbines
- Fixed NCRPA missing radiation resistance stats (it's 97% for the full set)
- Fixed NCRPA chestplate giving night vision even without a full set
- Probably fixed the fused meteorite sword recipe being missing (untested)
- Decreased the fusing difficulty of chlorine and calcium in the ICF which should hopefully make ClCa fuel pellets usable (untested)
- Fixed loot piles only having a single block render AABB, causing armor rewards from red rooms to blink out of existence at certain angles
- Fixed filled crate blocks not dropping crate items with a stack lock in place
- Fixed stack lock not being applied when an item crate is opened, allowing them to be stacked while the item is open
- Fixed clientonly melee component call on the power armor melee controller
- Fixed SEDNA melee (bayonets, power armor melee) being able to punch dead or dying entities, which would swallow hits intended for entities behind them
- Poor render performance with Nuclear Blast Furnaces
- Gas centrifuge recipe for mineral slurry doesn't show all outputs
- Fixed Budding Certus Quartz block recipe (thanks to @kotofev for finding this bug)
- Fixed taurun armor not having working gas masks
- Refactored the armor system, stats like radiation and particle protection are no longer scattered over various registries, making future sets less likely to miss them
- Fixed crucible smeling one too many items with no template installed, causing the gauge to exceed the boundaries
- Potentially fixed another issue with artillery rocket targeting



**Changed**
- Reworked the industrial turbine
   └ New model and texture
   └ Removed the GUI, it now uses the same in-world compressor toggle as the leviathan turbine
   └ No longer has a volatile power buffer, power isn't buffered at all anymore, similar to steam engines and MHD turbines
   └ Steam capacity changes based on compression level, the ratio for turbine cascades is now 1:1:1:1
   └ Comes with a flywheel, energy output slowly ramps up as steam is supplied and slowly goes down as steam cuts out
   └ Recipe is similar to the old industrial turbine, but slightly simplified and cheaper
- Leviathan turbines no longer have a power buffer
- Updated russian and chinese localization
- The PWR can now be controlled via RoR
   └ The RoR value reader can read core and hull heat as well as fuel depletion in percent
   └ The RoR controller can set the control rod level in percent as well as jettison all loaded fuel
- Having 528, expensive or rampant mode enabled now displays a badge in the top left corner, showing that it is enabled
   └ Badges can be disabled with the ```BADGES_HUD``` value of ```/ntmclient```
   └ The badge only shows up if the "true" configuration is used, 528 requires default settings, expensive requires the precision assembler config to not be modified and rampant needs most of the default settings enabled
   └ If all three modes are enabled, the "328 mode" badge also appears
- Removed toothpicks, as they haven't been used in recipes for well over a year
- Cleaned up a ton of unused assets
- The old crucible smelting rules when not using a template can be restores with the ```/ntmserver``` value ```LEGACY_CRUCIBLE_RULES```
- Due to repeated complaints, power armor sounds are now generally more quiet, with 25% volume for steps and 50% volume for jumping and landing
- Reduced mask man's projectile resistance from 75% to 50%
- Reduced maskman's resistance to damage above 50 from 75% to 50%
- Remnants power armor can now use the melee controller, allowing Sergeant Arch Dornan to beat the snot out of people
- Improved gibbing
   └ All cybercrab variants can now be gibbed, turning into metal fragments
   └ Iron golems now also turn into metal instead of fleshy chunks
   └ Slimes can now be gibbed, turning into slime globs
   └ Creepers now also gib into slime instead of blood
- The ZIRNOX can now be toggled by supplying redstone to one of its ports
- Snow golems now use the grey metallic gib particles instead of blood
- The heavy magnetic storage tank now uses BSCCO instead of AA
- Increased the industrial steam turbine's throughput to 150mB/t of UDS exactly 
   └ In addition to being an almost 50% buff, this also fixes the slight issue where turbine chains couldn't reach 100% throughput
- The remants power armor melee ability now has a refire check, meaning the attack will be repeated automatically if the attack button is held down 
   └ ATATATATATATATATATATATATATATA
- Power armor melee attacks now detect entities with a hitbox that's 0.5 blocks larger in all directions, making it substantially easier to hit small targets
- As a side effect, this also increases the maximum range by 0.5 blocks
- Fluid identifiers can now be used to change atmospheric compressor extraction type (screwdrivers still work too)
- Fissile Materials quest now can be completed via Chicago Pile quest
- Reworked Orbital Station quest
- Desh quests now mentions mercury
- Reworked Batteries quest
- Added ME Subnetting quest
- Removed Schrabidate Capacitor quest
- Added Pipe Anchors quest
- Updated russian localization
- Removed T45 protections entirely
- The ICF laser controller max output can now be adjusted in the config, both stats for the capacitors and turbochargers can be changed separately
- Updated Industrial Steam Turbine quest
- Added Ferrouranium Anvil skip in the Desh Anvil quest
- Added Deuterium Extraction Tower quest
- Added PWR powered Steel Furnace quest



[Full Changelog](https://github.com/Nuclear-Tech-New-Horizons/NTNH/compare/2.6.0...2.7.0)

## Download
[GitGub](https://github.com/Nuclear-Tech-New-Horizons/NTNH/releases/tag/2.7.0)
