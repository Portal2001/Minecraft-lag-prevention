# Minecraft-lag-prevention
## Mob/entity lag
First most common lag is from mobs either from mob farms or not optimized well
- How to find out?
  - [spark](https://www.spigotmc.org/resources/spark.57242/)
  - timings(this method is not recommended due to performance hit)
- Prevention
  - optimize your server with [Guide1 by papermc](https://eternity.community/index.php/paper-optimization/) and [Guide2 by purpurmc](https://github.com/YouHaveTrouble/minecraft-optimization)
  - use [FarmControl](https://www.spigotmc.org/resources/farmcontrol-1-15-1-18.86923/)
    - helps to optimize large mob farms
  - use [EntityDetection](https://www.spigotmc.org/resources/entitydetection-tile-entity-support.20588/)
    - helps to find the most populated chunks in whole world.
  - use [AntiRaidFarm](https://www.spigotmc.org/resources/antiraidfarm-block-cheaty-infinite-raid-farms.83283/)
    - helps to stop nonstop raids farms
## Redstone lag
Its commonly used by players to make 0 tick farm (without observer or continuous)
- How to find out?
  - [spark](https://www.spigotmc.org/resources/spark.57242/)
  - timings(this method is not recommended due to performance hit)
- Prevention
  - use-faster-eigencraft-redstone= true in paper.yml
    - helps to optimize redstone by papermc
  - use [Insights](https://www.spigotmc.org/resources/insights-super-configurable-region-limits-asynchronous-scans-1-18.56489/)
    - helps to limit redstone and other items per chunk to limit the use of it
  - use [AntiRedstoneClock](https://www.spigotmc.org/resources/antiredstoneclock-worldguard-plotsquard-support-1-8-1-17.18557/) 
    - helps to cut down redstone clocks according to TPS
    - for teleport to the clock can use [Redstone Clock Detector](https://dev.bukkit.org/projects/redstone-clock-detector)
## Other common lag machines
  - Armor stands 
    - armor-stands-tick: false in paper.yml
      - stop the tick on Armor stands
    - armor-stands-do-collision-entity-lookups: false in paper.yml
  - Minecarts
    - use [CAProtect-Lite](https://github.com/castaway-gg/CAProtect-Lite)
      -  prevents players from stacking thousands of minecarts together
    - /gamerule maxEntityCramming 8
  - llama spit
    - rare event but can be solved
    - entity-per-chunk-save-limit
      - llama_spit: 3
  
