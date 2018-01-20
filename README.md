# VortiK's Deep Core Mining

Sad to see your outposts depleted and empty ore trains on your rails ? No more with Deep Core Mining ! Refactor your mining outpost to give them a new longterm breath !

This mod is designed to aleviate the "depleted ore outpost" and "need to keep building new outpost forever" problems without a too cheaty ore generator solution. Adds a new type of equivalent ore resources that only spawn in place of depleted field to be mined with specific expensive drill.
- New ore resource "patches" have a 10% chance to spawn under depleted normal ore for Iron, Copper, Uranium, Coal and Stone.
- Ore patches are like oil and provide an infinite yield that diminish with usage but with a small infinite minimum.
- Ore patches can be manually mined to free land and get a burst of resources as the cost of refining and losing the infinite minable patch.
- New advanced and animated mining drill, the Deep Core Mining Drill (DCMD) is used to mine ore patches with associated technology and its own intermediate component ; ~16x more expensive to build but ~13x more powerful than a normal electric mining drill !

The idea is to repurpose old mining outpost when ore is depleted. So the infrastructure is still usefull for the investment of resources and time to replace old drills and building new machines while also providing a small but steady infinite source of ore.

Other new features
- Advanced deep core mining drill to mine rare cracks in the world. Provide infinite ore, but require heavy refining.
- Manual planner tool to remove ore patches and cracks from the world to free land or get a boost of refinable resources.
- Drills require sulfuric acid (for uranium and cracks) that *must* be injected directly with a pump (pipes will not be enough).

Graphics for the mining drills are not mine, source : https://www.spriters-resource.com/

---------------------------------------------------------------------------------------------------
Version: 1.7.0
Date: 20. 01. 2018
 Features:
    - New Advanced Deep Core Mining drill, bigger, expensiver and it has its own working sound. Dedicated to mine the ...
    - New Deep Core Mining Cack resources that are a rare spawn in the world (~1/500 chance per chunk). Enable to mine the ...
    - New Resource Deep Core Ore Chunk from DCM Cracks that must be refined in a centrifuge and will yield ore chunks that themselves require refining to get ore.
    - DCM Crack can be planner removed and require sulfuric acid to mine (like uranium).
    - Made both DCMD and ADCMD not rotatable and fixed in south orientation to match their sprite (thanks discord @Bilka#2444)
  Changes:
    - Review descriptions & locales.
    - Review Technologies, now in 3 tiers with appropriate cost and requirements. Migration is done for existing saves.
    - Resorted all DCM items in inventory (should be better if not perfect).
    - Changed spawn range setting and new default is 1 (from 250) as all deep core ore resource entities can be manually harvested and removed if needed with 1.6.0 planner tool.
    - Review DCMD graphics, adds ore exit and proper pipe input.
  Fixes:
    - Sounds tuning, graphics enhancements and code improvement accross the board.
---------------------------------------------------------------------------------------------------
Version: 1.6.1
Date: 14. 01. 2018
  Fixes:
    - Removed crash inducing migration file that shouldn't be there.
---------------------------------------------------------------------------------------------------
Version: 1.6.0
Date: 14. 01. 2018
  Features:
    - New Manual Mining feature using a selection tool to select ore patches to remove.
    - Removing ore patches requires deep core mining drones and sulfuric acid barrel for uranium ore patches.
    - Removing ore patches generates ore chunks of 10% of the remaining ore patch up to a max of 1 000 (maxes out at ~300% of ore patches amount).
    - Deep Core Ore chunks require refining with sulfuric acid to get normal ore at 100 per unit.
    - Some graphics of manual mining and refining process are placeholder and may be improved later.
    - Added changelog.txt :)
  Changes:
    - Split Deep Core Mining technology to unlock manual patch removing tools earlier and kept DCMD high tech.
    - Reduced default range from start from which ore patches can spawn from 250 to 1 as there is now a tool to remove them if needed.
---------------------------------------------------------------------------------------------------
Version: 1.5.0
Date: 09. 01. 2018
  Features:
    - Nuclear Age
    - Added uranium ore patches and made them glow (inspiration from https://mods.factorio.com/mods/wormmus/wormmus-glowing-ores)
    - DCMD can mine uranium ore patches and require sulfuric acid (100 from 10 for normal mining drill)
    - DCMD will need a dedicated pump to inject fluid in it
    - DCMD now has circuit interface. Like mining drill or pumpjack can be toggled on/off and read remaining resources (like pumpjacks it will output the mining rate)
    - Added min and max for random ore patches values on spawn as a mod setting you can change (defaults from 60 000 to 300 000, same as before)
  Changes:
    - Changed DCMD ore output to better fit the sprite (you'll need to fix your existing mines)
  Fixes:
    - Fixed some translations typo & grammar
---------------------------------------------------------------------------------------------------
Version: 1.4.2
Date: 26. 12. 2017
  Fixes:
    - Mining speed fix
    - DCMD mining speed was bugged because of a leftover test (probably since 1.0 of the mod). Tested with the originally intended 27x more power of a normal mining drill, felt overwhelming (too much ore). It is now ~13x times faster at mining as the normal mining drill (cost unchanged, still ~16x).
    - Thanks for the report in https://mods.factorio.com/mods/VortiK/vtk-deep-core-mining/discussion/22655
---------------------------------------------------------------------------------------------------
Version: 1.4.1
Date: 13. 12. 2017
  Fixes:
    - Fixed crash because of missing icon_size on some entity that is now required.
---------------------------------------------------------------------------------------------------
Version: 1.4.0
Date: 13. 12. 2017
  Changes:
    - Updated for Factorio 0.16
---------------------------------------------------------------------------------------------------
Version: 1.3.1
Date: 29. 11. 2017
  Changes:
    - Balanced DCMD pollution as it was indeed way to high, from 1000 to 150 without module which is closer to the intended ~10-15x a normal mining drill (9 pollution). It can of course still be reduced by 80% with 3 efficiency modules 1 for ~3x pollution of a normal mining drill (30 vs 9) and ~15x an efficiency moduled mining drill (30 vs 1.8).
    - Thanks a lot for the detailed feedback in this discussion https://mods.factorio.com/mods/VortiK/vtk-deep-core-mining/discussion/19928
---------------------------------------------------------------------------------------------------
Version: 1.3.0
Date: 10. 11. 2017
  Features:
    - Stone age
    - Added support for deep core mining of depleted stone with stone patches
    - Added map-level mod runtime configurations for enabling each ore patches (iron, copper, coal, stone). All enabled by default, if disabled will prevent spawning of new ore patches when normal ore is depleted.
---------------------------------------------------------------------------------------------------
Version: 1.2.0
Date: 13. 08. 2017
  Changes:
    - Changed default minimum range from the start where ore patch spawn on depleted ore from 500 to 250.
    - Made the minimum spawn range a setting that can be changed in the mod options game menu.
---------------------------------------------------------------------------------------------------
Version: 1.1.1
Date: 12. 08. 2017
  Fixes:
    - Minor fix to Deep core mining drill selection box
---------------------------------------------------------------------------------------------------
Version: 1.1.0
Date: 12. 08. 2017
  Features:
    - Ore patches won't spawn on depleted ore in the starting zone < 500 blocs (~1-2 starting area radar size) ; it's a high tech mining solution not available until mid-endgame anyway.
    - Added shadow to the Deep core mining drill !
    - (internal) Added Factorio community Stdlib : https://github.com/Afforess/Factorio-Stdlib (it's awesome for modding, try it !)
---------------------------------------------------------------------------------------------------
Version: 1.0.0
Date: 11. 08. 2017
  Features:
    - initial release