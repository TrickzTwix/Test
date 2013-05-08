This configuration file is stored on disk at `plugins/Factions/???`.

source file: [factions.entity.MConf](https://github.com/MassiveCraft/Factions/blob/master/src/com/massivecraft/factions/entity/MConf.java)

| Configuration name | Default value | Description | Acceptable values |
| ------- |:---------:| --- |
| taskPlayerPowerUpdateMinutes | 1 | How often to run the power update | decimal |
| taskPlayerDataRemoveMinutes | 5 | How often to run the data removal | decimal |
| taskEconLandRewardMinutes | 20 | How often to run the land reward | decimal |
| -------- |
| removePlayerDataWhenBanned | true | Whether or not to delete the data for a player when they are banned | true/false |
| removePlayerDataAfterInactiveDays | 20.0 | How many days a player has to be inactive before their data is deleted | decimal |
| -------- |
| radiusClaimFailureLimit | 9 | When doing a radius claim, how many fails in a row to tolerate before aborting | number |
| radiusClaimRadiusLimit | 5 | Maximum radius when using radius claim. (Load = radius^2) | number |
| -------- |
| chatSetFormat | false | Override chat format from other plugins? | true/false |
| chatSetFormatAt | EventPriority.LOWEST | What EventPriority to set the chat format at. | [EventPriority](//link_goes_here) |
| chatSetFormatTo | `<{factions_relcolor}§l{factions_roleprefix}§r{factions_relcolor}{factions_name|rp}§f%1$s> %2$s` | What chat format to override to | string |
| chatParseTags | true | Parse tags in the chat format? | true/false |
| chatParseTagsAt | EventPriority.LOW | What EventPriority to parse the tags at. | [EventPriority](//link_goes_here) |
| herochatFactionName | "Faction" | HeroChat faction-only channel long name. | string |
| herochatFactionNick | "F" | HeroChat faction-only channel short name. | string |
| herochatFactionFormat | "{color}[&l{nick}&r{color} &l{factions_roleprefix}&r{color}{factions_title|rp}{sender}{color}] &f{msg}" | What chat format too use for the faction-only channel. | string |
| herochatFactionColor | ChatColor.GREEN | What color the faction-only channel should be. | [ChatColor](//link_goes_here) |
| herochatFactionDistance | 0 | See HeroChat documentation. (0=unlimited?) | number |
| boolean herochatFactionIsShortcutAllowed | false | **TODO** | true/false |
| boolean herochatFactionCrossWorld | true | **TODO** | true/false |
| boolean herochatFactionMuted | false | **TODO** | true/false |
| Set<String> herochatFactionWorlds | new HashSet<String>() | 
// HeroChat: The Allies Channel
| String herochatAlliesName | "Allies" | 
| String herochatAlliesNick | "A" | 
| String herochatAlliesFormat | "{color}[&l{nick}&r&f {factions_relcolor}&l{factions_roleprefix}&r{factions_relcolor}{factions_name|rp}{sender}{color}] &f{msg}" | 
| ChatColor herochatAlliesColor | ChatColor.DARK_PURPLE | 
| int herochatAlliesDistance | 0 | 
| boolean herochatAlliesIsShortcutAllowed | false | 
| boolean herochatAlliesCrossWorld | true | 
| boolean herochatAlliesMuted | false | 
| Set<String> herochatAlliesWorlds | new HashSet<String>() | 
| -------- |
// COLORS
| -------- |
| ChatColor colorMember | ChatColor.GREEN | 
| ChatColor colorAlly | ChatColor.DARK_PURPLE | 
| ChatColor colorTruce | ChatColor.LIGHT_PURPLE | 
| ChatColor colorNeutral | ChatColor.WHITE | 
| ChatColor colorEnemy | ChatColor.RED | 
| ChatColor colorNoPVP | ChatColor.GOLD | 
| ChatColor colorFriendlyFire | ChatColor.DARK_RED | 
//| ChatColor colorWilderness | ChatColor.DARK_GREEN | 
| -------- |
// PREFIXES
| -------- |
| String prefixLeader | "**" | 
| String prefixOfficer | "*" | 
| String prefixMember | "+" | 
| String prefixRecruit | "-" | 
| -------- |
// DERPY OVERRIDES
| -------- |
// TODO: Should worldsNoPowerLoss rather be a bukkit permission node?
// TODO: These are derpy because they possibly use an invalid design approach.
// After universe support is added. Would some of these be removed?
// Could it also be more customizeable using some sort of permission lookup map?
// mainly for other plugins/mods that use a fake player to take actions, which shouldn't be subject to our protections
| Set<String> playersWhoBypassAllProtection | new LinkedHashSet<String>() | 
| Set<String> worldsNoClaiming | new LinkedHashSet<String>() | 
| Set<String> worldsNoPowerLoss | new LinkedHashSet<String>() | 
| Set<String> worldsIgnorePvP | new LinkedHashSet<String>() | 
| -------- |
// EXPLOITS
| -------- |
| boolean handleExploitObsidianGenerators | true | 
| boolean handleExploitEnderPearlClipping | true | 
| boolean handleExploitTNTWaterlog | false | 
| -------- |
// LOGGING
| -------- |
| boolean logFactionCreate | true | 
| boolean logFactionDisband | true | 
| boolean logFactionJoin | true | 
| boolean logFactionKick | true | 
| boolean logFactionLeave | true | 
| boolean logLandClaims | true | 
| boolean logLandUnclaims | true | 
| boolean logMoneyTransactions | true | 
| boolean logPlayerCommands | true | 