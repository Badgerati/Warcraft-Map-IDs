Warcraft Map IDs
================

Here is a list of nearly every possible Map ID for use with add-on development for World of Warcraft.
The IDs are already formatted for use with LUA, and can be freely used by everyone.

The IDs were obtained initially from WoWWiki, but also from an add-on I once created called QuestTracker - so a lot of
them have been collected purely by myself. You will find the IDs for all the expansions - including Cataclysm. Even
including the Map IDs for the Outland dungeons from an update Blizzard made later on.

As pointed out above, this is nearly all of the IDs. So if you do come across one not listed here, please tell me :)



Usage
-----

This is only a very minor point. Below is an example of how you could use these codes (this is the way I used them
for my add-on):

	
	local PlayerAreaID = GetCurrentMapAreaID();
	local PlayerLocation = AreaIDs[PlayerAreaID];

So we first get the integer value of where the player is located; be it in a city, region, dungeon or pvp-battlefield, etc.
Let's say the value of `749` is returned from `GetCurrentMapAreaID()`. When we index into the array with this value on
the next line, then the name of the area the player is in is returned - in this case: `Wailing Caverns`.