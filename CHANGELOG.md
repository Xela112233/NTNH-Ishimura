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
- Added ArmoredArms mod
- Added "Burn Time" description to burn-able items
- Creative klystron
   └ Always outputs as much KyU as the most demanding existing recipe needs
- Added a bunch of optimization mods that should improve overall performance



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
- Potentially fixed an issue in regards to some hidden structures spawning
- Fixed fluid counter valve not having a recipe
- Fixed issue where /ntmreload would break registered fluids from addons
- Fixed yet another issue regarding crates
- Fixed RBMK fluid heaters losing their tank types when unable to boil anything
- Fixed the FEnSU, cyclotron and reliant robin missile being uncraftable due to stacksize limitations
   └ The system for detecting impossible recipe has been improved, instead of a fixed 64 item limit, it now uses the actual limit of the item (or 64 for ore dictionary inputs)
- Fixed yet another issue regarding addon fluids breaking on recipe reload
- Fixed YET ANOTHER issue regarding crates, AGAIN
- Fixed a rare issue where the fusion reactor could have negative fuel
- Fixed battery socket priority tooltip offset
- Fixed enchantability on many armor sets being incorrect
   └ Most power armors are intended to not be enchantable at all
- Fixed crash caused by the balefire bomb
- Fixed heat transfer rate labels on the boilers and coker unit being off by a magnitude of 10
- Fixed crucible not having a heat transfer rate tooltip
- Fixed certain heliostat mirror rotations not showing the mirror
- Fixed chopper recipe creating eight choppers instead of one
- Being able to put non-drive items into planner drive slots
- Log spam when suffocating
- Air bubbles appear when using DNT, even though it works as a spacesuit without PLSS



**Changed**
- NTNH is slowly being localized! Check out current progress and contribute - https://crowdin.com/project/ntnh
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
- NBT-tags are no longer shown in the description of items
- Updated chinese and russian localization
- Increased density of osmiridium ores in tom craters considerably (from 1:500 to 1:200)
- Added a new server setting called ENABLE_MKU to toggle contageon effects, spread and save (part of /ntmserver)
- Extended logging now logs uses of MKU
- Mass storage units now display their held item on a display
- Improved HUD gauges, electric chestplates with jetpacks installed now two gauges side by side
- Material autogen now creates redstone in ingot form, allowing smaller than block quantities to be cast
- Removed the ancient ZPE blocks
- Drone hitboxes are now way smaller, which should cause them to get stuck when flying less
- Sef-charging batteries have been reworked
   └ They are now a new item with metadata (legacy ones still work)
   └ The base form is an empty selfcharger which is filled with two billets of material, i.e. no more upgrade recipes
   └ There are a few new variants like cobalt-60 and gold-198
   └ New selfchargers have a model when plugged into a battery socket
   └ Selfchargers are a fair bit weaker than their old counterparts, but substantially cheaper too
- Old batteries now have the "LEGACY" tag
- Pneumatic pipe networks with multiple outputs, especially filtered ones, should now have much better throughput due to not constantly failing to send items in round robin mode
- The [N] calculator window now shows a history of previous operations
- Simplified the cyclotron recipe
- Station drives can now be used to recall docked & fueled drop pods to your current location
- Stations now show up in the sky of the orbited planet
- Food stacksize have been MASSIVELY increased
- Recolored the main menu



[Full Changelog](https://github.com/Nuclear-Tech-New-Horizons/NTNH/compare/2.4.1...2.5.0)

## Download
[GitGub](https://github.com/Nuclear-Tech-New-Horizons/NTNH/releases/tag/2.5.0)
