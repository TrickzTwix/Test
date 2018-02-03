Faction Permissions allows faction leaders to grant specific permissions to specific relations and roles. Permissions were first added on [Jan 4 '17](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d).

## Command Usages
Command | Description
--- | ---
/f perm [relation] [action] [access] | Manage permissions for your Faction
/f perm enemy build deny | Deny build to an enemy
/f perm all lever deny | Deny everyone from building
/f perm truce all allow | Allow truces to do everything

## Permissions
Permissions are defined by [PermissableActions](https://github.com/drtshock/Factions/blob/1.6.x/src/main/java/com/massivecraft/factions/zcore/fperms/PermissableAction.java). PermissableActions are something that a user does on the server. To grant a user permission to do something, you must specify the `PermissableAction` in the command. 

Here is a list of all actions and what they do.

Implemented Date | Action | Description
--- | --- | ---
[Jan 4 '18](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d) | build | Allow placing blocks
[Jan 4 '18](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d) | destroy | Allow breaking blocks
[Jan 4 '18](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d) | frostwalk | Allow frost walking
[Feb 3 '18]() | door | Allow the use of doors
[Feb 3 '18](https://github.com/drtshock/Factions/commit/182022fe5fa15e44b2bc31ed2733dff8fbf1888c) | button | Allow the use of buttons
[Feb 3 '18](https://github.com/drtshock/Factions/commit/182022fe5fa15e44b2bc31ed2733dff8fbf1888c) | door | Allow use of doors
[Feb 3 '18](https://github.com/drtshock/Factions/commit/182022fe5fa15e44b2bc31ed2733dff8fbf1888c) | lever | Allow the use of levers
[Feb 3 '18](https://github.com/drtshock/Factions/commit/32b13befcecb751e3b2c6dbb1eba7daf245db87e) | container | Allow the use of containers (chests, enderchests, trapped chests)
[Feb 3 '18](https://github.com/drtshock/Factions/commit/baea59a1cd22a9427c388e870117a20556885279) | invite | Allow inviting new players
[Feb 3 '18](https://github.com/drtshock/Factions/commit/925014bd60ae7972c829366ff87214deea59871e) | kick | Allow kicking players
[Feb 3 '18](https://github.com/drtshock/Factions/commit/baea59a1cd22a9427c388e870117a20556885279) | sethome | Allow setting the Faction home
[Feb 3 '18](https://github.com/drtshock/Factions/commit/ad10222c2defed75de23eae252897899229bcdfe) | withdraw | Allow withdrawing from the Faction bank
[Jan 4 '18](https://github.com/drtshock/Factions/commit/4db185e3ee757be2bea410f6e3164737c612bfc1) | promote | Allow promoting / demoting other players. Doesn't allow promotion up to admin.
TBD | perms | Allow managing permissions
[Feb 3 '18](https://github.com/drtshock/Factions/commit/1b088ccd54cf79e7783f67d1cd293b35d65465ab) | warp | Allow use of /f warp
[Feb 3 '18](https://github.com/drtshock/Factions/commit/1b088ccd54cf79e7783f67d1cd293b35d65465ab) | setwarp | Allow use of /f setwarp