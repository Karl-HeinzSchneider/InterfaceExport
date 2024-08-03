Fork
====================
This fork fixes the tool for the use on windows, and provides .bat files for automation.

### Usage ###
* clone the project
* get the win64 (modified) lua runtime from [here](https://www.townlong-yak.com/casc/) => Dependencies => Win64 => `lua52-m64.exe`, and copy it into the project root
* run it like so: `lua52-m64.exe export.lua classic live code` (command line settings see below), or use one of the provided .bat files, e.g. `classic-live-code.bat`
* locate the files inside the `\_files` folder, e.g. `\_files\wow_classic\Interface`

# WoW Interface Export #

This tool that will extract the interface files for World of Warcraft, either from a local install or from the CDN.

Usage:
`lua export.lua [project] [branch] [filter]`

### project ###
  * `retail`      - Default
  * `classic`     - Most recent Classic version 

These can also be used to refer to a specific WoW Classic project

  * `wrath`       - WotLK Classic
  * `classic_era` - Vanilla Classic
  * `vanilla`     - Vanilla Classic

### branch ###
  * `live` - Default
  * `ptr`
  * `ptr2` - Retail client only
  * `beta`

### filter ###
  * `all`  - Default
  * `code`
  * `art`
  * `png` - Like `art`, but also converts to png


Tools used:
  * [LuaCasc](https://www.townlong-yak.com/casc/)
  * [LuaDBC](https://www.townlong-yak.com/casc/dbc/)
  * [LuaFileSystem](https://luarocks.org/modules/hisham/luafilesystem)
  * [LuaCSV](https://luarocks.org/modules/geoffleyland/csv) (optional)
