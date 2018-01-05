Faction Permissions allows faction leaders to grant specific permissions to specific relations and roles. Permissions were first added on [Jan 4 '17](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d).

## Command Usages
Command | Description
--- | ---
/f perm [relation] [action] [access] | Manage permissions for your Faction
/f perm enemy build deny | Deny build to an enemy
/f perm all lever deny | Deny everyone from building
/f perm truce all allow | Allow truces to do everything

## Permissions
Permissions are defined by [Actions](https://github.com/drtshock/Factions/blob/1.6.x/src/main/java/com/massivecraft/factions/zcore/fperms/Action.java). Actions are something that a user does on the server. To grant a user permission to do something, you must specify the `Action` in the command. 

Here is a list of all actions and what they do.

Implemented Date | Action | Description
--- | --- | ---
[Jan 4 '17](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d) | build | Allow placing blocks
[Jan 4 '17](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d) | destroy | Allow breaking blocks
[Jan 4 '17](https://github.com/drtshock/Factions/commit/687bac31dbb885e650bc50e1e99e491865869b2d) | frostwalk | Allow frost walking
TBD | door | Allow the use of doors
TBD | button | Allow the use of buttons
TBD | lever | Allow the use of levers
TBD | container | Allow the use of containers (chests, enderchests)
TBD | invite | Allow inviting new players
TBD | kick | Allow kicking players
TBD | sethome | Allow setting the Faction home
TBD | withdraw | Allow withdrawing from the Faction bank
[Jan 4 '17](https://github.com/drtshock/Factions/commit/4db185e3ee757be2bea410f6e3164737c612bfc1) | promote | Allow promoting / demoting other players. Doesn't allow promotion up to admin.
TBD | perms | Allow managing permissions