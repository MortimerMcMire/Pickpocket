# Pickpocket
MWSE-lua Pickpocket mod for TES3: Morrowind
Adds a custom real-time menu to pickpocketing and restores a formerly-useless mechanic.
Version 2.1

### 2.1 Update

Sigourn was gracious enough to take feedback and update my mod to fix a window bug when loading a save

### About: 
This completely changes how pickpocketing works. When sneaking and mousing over npcs, you will see a new window pop up. 
Example: https://streamable.com/2w3m9

In that window will be all of the items you are able to steal. If you are undetected, and press the activate key (spacebar by default), you take that item.
You will only see items you can steal. If the npc has items you are unable to steal at your current skill level, it will indicate so.

The math works like this: If your security skill >= (their security skill + item weight) -> You can steal it.

There are caveats; if they have it equipped, they get a bonus to their check. That means your chances of stealing a dagger off a thief are
pretty much zero. But it's possible.

Likewise, it is very unlikely to steal off a merchant. They have an additional bonus on top of that. After all, merchants HAVE to be wary of thieves.

By default you cannot steal weapons and shields. Effortless supplies of ebony maces is pretty broken! Disable it in options if you wish.

Finally, there is an option in settings to allow you to steal armor/clothing npcs wear. The default bonus on that is also 50, but this is still incredibly broken and unrealistic. This option is disabled for good reason, but feel free to enable it and set the requirement to 200 if you want.

### Why I made this / thoughts:

I can't think of anyone who used pickpocketing in the vanilla game. 
It did a series of checks and if any one of them failed you were noticed. A similar effect is in play with Skyrim, except the chance is displayed on your screen.

Both options are bad, and here's why: I don't trust you, or myself not to save and reload. You might have a stronger will than I do, but if I see a 30% chance I'm going to save and reload until I get that damn ring. This mod also gives you the chance to steal weapons/shields off of people. It's very tough, but possible. I wanted to be able to steal Auriel's Shield, and dammit now I can!

"Can I use sneak instead of security?"
No. You can change it in one line of the lua if you want but I will never provide that option.
-Security is worthless with the prevalence of open spells + open scrolls
-The same skill that governs precision with lockpicks should govern sleight of hand
-Your sneak is already factored into the whole equation as you can't take anything successfully when seen
-Putting both on the same attribute means you just train sneak and become a thief god

There is a Mod Configuration Menu included. In that you have the option to:
-Adjust penalties for pickpocketing
-Adjust difficulty of stealing equipped items
-Adjust bonus given to merchants
-Allow stealing of weapons/armor/jewelry
-Allow stealing of worn armor
-Adjust difficulty of stealing said armor
-Enable/disable the mod entirely
-Hide NPC tooltips when sneaking (only affects it if you are already sneaking when you mouseover an npc)

### Requirements:

-MGEXE
-MWSE-lua beta branch (available here: https://nullcascade.com/mwse/mwse-dev.zip )
-OpenMW is not supported

### Installation:

-Drag and drop data files folder, merge if asked.

### Uninstallation:

-Remove or rename the main.lua file. There is also a mod configuration option to disable the mod as well.

### Special Thanks:

Sigourn - Bugfixing
Nullcascade - MWSE
Hrnchamd - MWSE
