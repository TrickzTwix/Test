This configuration file is stored on disk at `/mstore/factions_uconf@[UNIVERSE_ID]/instance.json?`.

source file: [factions.entity.UConf](//github.com/MassiveCraft/Factions/blob/master/src/com/massivecraft/factions/entity/UConf.java)

```json
{
    "enabled": true,
    "factionIdNone": "3defeec7-b3b1-48d9-82bb-2a8903df24e3",
    "factionIdSafezone": "bfe88990-ce13-412f-b839-8784a02ef8b0",
    "factionIdWarzone": "04386096-acb8-484f-8daa-96c6331fa56a",
    "defaultPlayerFactionId": "3defeec7-b3b1-48d9-82bb-2a8903df24e3",
    "defaultPlayerRole": "RECRUIT",
    "defaultPlayerPower": 0,
    "defaultFactionOpen": false,
    "defaultFactionFlags": {
        "PERMANENT": false,
        "PEACEFUL": false,
        "INFPOWER": false,
        "POWERLOSS": true,
        "PVP": true,
        "FRIENDLYFIRE": false,
        "MONSTERS": true,
        "EXPLOSIONS": true,
        "FIRESPREAD": true,
        "ENDERGRIEF": false
    },
    "defaultFactionPerms": {
        "BUILD": [
            "LEADER",
            "OFFICER",
            "MEMBER",
            "ALLY"
        ],
        "PAINBUILD": [],
        "DOOR": [
            "LEADER",
            "OFFICER",
            "MEMBER",
            "RECRUIT",
            "ALLY"
        ],
        "BUTTON": [
            "LEADER",
            "OFFICER",
            "MEMBER",
            "RECRUIT",
            "ALLY"
        ],
        "LEVER": [
            "LEADER",
            "OFFICER",
            "MEMBER",
            "RECRUIT",
            "ALLY"
        ],
        "CONTAINER": [
            "LEADER",
            "OFFICER",
            "MEMBER"
        ],
        "INVITE": [
            "LEADER",
            "OFFICER"
        ],
        "KICK": [
            "LEADER",
            "OFFICER"
        ],
        "SETHOME": [
            "LEADER",
            "OFFICER"
        ],
        "WITHDRAW": [
            "LEADER",
            "OFFICER"
        ],
        "TERRITORY": [
            "LEADER",
            "OFFICER"
        ],
        "ACCESS": [
            "LEADER",
            "OFFICER"
        ],
        "DISBAND": [
            "LEADER"
        ],
        "PERMS": [
            "LEADER"
        ]
    },
    "powerMax": 10,
    "powerMin": 0,
    "powerPerHour": 2,
    "powerPerDeath": -2,
    "canLeaveWithNegativePower": true,
    "factionMemberLimit": 0,
    "factionPowerMax": 0,
    "factionNameLengthMin": 3,
    "factionNameLengthMax": 16,
    "factionNameForceUpperCase": false,
    "claimsMustBeConnected": true,
    "claimingFromOthersAllowed": true,
    "claimsCanBeUnconnectedIfOwnedByOtherFaction": true,
    "claimsRequireMinFactionMembers": 1,
    "claimedLandsMax": 0,
    "homesEnabled": true,
    "homesMustBeInClaimedTerritory": true,
    "homesTeleportCommandEnabled": true,
    "homesTeleportAllowedFromEnemyTerritory": true,
    "homesTeleportAllowedFromDifferentWorld": true,
    "homesTeleportAllowedEnemyDistance": 32,
    "homesTeleportIgnoreEnemiesIfInOwnTerritory": true,
    "permanentFactionsDisableLeaderPromotion": false,
    "actionDeniedPainAmount": 2,
    "disablePVPForFactionlessPlayers": false,
    "enablePVPAgainstFactionlessInAttackersLand": false,
    "territoryShieldFactor": 0.3,
    "denyCommandsPermanentFactionMember": [],
    "denyCommandsTerritoryRelation": {
        "ENEMY": [
            "home",
            "sethome",
            "tpahere",
            "tpaccept",
            "tpa",
            "warp",
            "warps",
            "spawn",
            "wtp",
            "uspawn",
            "utp",
            "mspawn",
            "mtp",
            "fspawn",
            "ftp",
            "jspawn",
            "jtp"
        ],
        "NEUTRAL": [],
        "TRUCE": [],
        "ALLY": [],
        "MEMBER": []
    },
    "lwcRemoveOnChange": {
        "BUY": false,
        "SELL": false,
        "CONQUER": false,
        "PILLAGE": false
    },
    "econEnabled": false,
    "econLandReward": 0,
    "econUniverseAccount": "",
    "econChunkCost": {
        "BUY": 30,
        "SELL": -20,
        "CONQUER": -10,
        "PILLAGE": -10
    },
    "econCostCreate": 200,
    "econCostSethome": 0,
    "econCostJoin": 0,
    "econCostLeave": 0,
    "econCostKick": 0,
    "econCostInvite": 0,
    "econCostDeinvite": 0,
    "econCostHome": 0,
    "econCostName": 0,
    "econCostDescription": 0,
    "econCostTitle": 0,
    "econCostOpen": 0,
    "econRelCost": {
        "ENEMY": 0,
        "ALLY": 0,
        "TRUCE": 0,
        "NEUTRAL": 0
    },
    "bankEnabled": true,
    "bankFactionPaysCosts": true,
    "bankFactionPaysLandCosts": true
}
```
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