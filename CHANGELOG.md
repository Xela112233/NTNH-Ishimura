# 2.6.0 Release

## What's changed?
**Added**
- HTR-F4 NEO Station Thruster added
   └ Connect to the new fusion reactor to provide thrust for your space stations!
- Lithium hydroxide terraforming 
   └ Can convert CO2 in an atmosphere into breathable oxygen, great for terraforming Duna well before Dyson anatmogenesis becomes available
   └ A new machine - the Atmospheric Emitter - has been added to emit huge amounts of gases quickly
- QMAW for the Rocket Launch Pad and the Vehicle Assembly Base
- Dusty + airless celestial bodies now exhibit a faint particulate glow at sunset/sunrise due to charged particles
- Added Transparency Border to recipe-background and catalyst- (NEI)
- Added tooltip for "Required Crafts" with shift in NEI
- Revamped shader support (Shader Fixer was reworked)
- Better OSX J8 Support
- Better video settings search
- Dynamic light improvements



**Fixed**
- Fixed an issue when exiting a GUI after fast-moving items with shift causes the player to stuck in shift position
- Fixed crash of the game caused by Assembly Machine GUI
- Potentially fixed a crash caused by MobsInfo (#43)
- Fix Exception on Server start (#44)
- Fix WorldServer leak in NEIServerConfig
- Fix NEI transparency border
- Correctly crop colored text (NEI)
- Fix Autocrafting for recipe without ingredients in bookmarks
- Potentially fixed yet another issue regarding crates
- Fixed battery socket fillpercent RoR function always assuming a max power of 1
- Fixed issue where multiblock ports would generate many OpenComputers component entries
- Fixed RBMK automatic control rods having incorrect settings when using the copy tool
- Fixed battery sockets producing junk debug data in the logs
- Fixed an issue where the charging station would crash when trying to charge certain items
- Fixed the DFC's core component not dropping its contents when mined
- Fixed audio problems with guns
- Fixed third person muzzleflash on the miniguns clipping the barrel
- Fixed arc furnace IO slots stacking items with incompatible NBT
- Fixed a bounding box issue with casing particles, causing them to slide sideways on the first tick, making trajectories weird
- Fixed some turrets not using the more modern casing spawner system which allows casings to have a smoke trail
- Fixed incorrect tooltip on the upgrade stat screen for assembly factories
- Fixed crash caused by RBMK overpressure meltdown mechanic
- Fixed a crash causing by the charging station in combination with the new battery packs
- Fixed a broken and originally unintended feature where the flamethrower turret would be loadable using regular item tanks
   └ Most ammo slots now work for loading, the empty canisters are returned via the fluid ID slot
- Fixed a dupe regarding conveyors
- Crash on mob spawning due to forge enum extensions
- Orbital rocket assembly allows stacks larger than 8
- Fix GLSL 120 support
- Fix OSX F3 crash
- Lighting fixes
- Buffer fixes
- Fix NTM:Space sunset not rendering
- Various Shader Fixes
- Dynamic Lights Improvements
- Fix end portal w/ Shaders
- Misc Shaderpack loading fixes




**Changed**
- Fixed "definitely a pig" - Ezzocorbi
- Optimize TileEntities
- Misc small changes, and a few small fixes
- Add texture for toggled state of magnet button
- Updated russian localization
- Updated ukrainian localization
- Updated italian localization
- Rad absorbers now use metadata, existing blocks will be converted automatically
- Fissure bombs that go off in crater biomes now create fissures with metadata 1 which creates radioactive volcanic lava
   └ If a crater biome is created on top of an existing fissure, it will keep producing normal volcanic lava
- Simplified the battery socket's client packets, reducing CPU load
- Muzzle flashes on guns now work in third person mode, including on other players and on NPCs, making it more apparent when you're being fired at
   └ This includes non-standard special effects like the .44 gap flash and the .35-800 ejector plume
- Removed the old unused satellite deco blocks, freeing up 6 block IDs
- Crucibles that smelt metal with no template set will no place the metal in the recipe stack instead of the waste stack, this should make it easier to get a recipe to work in the many, many cases where people add the template after smelting the material
- Battery sockets and the FENSU now support the copy tool
- Removed unused displaylist support from the model loader
   └ DLs have been long phased out in favor of VBOs anyway
- Rebranded canned horse slime
   └ Now with extra bone marrow
- Updated the deuterium tower's model
- Updated most blast door visuals
- RBMKs now have QMAW pages
- Updated the model on the heavy magnetic storage container
- Increased the power draw on the osmiridium welding recipe
- Bullet casings now make sounds when falling to the ground
- Most ammo types now have QMAW pages, including information on whether or not they are a war crime
- Both assembly and chemical factories now have four special ports that only allow items inserted to go into one recipe group
- All models using the HFR wavefront loader can now be hot-swapped via resource reload (F3 + T)
- Updated most door models
   └ Door skins are no longer a dedicated item, the skin can be changed using a screwdriver
   └ Available skins are cycled through in the item preview
   └ Fire doors and secure access doors no longer use clipping planes (i.e. making the doors not render outside of their frames)
   └ Vault doors have been ported to the current door system, the blocks should convert automatically
- LPW-3N now shows a hint on how to operate it
- Acidizer partitioner can now accept up to 96 different input items, greatly enhancing its ability to process all the bedrock ores available in space
- Tektite is now deleted by the mining laser nullifier upgrade
- Lesser/Greater Australium can now be cast into ingots



[Full Changelog](https://github.com/Nuclear-Tech-New-Horizons/NTNH/compare/2.5.0...2.6.0)

## Download
[GitGub](https://github.com/Nuclear-Tech-New-Horizons/NTNH/releases/tag/2.6.0)
