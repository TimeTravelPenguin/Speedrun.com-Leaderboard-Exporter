# Speedrun.com Leaderboard Exporter (SLE)

SLE is a program that exports basic speedrun.com leaderboard information for data analysis.
It helps to aid in the documentation of speedruns at a given time from speedrun.com

## How to use

To export a speedrun's leaderboard from speedrun.com, simply edit the config file, run the program, and click the appropriate prompts.

In the config file, you can modify the target user, game, category, and any query you wish to apply.
This is where a little bit of research and knowledge come in. Locate your speedrun leaderboard on the speedrun.com website, and find the game's ID. This is in the URL. An example would be *SMO* for Super Mario Odyssey, or, https://www.speedrun.com/smo.

Similary, you need to find the category ID by doing a similar method. Once on the website, click on the category and find it in the URL. For example:
* https://www.speedrun.com/smo#Any	-> category = 'any'
* https://www.speedrun.com/smo#100	-> category = '100'
* https://www.speedrun.com/smo#All_Missions	-> category = 'All_Missions'

Note that some leaderboards can be a little funky due to how they have been set up, and filtering with "variables" may be a neccisary requirement for optimal results. This will be made simpler in future updates.
For more information about query types, check it out [here](https://github.com/speedruncomorg/api/blob/master/version1/runs.md#get-runs).

More information can be found by looking into the speedrun.com API, which can be found [here](https://github.com/speedruncomorg/api).

## Once exported

Once the script is completed, you will have a .txt file with each line containing something similar to [these](https://github.com/TimeTravelPenguin/Speedrun.com-Leaderboard-Exporter/blob/master/ExampleFiles)

Each line has each data separated by a tab space, allowing for an easy import into spreadsheets (e.g. Microsoft Excel), for easy graphing, or analysis

## Downloading

The latest release can be downloaded from the [Releases Page](https://github.com/TimeTravelPenguin/Speedrun.com-Leaderboard-Exporter/releases). From here, the .zip file of recent build can be found. The files can then be extracted and opened.

## Requirements

As of the current build, it has the following system requirements:

* python 3
* the following python libraries (there is an installer to aid you in the download): Gevent

## Minor note

Some leaderboards have 'subcategories', filtered by things called 'variables'
At current, my program cannot filter these (easily), and there will be better managment for these in the future.

Some exmples are:
* Super Mario 64 - 16 star: N64, EMU, VC
* Super Mario Odyssey - any%: 1 Player, 2 Players

The leaderboard currently combines ALL runs. But, it will handle this in the future!
