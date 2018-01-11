# ThermosX

![Thermos](thermos_icon.png)

[![Build Status](https://api.travis-ci.org/DireClanMC/ThermosX.svg?branch=master)](https://travis-ci.org/DireClanMC/ThermosX)
![Minecraft Forge v10.13.4.1614][forge]
![Minecraft v1.7.10][mc]
![Java JDK v1.8][java]
![Spigot 1.7.10 Snapshot][spigot]

### What's ThermosX?
ThermosX is a fork of KCauldron and Thermos, a CraftBukkit-Forge server for Minecraft 1.7.10. After periods of inactivity on KCauldron's (and Thermos) GitLab concerning major issues, ThermosX was created to allow active members of the Minecraft coding community to optimize it and provide fixes in a timely manner.

We hope to eliminate all issues with CraftBukkit-Forge servers. In the end, we envision a seamless, low lag ThermosX experience.

Advantages over KCauldron:
+ Lag-lowering optimizations
+ Better world protection (Forge stuff doesn't bypass Bukkit plugins!)
+ Many patches that KCauldron didn't get from Spigot
+ Dupe glitch fixes
+ Includes Spigot API to load plugins made for Spigot


## Installation
Click [here](http://direclanmc.github.io/ThermosX/install)

## Downloads
~~You can download the pre-built packages from [here](https://github.com/DireClanMC/ThermosX/releases).

**ThermosX is still in beta and you may encounter issues in using it with your server. You have been warned!**

P.S. **PLEASE** look at the release notes before downloading! :smile:

##Installing WarmRoast
[Tutorial Video](https://youtu.be/c0ffjooX7Jw)

## Contributing

Please read the [guide](https://github.com/DireClanMC/ThermosX/blob/master/CONTRIBUTING.md) on how to contribute - Thermos always needs improvements :smile: 


## Build Requirements
* Java 8u101 JDK or higher
* `JAVA_HOME` defined on your OS

## Building DireClanMC/ThermosX
* Checkout project
  * You can use IDE or clone from console:
  `git clone https://github.com/CyberdyneCC/Thermos.git`
* Setup
  * Auto: `setup.sh`
  * Manual:
  `git submodule update --init --recursive`
* Build
  * This process downloads minecraft and apply patches
  * If you have gradle integration in IDE - you can still use gui
  * Auto: `build.sh`
  * Manual:
  `./gradlew setupCauldron jar`

All builds will be in `build/distributions`
  
## Updating sources
* Update sources
  * `git pull origin master`
* Re apply patches & build binaries
  * `./gradlew clean setupCauldron jar`

## Known Caveats, use provided fixes at your own risk.

✔ Aether II: isDonor function can lock up servers. [Fixed]

✔ BungeeCord: It's been known for years that BungeeCord barely works with Forge & seems that it'll never be supported officially. [Fixed]

✔ BuyCraftX: Doesn't seem to work with Thermos, info on why it doesn't is unknown currently. [Fixed]

✔ Citizens: Not compatible with forge [Fixed]

✖ Lilypad: 100% not compatible with Forge, lead developer has declined to add support when asked.

✔ DraconicEvolution: P keybind will bypass protection. [Fixed]

✔ Factions + MassiveCore: No protection from Forge items. [Fixed]

✔ TuxTwoLib: Didn't work with ThermosX at all [Fixed]

✔ Mobius / Opis: You can download fixed version [HERE](https://cdn.discordapp.com/attachments/172072987154055168/186577486593785857/MobiusCore-1.2.5-Thermos.jar)

✔ SkinsRestorer (for those using offline ThermosX server): Latest working version is 10.4.4 [HERE](https://www.spigotmc.org/resources/skinsrestorer.2124/download?version=58535)

[Fixed]: http://gogs.tcpr.ca/TCPR/Fixes "Fixed"
[forge]: https://img.shields.io/badge/Minecraft%20Forge-v10.13.4.1614-green.svg "Minecraft Forge v10.13.4.1614"
[mc]: https://img.shields.io/badge/Minecraft-v1.7.10-green.svg "Minecraft 1.7.10"
[java]: https://img.shields.io/badge/Java%20JDK-v1.8-blue.svg "Java JDK 8"
[spigot]: https://img.shields.io/badge/Spigot-v1.7.10--R0.1--SNAPSHOT-lightgrey.svg "Spigot R0.1 Snapshot"
