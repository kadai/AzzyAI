# AzzyAI-Fork for kRO Homunculus Update

This is not the official AzzyAI but a fork.
For the original repository please refer to: https://github.com/SpenceKonde/AzzyAI

For more information, see the official website: http://drazzy.com/ro/ai

## Versions
Currently, there are two versions of this AI:
### [Main](https://github.com/Kisaro/AzzyAI/archive/master.zip)
This branch attempts to be close to vanilla azzyai without further modifications except introducing the skill-changes below. **Pick this version if you want to be as close to vanilla azzyai as possible and like tinkering with the settings.**
### [Custom](https://github.com/Kisaro/AzzyAI/archive/custom-settings.zip)
Contains everything above, plus some personal adjustments to auto-cast some skills and modifications to cooldowns to aim for 100% uptime of various buffs. **Pick this version if you want an AI tailored to Amistr+Dieter out of the box.**

## Install ##
 - Download a version ([main](https://github.com/Kisaro/AzzyAI/archive/master.zip) or [custom](https://github.com/Kisaro/AzzyAI/archive/custom-settings.zip)) of your choice from above
 - Open the downloaded ZIP-file
 - Navigate to your Ragnarok-folder
 - Copy the *USER_AI*-folder from the ZIP-file into the *AI*-folder of your Ragnarok-folder (will overwrite the currently installed user-AI, make backups!)
 - To instantly see changes ingame, *Rest* -> *Call* your Homunculus or use `@refresh` if you have access to server commands

## Debugging ##
You can debug the Homunculus AI and what information it is seeing with the command "/traceai", this will write all the log calls to a file named "TraceAI.txt" inside your main Ragnarok Online install folder. Other text files with log information may also be generated.

Be warned that activating this log saving feature may cause the client to lag heavily, make it unresposive and even make it crash. Only use it when you know exactly what you are doing.

## Updating the AI ##
After you have downloaded the code contained in this repository, you can copy this files into your ./AI/USER_AI folder. Make a backup of your old folder if you want to preserve your old settings.

If you are updating from another AzzyAI version and want to preserve your current settings, it is adviced you backup and then restore the next files:
 - H_Config.lua
 - H_Extra.lua
 - H_PVP_Tact.lua
 - H_Tactics.lua
 - M_Config.lua
 - M_Extra.lua
 - M_PVP_Tact.lua
 - M_Tactics.lua

## Changes ##
Skills are updated to their new max-level to reflect [official kRO changes](http://ro.gnjoy.com/news/notice/View.asp?BBSMode=10001&seq=6843&curpage=1)

This includes the following skills:
 - Eira
   - Xeno Slasher
   - Eraser Cutter
 - Bayeri
   - Stahl Horn
   - Heilige Stange
 - Sera
   - Needle of Paralyze
   - Pain Killer
 - Dieter
   - Lava Slide
   - Pyroclastic
 - Eleanor
   - Silvervein Rush
   - Midnight Frenzy

Addionally, with the arrival of 4th jobs and new homunculus skills, the following new skills have been added:
 - Dieter
   - Tempering
   - Blast Forge (Thanks to [vorpal1337](https://github.com/vorpal1337))
   
## Disclaimer ##
Certain functionality may not work as expected or not at all due to the declining support of AIs in newer clients, backup your current AI in any case before applying. Feel free to open issues if you find bugs. **Pull-requests are welcome!**
