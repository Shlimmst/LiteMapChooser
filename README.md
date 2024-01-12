# LiteMapChooser
This plugin allows you to change map, nominate map, rtv

# Fork
This fork contains:
* Some minor fixes to be more compatible with the latest versions of CSSharp
* A fix for the error 'CSSharp: Native XXXXX was invoked on a non-main thread'https://github.com/Shlimmst/LiteMapChooser/blob/main/README.md
* A new config variable "MapChangeDelayInSeconds"

If there are any problems, make an issue. Since this is not my main focus I will try to get back to them.

**NOTE: this has been tested on gamemodes without rounds (e.g. Surf)**

# Installation
1. Install [CounterStrike Sharp](https://github.com/roflmuffin/CounterStrikeSharp) and [Metamod:Source](https://www.sourcemm.net/downloads.php/?branch=master)

2. Download LiteMapChooser

3. Unzip the archive and upload it to the game server

# Configs
The config is created automatically in the same place where the dll is located
```
{
  "RoundsBeforeNomination": 6,	//After how many rounds is given the opportunity to nominate a map
  "VotingRoundInterval": 5,	//How many rounds after which to start voting on a completed map
  "VotingTimeInterval": 10.0, //How long to start voting on a completed map (in minutes)
  "Needed": 0.6, //Percentage of players needed to rockthevote
  "MapChangeDelayInSeconds": 30 //Amount of seconds between the map being chosen and the actual map change
}
```
for maps from the workshop, add the prefix "ws:" to maps.txt
```
cs_italy
cs_office
de_dust2
de_inferno
de_mirage
de_nuke
de_overpass
de_vertigo
ws:surf_beginner
ws:surf_void
ws:surf_utopia_njv
ws:surf_ace
ws:surf_kitsune_cs2
```

# Commands
**ccs_rtv**,**!rtv** - starts the map change process

**css_nominate**,**!nominate** - opens the map menu
