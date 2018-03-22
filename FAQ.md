### Queston: Does this need McCore?
**Answer:** No, it does not need McCore
### Question: My Faction does not show up in chat, What can i do?
**Answer:**
Alright, first off you need a chat plugin. We recommend EssentialsX (https://github.com/EssentialsX/Essentials) since it is free and is very active. Usually, FactionsUUID automatically adds your faction at the end of the chat for you, but using the variable [FACTION] should make it work. If that doesn't work, here are some other options.

Chat Control Pro is a premium resource and has tons of features besides warning people. It has chat formatting, listeners, handlers, etc. It is very active as well, but as I said, it is premium. You MUST enable chat formatting in the formatting.yml file it creates in order for this to work. If you have EssentialsChat (which isn't working if you choose this option) it might conflict with ChatControl, so beware if it doesn't work.
What you do is this: In the formatting.yml file, there is a `Formats:` section. There, find `Chat:` and add this into the section:

    `Faction:
      Message: '{rel_factions_relation_color}{factionsuuid_player_role}{factionsuuid_faction_name}&r '`

Make sure you have PlaceholderAPI installed, and have done /papi ecloud download FactionsUUID. Otherwise, this will not work. After you have done that, do /restart and wait for your server to load. If all goes well - good job! If it doesn't - make sure no other chat-formatting plugins are enabled, like EssentialsChat, DeluxeChat, HeroChat, etc.

### HOW DO I CLAIM THE WARZONE AND SAFEZONE

**Answer:** To claim land for the warzone and safezone, you need to execute the following command:
1. /f bypass
2. /f claim <radius> [Warzone/SafeZone]

Provided they have the necessary permissions to do so.