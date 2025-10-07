# Important Standards when Modding for SuperStates Mod for EU5 #

_NOTICE: This is a work in progress that likely will details change as work on SuperStates Mod in EU5 progresses, these are prelimary standards mostly taken from standards already used in the EU4 project._

## Scope of Area ##

The mod's scope of area is defined as the **subnational entities** of nations with a **federal system** within the regions of **Australia, Oceania, North and South America**.  Not all federal nations are included currently (Brazil, Venezeula, Argentina, the long since defunct Federal Republic of Central America; over time these are expected to be added).

Most nations that are added that aren't federal in nature are included as flavor and are only intended to appear as the game progresses and others are implimented from the start due to their past association with the United States or other federal nation.

**The mod _will not_ include any area or nation within _Africa, Asia, or Europe_ except in instances where particular territories are needed for accuracy to one of the federal nations added in the mod _(currently this is Australia with the Indian Ocean Territories)_.**  However, there could be the need due to performance problems to either empty out Africa (everything south of the Sahara) or remove a number of tribal nations.  This will be addressed when needed however.

## Nation Tags ## 
*(country_tags/00_countries.txt)*

Nation Tags are required to be unique in order to avoid issues with debugging the mod in game.
However, vanilla tags change from time to time in major updates and may require reassigning mod nations tags.
Mod nations that are in the vanilla game and are to be modified for the mod are to use the vanilla tag to make debugging easier and to keep the tag list in the game short.
Vanilla tags that are introduced due to an update take precedence over mod tags if the new vanilla tag is not in the area covered by the mod.
New tags and reassigned tags for nations wthin the mod area should be checked agaist the master tag list used by the mod and by vanilla before being included.

Too many tags could cause issues with the EU5 engine and generally is seen as an unnecessary performance hit.

## Provinces ##

There are important rules on modding provinces in SuperStates Mod for EU5.

This section likely will be replaced with simplier rules.  As the EU5 is detailed and large enough to handle single counties, it is expected that all 3,644 counties and equivilents in the United States likely will be represented in the EU5 mod.  The rules will be simple in that a county will have its proper name and proper county seat name.  This will apply to other nations as well, though there is no reason to expect any problems, if there problems encountered the rules will be listed here.

### Provinces.bmp ###
Colors for modded provinces that require a new province ID for SuperStates Mod in EU5 *MUST* be _Prime Numbers_ for the RGB values.
0,1,2,3,5,7,11,13,17,19,23,29,31,37,41,43,53,59,61,67,71,73,79,83,89,97,101,103,107,109,113,127,131,137,139,149,151,157,163,167,173,179,181,191,193,197,199,211,223,227,229,233,239,241,251

### Old EU4 Standards that likely will not apply but are currently being kept. ###

Provinces added to or modified on the map within the Mod's area are a collection of US county-equivalent local governments.  Not every nation (or even US state) follows the same idea as to what is a county or is an equivalent.  GIS maps are heavily used in drawing along modern boundaries of these county-equivalent local government bouandaries.  This tends to make blocky provinces in parts of the map but it is a design decision by the original author, KeoniPhoenix, to make editing the map more consistent and keep it somewhat accurate.

Province and their capital city names in the mod take the following format:  The collection of county-equivalent governments that make up a province are named based on the location of the largest county seat within that collection.  For instance the in Northeastern Illinois, Chicago being the largest city among the counties that make up the province requires the province to be named Cook and the capital city to be named Chicago.

This system breaks down however in some places that use different concepts when creating their local governments (Australia).  In the case of Australia, the province and capital city name are the city name of the metropolitan area.  For instance Sydney is a collection of differently sized local governments but grouped into the geographcial "Sydney" region, much like how the real life Greater London is just called London despite the City Corporation of London being only a square mile and a population of a few thousands.

Some Canadian provinces have only a single level of local government but have different types.  Provinces like Edmonton in Alberta are to be named after their principal cities but other provinces are named after the largest rural municipality that might apply (though for now most are named after principle cities).  Ontario and Quebec use a mixed system of counties and depending on which city can either be a single tier municipality, like Toronto, or a second tier munciaplity like Owen Sound.  Second Tier cities in Ontario and Quebec are to be treated as if they were in the US, and those that are county seats are the capital name and their county name is the province name.

Mexico operates mostly like the US however most of the time the county-equivalent is the only local government in that state, municipalities in Mexico are varied by state just like the United States.  The same rules apply in naming, though most large cities are also their municipality name in most, but not all, instances in Mexico.

Argentina, Brazil, and Venezeula all use similar systems for their county-equivalent municipalities as Mexico.

## Use of DLC Features ##

Some features of DLCs can be implemented within the mod, however the code for them must always restrict it so as to require the DLC in question to be active for the players playing the mod.  This is entirely a liability reduction issue between the Mod authors and Paradox Interactive.

## Mod Distribution ##

The mod's official release will always be from the Steam Workshop and Paradox Mods service and while the mod files can be downloaded from GitHub, it requires manual installation which **will never be supported except by special extraordinary means**.  Support for the mod requires proving the game is within one's Steam library and the discretion of the Mod Development Lead, KeoniPhoenix.

## Mod Name ##

The names SuperStates and SuperStates Mod and **any** variants (i.e. "New SuperStates Mod") is retained by the mod author, KeoniPhoenix.  If the mod is forked or modified into a new project, it must use a new and completely unique name as to avoid issues with this mod project.  If the issue is particularly egregious, official action may be taken.

Exceptions to this rule are mod repositories used by community members helping in the modding project as it would be cumbersome to require them to change names in order to help push and pull changes to the mod.  **This rule is primarily intended to be applied towards mods in the Steam Workshop or mods distributed in channels not authorized or sanctioned by Paradox Interactive.**
