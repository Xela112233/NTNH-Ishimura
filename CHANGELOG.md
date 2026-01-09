# 2.5.0 Release

## What's changed?
**Added**
- Added new HUD features (everything is customizable)
- Added blur when entering GUIs
- Added various optimizations and tweaks
- Added item physic
- Added Keyboard Wizard (check controls settings)
- Added opticubes
- Added Resource Pack Organizer
- Added satchels and pouches
- New models for:
   └ Stardar
   └ Orbital Station Computer
   └ Solar Panel
- New GUIs for:
   └ Cryogenic Distillation Machine
   └ Vacuum Solderer
- New battery system
   └ Energy storage blocks, capacitors and battery items are now deprecated, but can still be used
   └ There is now new types of battery items, as well as capacitor items
   └ Instead of energy storage blocks, there is now a battery socket, which allows those new items to be connected to the power grid
   └ Battery sockets act like cables, they will connect power grids when two cables are plugged into them in different directions
   └ Self-chargers and creative batteries are still around, as well as spark batteries which are needed for the balefire bomb
   └ The FEnSU has been replaced by a much larger version with unlimited energy storage
- Fluid valve with counter
   └ Reads total fluid movement within a network
   └ Value can be read or reset with OC or RoR
   └ Allows for very precise portioning and fluid control



**Fixed**
- Fixed broken skins
- Fixed various bugs
- Fixed top-left corner in the main menu
- Fixed Xenon thruster uncraftable in new assembly machine
- Ore clusters rendering partially transparent
- Custom rockets churning chunks with unused vanilla lava/water checks
- Fixed meteors using a nonexistant keepalive timer, causing potential audio flickering in certain cases
- Potentially fixed a performance issue caused by transmission networks not being deleted when they have no active links
- Fixed power not saving for mining lasers
- Fixed the annihilator producing blank 528 mode blueprints when 528 mode isn't even enabled
- Fixed black fire not using the skeletonizer on death
- Fixed arc furnace electrodes not being able to be plugged into the arc furnace unless the lid is fully open
- Fixed broken keybind localization



**Changed**
- Glass now breaks faster with a pickaxe
- Reworked ropes crafting recipe
- Brewing stand now shows what potions are in it
- Reworked Woven Cotton recipe
- Removed unused mods
- MASSIVELY debuffed mobs
- Station hum now uses the ambient sound category
   └ A few other sounds moved into more appropriate sound categories
- Conglomerate processing now requires an initial brine washing step
- DNT suit now functions as a full spacesuit, without the need for a PLSS
- Suffocation damage now scales over time
- Changed icon of the NTNH window
- Updated italian localization
- After not being part of worldgen for a long time, oily coal is finally being removed
- The rare metal blocks that had been unobtainable and unused for the longest time have been removed
- The schrabidium transmutator's grace period is over, it is finally being destroyed
- Most of the legacy fusion reactor components, which were unobtainable and unusable, have been removed
   └ The block ID economy is looking better than ever
- Infinite water barrels can now be crafted with any water container and not just buckets
- OpenComputers integration for the PWR can now also read the heat capacity stats
- Removed the restriction that demands that cluster ores need to be mined by hand
- Laser beams from energy weapons are now a lot more narrow
- All steam turbines now have a passive drain on unused power in their buffers



[Full Changelog](https://github.com/Nuclear-Tech-New-Horizons/NTNH/compare/2.4.1...2.5.0)

## Download
[GitGub](https://github.com/Nuclear-Tech-New-Horizons/NTNH/releases/tag/2.5.0)
