This configuration file is stored on disk at `plugins/Factions/???/???`.

source file: [factions.entity.UConf](//github.com/MassiveCraft/Factions/blob/master/src/com/massivecraft/factions/entity/UConf.java)

| Configuration name | Default value | Description | Acceptable values |
| ------------------ | ------------- | ----------- | ----------------- |
| enabled            | true          | Is Factions enabled on this universe? | true/false |
| factionIdNone      | Random UUID   | Faction ID for 'Wilderness' / no faction | UUID |
| factionIdSafezone  | Random UUID   | Faction ID for SafeZone | UUID |
| factionIdWarzone   | Random UUID   | Faction ID for WarZone | UUID |
| defaultPlayerFactionId | (same as factionIdNone) | Faction for players entering this Universe | UUID |
| defaultPlayerRole  | RECRUIT       | Default role for players entering an existing faction | [Relation](//github.com/MassiveCraft/Factions/blob/master/src/com/massivecraft/factions/Rel.java) |
| defaultPlayerPower | 0.0           | Default power for players entering this Universe | decimal |
| defaultFactionOpen | false         | Whether players can freely join the default faction | true/false |
| defaultFactionFlags | [see below](#default-faction-flags) | Faction flags for newly created factions | FactionFlag setup |
| defaultFactionPerms | [see below](#default-faction-permissions) | Faction permissions for newly created factions | FactionPerm setup |
| powerMax           | 10.0          | Maximum power per player | decimal |
| powerMin           | 0.0           | Lowest power that **TODO** | decimal |
| powerPerHour       | 2.0           | Power gain for each hour of playing | decimal |
| powerPerDeath      | -2.0          | Power loss on each death | decimal |
| canLeaveWithNegativePower | true   | Whether faction members can leave when they have negative power. Some server owners prefer this, to avoid having an incentive to leave the faction temporarily. | true/false |
| factionMemberLimit | 0 (no limit)  | Maximum number of players per faction | number |
| factionPowerMax    | 0.0 (no limit) | Maximum power in a single faction | decimal
| factionNameLengthMin | 3           | Smallest allowable faction name length | number |
| factionNameLengthMax | 16          | Largest allowable faction name length. Pre-2.0, this number was 8. | number |
| factionNameForceUpperCase | false  | **TODO** | true/false |
| claimsMustBeConnected | true       | Whether claimed land must be connected to your first claim. | true/false |
| claimingFromOthersAllowed | true   | Whether factions may steal land from other factions. | true/false |
| claimsCanBeUnconnectedIfOwnedByOtherFaction | true | Whether the connection requirement is ignored while stealing land. | true/false |
| claimsRequireMinFactionMembers | 1 | How many faction members are required before any claims can be made. | number |
| claimedLandsMax    | 0 (no limit)  | Maximum number of claimed 16x16 areas per faction. *See also: factionPowerMax* | number |
| homesEnabled       | true          | Whether faction homes are enabled. | true/false |
| homesMustBeInClaimedTerritory | true | Whether faction homes must be inside your territory. | true/false |
| homesTeleportCommandEnabled | true | May players use `/f home` to teleport to their faction home? | true/false |
| homesTeleportAllowedFromEnemyTerritory | true | May players use `/f home` while in enemy territory, subject to the EnemyDistance restriction? | true/false |
| homesTeleportAllowedFromDifferentWorld | true | Is `/f home` allowed from another world (e.g. Nether)? | true/false |
| homesTeleportAllowedEnemyDistance | 32.0 | The minimum distance from all enemy faction members to use `/f home`. | decimal |
| homesTeleportIgnoreEnemiesIfInOwnTerritory | true | Is the AllowedEnemyDistance ignored while in your own territory? | true/false |
| permanentFactionsDisableLeaderPromotion | false | Is promotion to Leader disallowed in permanent factions (don't disappear with 0 players)? | true/false |
| actionDeniedPainAmount | 2         | How much to damage players who perform a pain-disallowed action. | number |
| disablePVPForFactionlessPlayers | false | Are players in the default faction disallowed from PvPing? | true/false |
| enablePVPAgainstFactionlessInAttackersLand | false | Is the previous option overridden while in the land of the attacking player? Note that this does mean the factionless player cannot hit back. | true/false |
| territoryShieldFactor | 0.3        | Percent to reduce damage while in your own territory. | decimal (percent) |
| denyCommandsPermanentFactionMember | empty list | Commands to deny members of a permanent faction. | list of string |
| denyCommandsTerritoryRelation | [see below](#default-deny-commands) | Commands to deny in faction territory by players with this relation | map of Rel to list of string |
| lwcRemoveOnChange 
                     |               |
