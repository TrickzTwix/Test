This configuration file is stored on disk at `plugins/Factions/???`.

source file: [factions.entity.MConf](https://github.com/MassiveCraft/Factions/blob/master/src/com/massivecraft/factions/entity/MConf.java)

| Configuration name | Default value | Description | Acceptable values |
| ------------------ | ------------- | ----------- | ----------------- |
| taskPlayerPowerUpdateMinutes | 1 | How often to run the power update | decimal |
| taskPlayerDataRemoveMinutes | 5 | How often to run the data removal | decimal |
| taskEconLandRewardMinutes | 20 | How often to run the land reward | decimal |
| removePlayerDataWhenBanned | true | Whether or not to delete the data for a player when they are banned | true/false |
| removePlayerDataAfterInactiveDays | 20.0 | How many days a player has to be inactive before their data is deleted | decimal |
| radiusClaimFailureLimit | 9 | When doing a radius claim, how many fails in a row to tolerate before aborting | number |
| radiusClaimRadiusLimit | 5 | Maximum radius when using radius claim. (Load = radius^2) | number |
| chatSetFormat | false | Override chat format from other plugins? | true/false |
| chatSetFormatAt | EventPriority.LOWEST | What EventPriority to set the chat format at. | [EventPriority](//link_goes_here) |
| chatSetFormatTo | [see below](#chatsetformatto-default-value) | What chat format to override to | string |
| chatParseTags | true | Parse tags in the chat format? | true/false |
| chatParseTagsAt | EventPriority.LOW | What EventPriority to parse the tags at. | [EventPriority](//link_goes_here) |
| herochatFactionName | "Faction" | HeroChat faction-only channel long name. | string |
| herochatFactionNick | "F" | HeroChat faction-only channel short name. | string |
| herochatFactionFormat | [see below](#herochatfactionformat-default-value) | What chat format too use for the faction-only channel. | string |
| herochatFactionColor | ChatColor.GREEN | What color the faction-only channel should be. | [ChatColor](//link_goes_here) |
| herochatFactionDistance | 0 | See HeroChat documentation. (0=unlimited?) | number |
| boolean herochatFactionIsShortcutAllowed | false | **TODO** | true/false |
| boolean herochatFactionCrossWorld | true | **TODO** | true/false |
| boolean herochatFactionMuted | false | **TODO** | true/false |
| Set<String> herochatFactionWorlds | new HashSet<String>() | 
| String herochatAlliesName | "Allies" | 
| String herochatAlliesNick | "A" | 
| String herochatAlliesFormat | [see below](#herochatalliesformat-default-value) | 
| ChatColor herochatAlliesColor | ChatColor.DARK_PURPLE | 
| int herochatAlliesDistance | 0 | 
| boolean herochatAlliesIsShortcutAllowed | false | 
| boolean herochatAlliesCrossWorld | true | 
| boolean herochatAlliesMuted | false | 
| Set<String> herochatAlliesWorlds | new HashSet<String>() |
| ChatColor colorMember | ChatColor.GREEN | 
| ChatColor colorAlly | ChatColor.DARK_PURPLE | 
| ChatColor colorTruce | ChatColor.LIGHT_PURPLE | 
| ChatColor colorNeutral | ChatColor.WHITE | 
| ChatColor colorEnemy | ChatColor.RED | 
| ChatColor colorNoPVP | ChatColor.GOLD | 
| ChatColor colorFriendlyFire | ChatColor.DARK_RED | 
| String prefixLeader | "**" | 
| String prefixOfficer | "*" | 
| String prefixMember | "+" | 
| String prefixRecruit | "-" | 
| playersWhoBypassAllProtection | empty list | Players who bypass all protection checks. Intended for other plugins that use a fake player to take actions. *May be removed in favor of world config files.* | list of string |
| worldsNoClaiming | empty list | Worlds where no faction claiming is allowed. **This overrides `/f bypass`.** | list of string |
| worldsNoPowerLoss | empty list | Worlds where death does not cause power loss. *May be removed in favor of world config files.* | list of string |
| worldsIgnorePvP | new LinkedHashSet<String>() | Worlds where Factions should perform no checks relating to PvP. *May be removed in favor of world config files.* | list of string |
| handleExploitObsidianGenerators | true | Should Factions prevent the obsidian generator exploit? | true/false |
| boolean handleExploitEnderPearlClipping | true | Should Factions attempt to block attempts at ender pearl clipping? | true/false |
| boolean handleExploitTNTWaterlog | false | Should Factions attempt to block ???**TODO**??? ? | true/false |
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