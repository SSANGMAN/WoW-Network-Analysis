# WoW-Network-Analysis

Overview
The World of Warcraft Avatar History Dataset is a collection of records that detail information about player characters in the game over time. It includes information about their character level, race, class, location, and social guild. The Kaggle version of this dataset includes only the information from 2008 (and the dataset in general only includes information from the 'Horde' faction of players in the game from a single game server).

Full Dataset Source and Information: http://mmnet.iis.sinica.edu.tw/dl/wowah/  
Code used to clean the data: https://github.com/myles-oneill/WoWAH-parser  
Ideas for Using the Dataset
From the perspective of game system designers, players' behavior is one of the most important factors they must consider when designing game systems. To gain a fundamental understanding of the game play behavior of online gamers, exploring users' game play time provides a good starting point. This is because the concept of game play time is applicable to all genres of games and it enables us to model the system workload as well as the impact of system and network QoS on users' behavior. It can even help us predict players' loyalty to specific games.

Open Questions
Understand user gameplay behavior (game sessions, movement, leveling)
Understand user interactions (guilds)
Predict players unsubscribing from the game based on activity
What are the most popular zones in WoW, what level players tend to inhabit each?
Wrath of the Lich King
An expansion to World of Warcraft, "Wrath of the Lich King" (Wotlk) was released on November 13, 2008. It introduced new zones for players to go to, a new character class (the death knight), and a new level cap of 80 (up from 70 previously). This event intersects nicely with the dataset and is probably interesting to investigate.

Map
This dataset doesn't include a shapefile (if you know of one that exists, let me know!) to show where the zones the dataset talks about are. Here is a list of zones an information from this version of the game, including their recommended levels: http://wowwiki.wikia.com/wiki/Zones_by_level_(original) .

Update (Version 3): dmi3kno has generously put together some supplementary zone information files which have now been included in this dataset. Some notes about the files:

Note that some zone names contain Chinese characters. Unicode names are preserved as a key to the original dataset. What this addition will allow is to understand properties of the zones a bit better - their relative location to each other, competititive properties, type of gameplay and, hopefully, their contribution to character leveling. Location coordinates contain some redundant (and possibly duplicate) records as they are collected from different sources. Working with uncleaned location coordinate data will allow users to demonstrate their data wrangling skills (both working with strings and spatial data).
