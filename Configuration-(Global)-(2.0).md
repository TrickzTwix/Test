This configuration file is stored on disk at `plugins/Factions/???`.

source file: [factions.entity.MConf](https://github.com/MassiveCraft/Factions/blob/master/src/com/massivecraft/factions/entity/MConf.java)

| Configuration name | Default value | Description | Acceptable values |
| ------------------ | ------------- | ----------- | ----------------- |
| taskPlayerPowerUpdateMinutes | 1.0 | How often to run the power update | decimal |
| taskPlayerDataRemoveMinutes | 5.0 | How often to run the data removal | decimal |
| taskEconLandRewardMinutes | 20.0 | How often to run the land reward | decimal |
| removePlayerDataWhenBanned | true | Whether or not to delete the data for a player when they are banned | true/false |
| removePlayerDataAfterInactiveDays | 20.0 | How many days a player has to be inactive before their data is deleted | decimal |
| radiusClaimFailureLimit | 9 | When doing a radius claim, how many fails in a row to tolerate before aborting | number |
| radiusClaimRadiusLimit | 5 | Maximum radius when using radius claim. (Load = radius^2) | number |
| chatSetFormat | false | Override chat format from other plugins? | true/false |
| chatSetFormatAt | LOWEST | What EventPriority to set the chat format at. | [EventPriority](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/event/EventPriority.java) |
| chatSetFormatTo | [see below](#chatsetformatto-default-value) | What chat format to override to | string |
| chatParseTags | true | Parse tags in the chat format? | true/false |
| chatParseTagsAt | LOW | What EventPriority to parse the tags at. | [EventPriority](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/event/EventPriority.java) |
| herochatFactionName | "Faction" | HeroChat faction-only channel long name. | string |
| herochatFactionNick | "F" | HeroChat faction-only channel short name. | string |
| herochatFactionFormat | [see below](#herochatfactionformat-default-value) | What chat format to use for the faction-only channel. | string |
| herochatFactionColor | GREEN | What color the faction-only channel should be. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| herochatFactionDistance | 0 | **TODO** 0=unlimited? | number |
| herochatFactionIsShortcutAllowed | false | **TODO** | true/false |
| herochatFactionCrossWorld | true | **TODO** | true/false |
| herochatFactionMuted | false | **TODO** | true/false |
| herochatFactionWorlds | empty list | Which worlds to use HeroChat integration onfor the faction channel. *May be removed in favor of world config files.* | list of string |
| herochatAlliesName | "Allies" | HeroChat allies-only channel long name. | string |
| herochatAlliesNick | "A" | HeroChat allies-only channel short name. | string |
| herochatAlliesFormat | [see below](#herochatalliesformat-default-value) | What chat format to use for the faction-only channel. | string |
| herochatAlliesColor | DARK_PURPLE | What color the faction-only channel should be. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| herochatAlliesDistance | 0 | **TODO** 0=unlimited? | number |
| herochatAlliesIsShortcutAllowed | false | **TODO** | true/false |
| herochatAlliesCrossWorld | true | **TODO** | true/false |
| herochatAlliesMuted | false | **TODO** | true/false |
| herochatFactionWorlds | empty list | Which worlds to use HeroChat integration on for the allies channel. *May be removed in favor of world config files.* | list of string |
| colorMember | ChatColor.GREEN | Color for members of your own faction. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| colorAlly | ChatColor.DARK_PURPLE | Color for members of allied factions. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| colorTruce | ChatColor.LIGHT_PURPLE | Color for members of truced factions. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| colorNeutral | ChatColor.WHITE | Color for members of neutral factions. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| colorEnemy | ChatColor.RED | Color for members of enemy factions. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| colorNoPVP | ChatColor.GOLD | Color for members of peaceful factions. | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| colorFriendlyFire | ChatColor.DARK_RED | **TODO** | [ChatColor](/Bukkit/Bukkit/blob/master/src/main/java/org/bukkit/ChatColor.java) |
| prefixLeader | "**" | Chat prefix for faction leaders. | string |
| prefixOfficer | "*" | Chat prefix for faction officers. | string |
| prefixMember | "+" | Chat prefix for faction members. | string |
| prefixRecruit | "-" | Chat prefix for recruits. | string |
| playersWhoBypassAllProtection | empty list | Players who bypass all protection checks. Intended for other plugins that use a fake player to take actions. *May be removed in favor of world config files.* | list of string |
| worldsNoClaiming | empty list | Worlds where no faction claiming is allowed. **This overrides `/f bypass`.** | list of string |
| worldsNoPowerLoss | empty list | Worlds where death does not cause power loss. *May be removed in favor of world config files.* | list of string |
| worldsIgnorePvP | empty list | Worlds where Factions should perform no checks relating to PvP. *May be removed in favor of world config files.* | list of string |
| handleExploitObsidianGenerators | true | Should Factions prevent the obsidian generator exploit? | true/false |
| handleExploitEnderPearlClipping | true | Should Factions attempt to block attempts at ender pearl clipping? | true/false |
| handleExploitTNTWaterlog | false | Should Factions attempt to block ???**TODO**??? ? | true/false |
| boolean logFactionCreate | true | 
| boolean logFactionDisband | true | 
| boolean logFactionJoin | true | 
| boolean logFactionKick | true | 
| boolean logFactionLeave | true | 
| boolean logLandClaims | true | 
| boolean logLandUnclaims | true | 
| boolean logMoneyTransactions | true | 
| boolean logPlayerCommands | true | 

### chatSetFormatTo default value
```
<{factions_relcolor}§l{factions_roleprefix}§r{factions_relcolor}{factions_name|rp}§f%1$s> %2$s
```
### herochatFactionFormat default value
```
{color}[&l{nick}&r{color} &l{factions_roleprefix}&r{color}{factions_title|rp}{sender}{color}] &f{msg}
```
### herochatAlliesFormat default value
```
{color}[&l{nick}&r&f {factions_relcolor}&l{factions_roleprefix}&r{factions_relcolor}{factions_name|rp}{sender}{color}] &f{msg}
```