## Configuring the lang.yml file
There is a full, & color-coded version of the lang.yml.
The base colors are gray (&7) and red (&c), giving it a cool, PVP-like feeling about it. To change these color codes, doing `CMD/CNTRL + F` and typing in `&c/&7` should show you all the positions in the file. We suggest you use Sublime when editing documents, as it has a neat tool called **Find All** which you use to replace the color codes with the ones you desire.

```yaml
# Lang file for FactionsUUID by drtshock & Wizzle
# Use & for color codes.
# Made with love <3


root:
  AUTHOR: misc
  RESPONSIBLE: misc
  LANGUAGE: English
  ENCODING: UTF-8
  LOCALE: en_US
  REQUIRESUNICODE: 'false'
  DEFAULT: 'true'
  STATE: complete
  LOCAL:
    AUTHOR: misc
    RESPONSIBLE: misc
    LANGUAGE: English
    REGION: US
    STATE: complete
COMMAND:
  ADMIN:
    NOTMEMBER: '&c%1$s&7 is not a member in your faction.'
    NOTADMIN: '&cYou are not the faction admin.'
    TARGETSELF: '&cThe target player musn''t be yourself.'
    DEMOTES: '&7You have demoted &c%1$s&7 from the position of faction admin.'
    DEMOTED: '&7You have been demoted from the position of faction admin by &c%1$s&7.'
    PROMOTES: '&7You have promoted &c%1$s&7 to the position of faction admin.'
    PROMOTED: '&c%1$s&7 gave &c%2$s&7 the leadership of &c%3$s&7.'
    DESCRIPTION: Hand over your admin rights
  AHOME:
    DESCRIPTION: Send a player to their f home no matter what.
    NOHOME: '&c%1$s&7 doesn''t have an f home.'
    SUCCESS: '&c$1%s&7 was sent to their f home.'
    OFFLINE: '&c%1$s&7 is offline.'
    TARGET: You were sent to your f home.
  ANNOUNCE:
    DESCRIPTION: Announce a message to players in faction.
  AUTOCLAIM:
    ENABLED: '&7Now auto-claiming land for &c%1$s&7.'
    DISABLED: '&7Auto-claiming of land disabled.'
    REQUIREDRANK: '&cYou must be &7%1$s&c to claim land.'
    OTHERFACTION: '&cYou can''t claim land for &7%1$s&c.'
    DESCRIPTION: Auto-claim land as you walk around
  AUTOHELP:
    HELPFOR: '&7Help for command "'
  BOOM:
    PEACEFULONLY: '&cThis command is only usable by factions which are specifically
          designated as peaceful.'
    TOTOGGLE: to toggle explosions
    FORTOGGLE: for toggling explosions
    ENABLED: '&c%1$s&7 has &c%2$s &7explosions in your faction''s territory.'
    DESCRIPTION: Toggle explosions (peaceful factions only)
  BYPASS:
    ENABLE: '&7You have &aenabled&7 admin bypass mode. You will be able to build or destroy
          anywhere.'
    ENABLELOG: ' &7has &aENABLED &7admin bypass mode.'
    DISABLE: '&7You have &cdisabled&7 admin bypass mode.'
    DISABLELOG: ' &7has &cDISABLED&7 admin bypass mode.'
    DESCRIPTION: Enable admin bypass mode
  CHAT:
    DISABLED: '&cThe built in chat channels are disabled on this server.'
    INVALIDMODE: '&cUnrecognised chat mode. &7Please enter either ''a'',''f'' or ''p'''
    DESCRIPTION: Change chat mode
    MODE:
      PUBLIC: '&7Public chat mode.'
      ALLIANCE: '&7Alliance only chat mode.'
      TRUCE: '&7Truce only chat mode.'
      FACTION: '&7Faction only chat mode.'
      MOD: '&7Mod only chat mode.'
  CHATSPY:
    ENABLE: '&7You have enabled chat spying mode.'
    ENABLELOG: ' &7has &aENABLED&7 chat spying mode.'
    DISABLE: '&7You have &cdisabled&7 chat spying mode.'
    DISABLELOG: ' &&has &cDISABLED&7 chat spying mode.'
    DESCRIPTION: Enable admin chat spy mode
  CLAIM:
    INVALIDRADIUS: '&cIf you specify a radius, it must be at least 1.'
    DENIED: '&cYou do not have permission to claim in a radius.'
    DESCRIPTION: Claim land from where you are standing
  CLAIMLINE:
    INVALIDRADIUS: '&cIf you specify a distance, it must be at least 1.'
    DENIED: '&cYou do not have permission to claim in a line.'
    DESCRIPTION: Claim land in a straight line.
    ABOVEMAX: &cThe maximum limit for claim line is &c%s&c.
    NOTVALID: '&7%s&c is not a cardinal direction. You may use &7north&c, &7east&c,
      &7south &cor &7west&c.'
  CONFIG:
    NOEXIST: '&cNo configuration setting "&c%1$s&c" exists.'
    SET:
      'TRUE': '" option set to true (enabled).'
      'FALSE': '" option set to false (disabled).'
      ADDED: '"%1$s" set: "%2$s" added.'
      REMOVED: '"%1$s" set: "%2$s" removed.'
    OPTIONSET: '" option set to '
    COLOURSET: '" color option set to "'
    INTREQUIRED: 'Cannot set "%1$s": An integer (whole number) value required.'
    LONGREQUIRED: 'Cannot set "%1$s": A long integer (whole number) value required.'
    DOUBLEREQUIRED: 'Cannot set "%1$s": A double (numeric) value required.'
    FLOATREQUIRED: 'Cannot set "%1$s": A float (numeric) value required.'
    INVALID:
      COLOUR: 'Cannot set "%1$s": "%2$s" is not a valid color.'
      COLLECTION: '"%1$s" is not a data collection type which can be modified with
        this command.'
      MATERIAL: 'Cannot change "%1$s" set: "%2$s" is not a valid material.'
      TYPESET: '"%1$s" is not a data type set which can be modified with this command.'
    MATERIAL:
      ADDED: '"%1$s" set: Material "%2$s" added.'
      REMOVED: '"%1$s" set: Material "%2$s" removed.'
    LOG: ' (Command was run by %1$s.)'
    ERROR:
      SETTING: '&cError setting configuration setting "&7%1$s" to "&7%2$s".'
      MATCHING: Configuration setting "%1$s" couldn''t be matched, though it should
        be... please report this error.
      TYPE: '''%1$s'' is of type ''%2$s'', which cannot be modified with this command.'
    DESCRIPTION: Change a conf.json setting
  CONVERT:
    BACKEND:
      RUNNING: Already running that backend.
      INVALID: Invalid backend
    DESCRIPTION: Convert the plugin backend
  CREATE:
    MUSTLEAVE: '&cYou must leave your current faction first.'
    INUSE: '&cThat tag is already in use.'
    TOCREATE: to create a new faction
    FORCREATE: for creating a new faction
    ERROR: '&cThere was an internal error while trying to create your faction. Please
          try again.'
    CREATED: '&c%1$s&7 created the new faction &c%2$s&7.'
    YOUSHOULD: '&7You should now: &c%1$s'
    CREATEDLOG: ' created a new faction: '
    DESCRIPTION: Create a new faction
  DEINVITE:
    CANDEINVITE: 'Players you can deinvite: '
    CLICKTODEINVITE: '&7Click to revoke invite for &c%1$s'
    ALREADYMEMBER: '&c%1$s&7 is already a member of &c%2$s'
    MIGHTWANT: '&7You might want to: &c%1$s'
    REVOKED: '&c%1$s&7 revoked your invitation to &c%2$s&7.'
    REVOKES: '&c%1$s&7 revoked &c%2$s''s&7 invitation.'
    DESCRIPTION: Remove a pending invitation
  DELFWARP:
    DELETED: '&7Deleted warp &7%1$s'
    INVALID: '&7Couldn''t find warp &7%1$s'
    TODELETE: to delete warp
    FORDELETE: for deleting warp
    DESCRIPTION: Delete a faction warp
  DESCRIPTION:
    CHANGES: 'You have changed the description for &c%1$s&7 to:'
    CHANGED: '&7The faction %1$s&7 changed their description to:'
    TOCHANGE: to change faction description
    FORCHANGE: for changing faction description
    DESCRIPTION: Change the faction description
  DISBAND:
    IMMUTABLE: '&7You cannot disband the Wilderness, SafeZone, or WarZone.'
    MARKEDPERMANENT: '&7This faction is designated as permanent, so you cannot disband
          it.'
    BROADCAST:
      YOURS: '&c%1$s&7 disbanded your faction.'
      NOTYOURS: '&c%1$s&7 disbanded the faction &c%2$s&7.'
    HOLDINGS: '&7You have been given the disbanded faction''s bank, totaling &c%1$s&7.'
    DESCRIPTION: Disband a faction
  FWARP:
    CLICKTOWARP: '&7Click to warp!'
    COMMANDFORMAT: '&7/f warp <warpname> [password]'
    WARPED: '&7Warped to &c%1$s&7!'
    INVALID:
      PASSWORD: '&cInvalid password!'
    TOWARP: to warp
    FORWARPING: for warping
    WARPS: '&7Warps: '
    DESCRIPTION: Teleport to a faction warp
    PASSWORD:
      REQUIRED: '&cThis faction warp requires a password, use command instead.'
  HELP:
    '404': '&cThis page does not exist'
    NEXTCREATE: '&7Learn how to create a faction on the next page.'
    HOME: '&7And don''t forget to set your home:'
    BANK:
      '1': '&7Your faction has a bank which is used to pay for certain'
      '2': '&7things, so it will need to have money deposited into it.'
      '3': '&7To learn more, use the money command.'
    PLAYERTITLES: '&7Player titles are just for fun. No rules connected to them.'
    OWNERSHIP:
      '1': '&7Claimed land with ownership set is further protected so'
      '2': '&7that only the owner(s), faction admin, and possibly the'
      '3': '&7faction moderators have full access.'
    RELATIONS:
      '1': '&7Set the relation you WISH to have with another faction.'
      '2': '&7Your default relation with other factions will be neutral.'
      '3': '&7If BOTH factions choose "ally" you will be allies.'
      '4': '&7If ONE faction chooses "enemy" you will be enemies.'
      '5': '&7You can never hurt members or allies.'
      '6': '&7You can not hurt neutrals in their own territory.'
      '7': '&7You can always hurt enemies and players without faction.'
      '8': ''
      '9': '&7Damage from enemies is reduced in your own territory.'
      '10': '&7When you die you lose power. It is restored over time.'
      '11': '&7The power of a faction is the sum of all member power.'
      '12': '&7The power of a faction determines how much land it can hold.'
      '13': '&7You can claim land from factions with too little power.'
    PERMISSIONS:
      '1': '&7Only faction members can build and destroy in their own'
      '2': '&7territory. Usage of the following items is also restricted:'
      '3': '&7Door, Chest, Furnace, Dispenser, Diode.'
      '4': ''
      '5': '&7Make sure to put pressure plates in front of doors for your'
      '6': '&7guest visitors. Otherwise they can''t get through. You can'
      '7': '&7also use this to create member only areas.'
      '8': '&7As dispensers are protected, you can create traps without'
      '9': '&7worrying about those arrows getting stolen.'
    ADMIN:
      '1': '&c/f claim safezone &7claim land for the Safe Zone'
      '2': '&c/f claim warzone &7claim land for the War Zone'
      '3': '&c/f autoclaim [safezone|warzone] &7take a guess'
    MOAR:
      '1': 'Finally some commands for the server admins:'
      '2': '&7More commands for server admins:'
      '3': '&7Even more commands for server admins:'
    DESCRIPTION: Display a help page
  HOME:
    DISABLED: '&cSorry, faction homes are disabled on this server.'
    TELEPORTDISABLED: '&cSorry, the ability to teleport to faction homes is disabled
          on this server.'
    NOHOME: '&cYour faction does not have a home.'
    INENEMY: '&cYou cannot teleport to your faction home while in the territory of
          an enemy faction.'
    WRONGWORLD: '&cYou cannot teleport to your faction home while in a different world.'
    ENEMYNEAR: '&cYou cannot teleport to your faction home while an enemy is within
          &7%s &cblocks of you.'
    TOTELEPORT: to teleport to your faction home
    FORTELEPORT: for teleporting to your faction home
    DESCRIPTION: Teleport to the faction home
  INVITE:
    TOINVITE: 'to invite someone'
    FORINVITE: 'for inviting someone'
    CLICKTOJOIN: '&7Click to join!'
    INVITEDYOU: ' &7has invited you to join '
    INVITED: '&c%1$s&7 invited &c%2$s&7 to your faction.'
    ALREADYMEMBER: '&c%1$s&7 is already a member of &c%2$s&7.'
    DESCRIPTION: Invite a player to your faction
    BANNED: '&7%1$s &cis banned from your faction. Not sending an invite.'
  JOIN:
    CANNOTFORCE: '&cYou do not have permission to move other players into a faction.'
    SYSTEMFACTION: '&cPlayers may only join normal factions. This is a system faction.'
    ALREADYMEMBER: '&c%1$s %2$s already a member of %3$s'
    ATLIMIT: '&7The faction &c%1$s&7 is at the limit of &c%2$d members, so &c%3$s&7
      cannot currently join.'
    INOTHERFACTION: '&c%1$s&7 must leave &c%2$s&7 current faction first.'
    NEGATIVEPOWER: '&c%1$s&7 cannot join a faction with a negative power level.'
    REQUIRESINVITATION: '&7This faction requires an invitation.'
    ATTEMPTEDJOIN: '&c%1$s&7 tried to join your faction.'
    TOJOIN: 'to join a faction'
    FORJOIN: 'for joining a faction'
    SUCCESS: '&c%1$s &7successfully joined &c%2$s&7.'
    MOVED: '&7%1$s moved you into the faction &c%2$s&7.'
    JOINED: '&c%1$s&7 joined your faction.'
    JOINEDLOG: '&c%1$s&7 joined the faction &c%2$s&7.'
    MOVEDLOG: '&c%1$s&7 moved the player &c%2$s &7into the faction &c%3$s&7.'
    DESCRIPTION: 'Join a faction'
    BANNED: '&cYou are banned from &7%1$s&c.'
  KICK:
    CANDIDATES: 'Players you can kick: '
    CLICKTOKICK: 'Click to kick '
    SELF: '&cYou cannot kick yourself.'
    NONE: That player is not in a faction.
    NOTMEMBER: '&c%1$s&7 is not a member of &c%2$s&7.'
    INSUFFICIENTRANK: '&cYour rank is too low to kick this player.'
    NEGATIVEPOWER: '&cYou cannot kick that member until their power is positive.'
    TOKICK: to kick someone from the faction
    FORKICK: for kicking someone from the faction
    FACTION: '&c%1$s&7 kicked &c%2$s&7 from the faction!'
    KICKS: '&cYou &7kicked &c%1$s&7 from the faction &c%2$s&7!'
    KICKED: '&c%1$s&7 kicked you from &c%2$s&7!'
    DESCRIPTION: Kick a player from the faction
  LIST:
    FACTIONLIST: '&7Faction List '
    TOLIST: to list the factions
    FORLIST: for listing the factions
    ONLINEFACTIONLESS: '&7Online factionless: '
    DESCRIPTION: See a list of the factions
  LOCK:
    LOCKED: '&7Factions is now locked.'
    UNLOCKED: '&7Factions is now unlocked.'
    DESCRIPTION: Lock all write stuff. Apparently.
  LOGINS:
    TOGGLE: '&7Set login / logout notifications for faction members to: &c%s'
    DESCRIPTION: Toggle(?) login / logout notifications for Faction members
  MAP:
    TOSHOW: to show the map
    FORSHOW: for showing the map
    UPDATE:
      ENABLED: '&7Map auto update &aENABLED&7.'
      DISABLED: '&7Map auto update &cDISABLED&7.'
    DESCRIPTION: Show the territory map, and set optional auto update
  MAPHEIGHT:
    DESCRIPTION: '&7Update the lines that /f map sends'
    SET: '&7Set /f map lines to &c%1$d'
    CURRENT: '&7Current mapheight: &c%1$d'
  MOD:
    CANDIDATES: 'Players you can promote: '
    CLICKTOPROMOTE: 'Click to promote '
    NOTMEMBER: '%1$s&c is not a member in your faction.'
    NOTADMIN: '&cYou are not the faction admin.'
    SELF: '&cThe target player musn''t be yourself.'
    TARGETISADMIN: '&cThe target player is a faction admin. Demote them first.'
    REVOKES: '&7You have removed moderator status from &c%1$s&7.'
    REVOKED: '&c%1$s&7 is no longer moderator in your faction.'
    PROMOTES: '&c%1$s&7 was promoted to moderator in your faction.'
    PROMOTED: '&7You have promoted &c%1$s&7 to moderator.'
    DESCRIPTION: Give or revoke moderator rights
  MODIFYPOWER:
    ADDED: '&7Added &c%1$f &7power to &c%2$s&7. &7New total rounded power: &c%3$d'
    DESCRIPTION: Modify the power of a faction/player
  MONEY:
    LONG: '&7The faction money commands.'
    DESCRIPTION: Faction money commands
  MONEYBALANCE:
    SHORT: show faction balance
    DESCRIPTION: Show your factions current money balance
  MONEYDEPOSIT:
    DESCRIPTION: Deposit money
    DEPOSITED: '&c%1$s&7 deposited &c%2$s&7 in the faction bank: &c%3$s'
  MONEYTRANSFERFF:
    DESCRIPTION: Transfer f -> f
    TRANSFER: '&c%1$s &7transferred &c%2$s&7 from the faction "&c%3$s&7" to the faction "&c%4$s&7"'
  MONEYTRANSFERFP:
    DESCRIPTION: Transfer f -> p
    TRANSFER: '&c%1$s &7transferred &c%2$s&7 from the faction "&c%3$s&7" to the player "&c%4$s&7"'
  MONEYTRANSFERPF:
    DESCRIPTION: Transfer p -> f
    TRANSFER: '&c%1$s &7transferred &c%2$s&7 &7from the player "&c%3$s&7" to the faction "&c%4$s&7"'
  MONEYWITHDRAW:
    DESCRIPTION: Withdraw money
    WITHDRAW: '&c%1$s &7withdrew &c%2$s&7 from the faction bank: &c%3$s'
  OPEN:
    TOOPEN: to open or close the faction
    FOROPEN: for opening or closing the faction
    OPEN: open
    CLOSED: closed
    CHANGES: '%1$s&7 changed the faction to &c%2$s&7.'
    CHANGED: '&7The faction &c%1$s&7 is now &c%2$s&7.'
    DESCRIPTION: Switch if an invitation is required to join
  OWNER:
    DISABLED: '&cSorry, but owned areas are disabled on this server.'
    LIMIT: '&cSorry, but you have reached the server''s &climit of %1$d &cowned areas
          per faction.'
    WRONGFACTION: '&cThis land is not claimed by your faction, so you can''t set ownership
          of it.'
    NOTCLAIMED: '&cThis land is not claimed by a faction. Ownership is not possible.'
    NOTMEMBER: '&c%1$s&7 is not a member of this faction.'
    CLEARED: '&7You have cleared ownership for this claimed area.'
    REMOVED: '&7You have removed ownership of this claimed land from %1$s&7.'
    TOSET: to set ownership of claimed land
    FORSET: for setting ownership of claimed land
    ADDED: '&7You have added %1$s&7 to the owner list for this claimed land.'
    DESCRIPTION: Set ownership of claimed land
  OWNERLIST:
    DISABLED: '&cSorry, but owned areas are disabled on this server.'
    WRONGFACTION: '&cThis land is not claimed by your faction.'
    NOTCLAIMED: '&7This land is not claimed by any faction, thus no owners.'
    NONE: '&7No owners are set here; everyone in the faction has access.'
    OWNERS: '&7Current owner(s) of this land: &c%1$s'
    DESCRIPTION: List owner(s) of this claimed land
  PEACEFUL:
    DESCRIPTION: Set a faction to peaceful
    YOURS: '&c%1$s&7 has &c%2$s &7your faction'
    OTHER: '&c%s&7 has &c%s &7the faction ''&c%s&7''.'
    GRANT: granted peaceful status to
    REVOKE: removed peaceful status from
  PERM:
    DESCRIPTION: '&7Edit or list your faction''s permissions.'
    INVALID:
      RELATION: '&cInvalid relation defined. Try something like ''ally'''
      ACCESS: '&cInvalid access defined. Try something like ''allow'''
      ACTION: '&cInvalid action defined. Try something like ''build'''
    SET: '&7Set permission &c%1$s &7to &c%2$s &7for relation &c%3$s&7.'
    TOP: RCT MEM OFF ALLY TRUCE NEUT ENEMY
  PERMANENT:
    DESCRIPTION: Toggles a faction's permanence
    GRANT: added permanent status to
    REVOKE: removed permanent status from
    YOURS: '&c%1$s&7 has &c%2$s&7 your faction'
    OTHER: '&c%s&7 has &c%s&7 the faction ''%s&7''.'
  PROMOTE:
    TARGET: 'You''ve been &c%1$s &7to &c%2$s&7.'
    SUCCESS: '&7You successfully &c%1$s %2$s &7to &c%3$s&7.'
    PROMOTED: promoted
    DEMOTED: demoted
    DESCRIPTION: /f promote <name>
    WRONGFACTION: '&c%1$s&7 is not part of your faction.'
    NOTTHATPLAYER: '&cThat player cannot be promoted.'
  PERMANENTPOWER:
    DESCRIPTION: Toggle faction power permanence
    GRANT: added permanentpower status to
    REVOKE: removed permanentpower status from
    SUCCESS: '&7You %s &c%s&7.'
    FACTION: '&c%s&7 %s your faction'
  NOACCESS: '&cYou don''t have access to that.'
  POWER:
    TOSHOW: to show player power info
    FORSHOW: for showing player power info
    POWER: '&e%1$s&7 - Power &l/ &7Maxpower: &c%2$d &l/ &c%3$d %4$s'
    BONUS: ' (bonus: '
    PENALTY: ' (penalty: '
    DESCRIPTION: Show player power info
  POWERBOOST:
    HELP:
      '1': '&cYou must specify "p" or "player" to target a player or "f" or "faction"
              to target a faction.'
      '2': '&cex. /f powerboost p SomePlayer 0.5  -or-  /f powerboost f SomeFaction
              -5'
    INVALIDNUM: '&cYou must specify a valid numeric value for the power bonus/penalty
          amount.'
    PLAYER: Player "%1$s"
    FACTION: Faction "%1$s"
    BOOST: '&7%1$s now has a power bonus/penalty of &c%2$d&7 to min and max power levels.'
    BOOSTLOG: '%1$s has set the power bonus/penalty for &c%2$s&7 to &c%3$d.'
    DESCRIPTION: Apply permanent power bonus/penalty to specified player or faction
  RELATIONS:
    ALLTHENOPE: '&cNope! You can''t.'
    MORENOPE: '&cNope! You can''t declare a relation to yourself.'
    ALREADYINRELATIONSHIP: '&cYou already have that relation wish set with %1$s.'
    TOMARRY: to change a relation wish
    FORMARRY: for changing a relation wish
    MUTUAL: '&7Your faction is now &c%1$s&7 to &c%2$s'
    PEACEFUL: '&7This will have no effect while your faction is peaceful.'
    PEACEFULOTHER: '&7This will have no effect while their faction is peaceful.'
    DESCRIPTION: Set relation wish to another faction
    EXCEEDS:
      ME: '&7Failed to set relation wish. You can only have &c%1$s %2$s&7.'
      THEY: '&7Failed to set relation wish. They can only have &c%1$s %2$s&7.'
    PROPOSAL:
      '1': '%1$s&7 wishes to be your %2$s'
      '2': '&7Type &c/%1$s %2$s %3$s&7 to accept.'
      SENT: '&c%1$s&7 were informed that you wish to be &c%2$s&7.'
  RELOAD:
    TIME: '&7Reloaded &call configuration files &7from disk, took &c%1$d ms&7.'
    DESCRIPTION: Reload data file(s) from disk
  SAFEUNCLAIMALL:
    DESCRIPTION: Unclaim all safezone land
    UNCLAIMED: '&7You unclaimed ALL safe zone land.'
    UNCLAIMEDLOG: '&c%1$s &7unclaimed all safe zones.'
  SAVEALL:
    SUCCESS: '&7Factions saved to disk!'
    DESCRIPTION: Save all data to disk
  SCOREBOARD:
    DESCRIPTION: Scoreboardy things
  SETDEFAULTROLE:
    DESCRIPTION: /f defaultrole <role> - set your faction's default role.
    NOTTHATROLE: You cannot set the default to admin.
    SUCCESS: 'Set default role of your faction to &c%1$s&7.'
    INVALIDROLE: '&cCouldn''t find matching role for &7%1$s.'
  SETFWARP:
    NOTCLAIMED: '&7You can only set warps in your faction territory.'
    LIMIT: '&7Your Faction already has the max amount of warps set &c(%1$d)&7.'
    SET: '&7Set warp &7%1$s and password &c''%2$s'' &7to your location.'
    TOSET: to set warp
    FORSET: for setting warp
    DESCRIPTION: Set a faction warp
  SETHOME:
    DISABLED: '&cSorry, Faction homes are disabled on this server.'
    NOTCLAIMED: '&cSorry, your faction home can only be set inside your own claimed
          territory.'
    TOSET: to set the faction home
    FORSET: for setting the faction home
    SET: '&c%1$s&7 set the home for your faction. You can now use:'
    SETOTHER: '&cYou have set the home for the %1$s&7 faction.'
    DESCRIPTION: Set the faction home
  SETMAXVAULTS:
    DESCRIPTION: Set max vaults for a Faction.
    SUCCESS: '&7Set max vaults for &c%s &7to &c%d'
  VAULT:
    DESCRIPTION: /f vault <number> to open one of your faction's vaults.
    TOOHIGH: '&cYou tried to open vault &7%d &cbut your faction only has &7%d&c vaults.'
  SHOW:
    NOFACTION:
      SELF: '&cYou are not in a faction'
      OTHER: '&cThat''s not a faction'
    TOSHOW: to show faction information
    FORSHOW: for showing faction information
    DESCRIPTION: '&7Description: &7%1$s'
    PEACEFUL: 'This faction is Peaceful'
    PERMANENT: '&7This faction is permanent, remaining even with no members.'
    JOINING: '&7Joining: &7%1$s '
    INVITATION: '&cAn invitation is required.'
    UNINVITED: '&cNo invitation is needed.'
    NOHOME: n/a
    POWER: '&7Land / Power / Maxpower: &7 %1$d/%2$d/%3$d %4$s.'
    BONUS: ' (bonus: '
    PENALTY: ' (penalty: '
    DEPRECIATED: (%1$s depreciated)
    LANDVALUE: '&7Total land value: &7%1$s %2$s'
    BANKCONTAINS: '&7Bank contains: &7%1$s'
    ALLIES: 'Allies: '
    ENEMIES: 'Enemies: '
    MEMBERSONLINE: 'Members online: '
    MEMBERSOFFLINE: 'Members offline: '
    COMMANDDESCRIPTION: Show faction information
    DEATHS:
      TIL:
        RAIDABLE: '&7DTR: %1$d'
    EXEMPT: '&cThis faction is exempt and cannot be seen.'
  SHOWINVITES:
    PENDING: 'Players with pending invites: '
    CLICKTOREVOKE: '&7Click to revoke invite for &c%1$s'
    DESCRIPTION: Show pending faction invites
  STATUS:
    FORMAT: '&c%1$s &7Power: &c%2$s &7Last Seen: &c%3$s'
    ONLINE: Online
    AGOSUFFIX: ' ago.'
    DESCRIPTION: Show the status of a player
  STUCK:
    TIMEFORMAT: m 'minutes', s 'seconds.'
    CANCELLED: '&7Teleport cancelled because you were damaged'
    OUTSIDE: '&7Teleport cancelled because you left &c%1$d &7block radius.'
    EXISTS: '&7You are already teleporting, you must wait &7%1$s'
    START: '&7Teleport will commence in &7%s&7. Don''t take or deal damage. '
    TELEPORT: '&7Teleported safely to %1$d, %2$d, %3$d.'
    TOSTUCK: to safely teleport %1$s out
    FORSTUCK: for %1$s initiating a safe teleport out
    DESCRIPTION: Safely teleports you out of enemy faction
  TAG:
    TAKEN: '&cThat tag is already taken.'
    TOCHANGE: to change the faction tag
    FORCHANGE: for changing the faction tag
    FACTION: '%1$s&7 changed your faction tag to %2$s'
    CHANGED: '&7The faction &c%1$s&7 changed their name to &c%2$s&7.'
    DESCRIPTION: Change the faction tag
  TITLE:
    TOCHANGE: to change a players title
    FORCHANGE: for changing a players title
    CHANGED: '&c%1$s&7 changed a title: &c%2$s'
    DESCRIPTION: Set or remove a players title
  TOGGLEALLIANCECHAT:
    DESCRIPTION: Toggles whether or not you will see alliance chat
    IGNORE: '&cAlliance chat is now ignored.'
    UNIGNORE: '&7Alliance chat is no longer ignored.'
  TOGGLESB:
    DISABLED: '&cYou can''t toggle scoreboards while they are disabled.'
  TOP:
    DESCRIPTION: 'Sort Factions to see the top of some criteria.'
    TOP: '&7Top Factions by &c%s&7. Page &c%d/%d'
    LINE: '%d. &6%s: &c%s'
    INVALID: '&cCould not sort by &7%s&c. Try balance, online, members, power or land.'
  UNCLAIM:
    SAFEZONE:
      SUCCESS: '&7Safe zone was unclaimed.'
      NOPERM: '&cThis is a safe zone. You lack permissions to unclaim.'
    WARZONE:
      SUCCESS: '&7War zone was unclaimed.'
      NOPERM: '&cThis is a war zone. You lack permissions to unclaim.'
    UNCLAIMED: '%1$s&7 unclaimed some of your land.'
    UNCLAIMS: '&7You unclaimed this land.'
    LOG: '%1$s unclaimed land at (%2$s) from the faction: %3$s'
    WRONGFACTION: '&cYou don''t own this land.'
    TOUNCLAIM: to unclaim this land
    FORUNCLAIM: for unclaiming this land
    FACTIONUNCLAIMED: '%1$s&7 unclaimed some land.'
    DESCRIPTION: Unclaim the land where you are standing
  UNCLAIMALL:
    TOUNCLAIM: to unclaim all faction land
    FORUNCLAIM: for unclaiming all faction land
    UNCLAIMED: '%1$s&7 unclaimed ALL of your faction''s land.'
    LOG: '%1$s unclaimed everything for the faction: %2$s'
    DESCRIPTION: Unclaim all of your factions land
  VERSION:
    VERSION: '&7You are running %1$s'
    DESCRIPTION: Show plugin and translation version information
  WARUNCLAIMALL:
    DESCRIPTION: Unclaim all warzone land
    SUCCESS: '&7You unclaimed ALL war zone land.'
    LOG: '%1$s unclaimed all war zones.'
  BAN:
    DESCRIPTION: 'Ban players from joining your Faction.'
    TARGET: '&cYou were banned from &7%1$s.'
    BANNED: '&c%1$s &7banned &c%2$s.'
    SELF: '&cYou may not ban yourself.'
    INSUFFICIENTRANK: '&cYour rank is too low to ban &7%1$s'
  BANLIST:
    DESCRIPTION: View a faction's ban list
    HEADER: '&6There are &c%d&6 bans for %s'
    ENTRY: '&7%d. &c%s &r- &a%s &r- &e%s'
    NOFACTION: '&4You are not in a Faction.'
  FLY:
    DISABLED: '&cSorry, Faction flight is disabled on this server.'
    DESCRIPTION: 'Enter or leave Faction flight mode'
    CHANGE: '&7Faction flight &c%1$s.'
    DAMAGE: '&7Faction flight &cdisabled&7 due to entering combat.'
    'NO':
      ACCESS: '&cCannot fly in territory of &7%1$s&c.'
  UNBAN:
    DESCRIPTION: 'Unban someone from your Faction'
    NOTBANNED: '&7%s &cisn''t banned. Not doing anything.'
    UNBANNED: '&c%1$s &7unbanned &c%2$s'
    TARGET: '&7You were unbanned from &c%s'
command:
  help:
    invitations: '&7You might want to close it and use invitations:'
LEAVE:
  PASSADMIN: '&cYou must give the admin role to someone else first.'
  NEGATIVEPOWER: '&cYou cannot leave until your power is positive.'
  TOLEAVE: to leave your faction.
  FORLEAVE: for leaving your faction.
  LEFT: '&7%s&c left faction &7%s&c.'
  DISBANDED: '&7%s&c was disbanded.'
  DISBANDEDLOG: 'The faction %s (%s) was disbanded due to the last player (%s) leaving.'
  DESCRIPTION: Leave your faction
CLAIM:
  PROTECTED: '&cThis land is protected.'
  DISABLED: '&cSorry, this world has land claiming disabled.'
  CANTCLAIM: '&cYou can''t claim land for &c%s&c.'
  ALREADYOWN: '%s&7 already own this land.'
  MUSTBE: '&7You must be &c%s&7 to claim land.'
  MEMBERS: '&7Factions must have at least &c%s&7 members to claim land.'
  SAFEZONE: '&cYou can not claim a Safe Zone.'
  WARZONE: '&cYou can not claim a War Zone.'
  POWER: '&cYou can''t claim more land! You need more power!'
  LIMIT: '&cLimit reached. You can''t claim more land!'
  ALLY: '&cYou can''t claim the land of your allies.'
  CONTIGIOUS: '&cYou can only claim additional land which is connected to your first
      claim or controlled by another faction!'
  FACTIONCONTIGUOUS: '&cYou can only claim additional land which is connected to your
      first claim!'
  PEACEFUL: '%s&7 owns this land. Your faction is peaceful, so you cannot claim land
    from other factions.'
  PEACEFULTARGET: '%s&7 owns this land, and is a peaceful faction. You cannot claim
    land from them.'
  THISISSPARTA: '%s&7 owns this land and is strong enough to keep it.'
  BORDER: '&cYou must start claiming land at the border of the territory.'
  TOCLAIM: to claim this land
  FORCLAIM: for claiming this land
  TOOVERCLAIM: to overclaim this land
  FOROVERCLAIM: for over claiming this land
  CLAIMED: '&c%s&7 claimed land for &c%s&7 from &c%s&7.'
  CLAIMEDLOG: '%s claimed land at (%s) for the faction: %s'
  OVERCLAIM:
    DISABLED: '&7Over claiming is disabled on this server.'
  TOOCLOSETOOTHERFACTION: '&7Your claim is too close to another Faction. Buffer required
      is %d'
  OUTSIDEWORLDBORDER: '&7Your claim is outside the border.'
  OUTSIDEBORDERBUFFER: '&7Your claim is outside the border. %d chunks away world edge
    required.'
  CLICK:
    TO:
      CLAIM: 'Click to try to claim &2(%1$d, %2$d)'
  YOUAREHERE: You are here
GENERIC:
  YOU: You
  YOURFACTION: your faction
  NOPERMISSION: '&cYou don''t have permission to %1$s.'
  DOTHAT: do that
  NOPLAYERMATCH: '&cNo player match found for "&7%1$s&c".'
  NOPLAYERFOUND: '&cNo player "&7%1$s&c" could not be found.'
  ARGS:
    TOOFEW: '&cToo few arguments. &7Use like this:'
    TOOMANY: '&cStrange argument "&7%1$s&c". &7Use the command like this:'
  DEFAULTDESCRIPTION: 'To set your description, do /f desc.'
  OWNERS: 'Owner(s): %1$s'
  PUBLICLAND: Public faction land.
  FACTIONLESS: factionless
  SERVERADMIN: A server admin
  DISABLED: disabled
  ENABLED: enabled
  INFINITY: âˆž
  CONSOLEONLY: 'This command cannot be run as a player.'
  PLAYERONLY: '&cThis command can only be used by ingame players.'
  ASKYOURLEADER: '&7 Ask your leader to:'
  YOUSHOULD: '&7You should:'
  YOUMAYWANT: '&7You may want to: '
  TRANSLATION:
    VERSION: 'Translation: %1$s(%2$s,%3$s) State: %4$s'
    CONTRIBUTORS: 'Translation contributors: %1$s'
    RESPONSIBLE: 'Responsible for translation: %1$s'
  FACTIONTAG:
    TOOSHORT: '&7The faction tag can''t be shorter than &c%1$s&7 chars.'
    TOOLONG: '&7The faction tag can''t be longer than &c%s&7 chars.'
    ALPHANUMERIC: '&7Faction tag must be alphanumeric. "&c%s&7" is not allowed.'
  PLACEHOLDER: '<This is a placeholder for a message you should not see>'
COMPASS:
  SHORT:
    NORTH: '&lN'
    EAST: '&lE'
    SOUTH: '&lS'
    WEST: '&lW'
CHAT:
  FACTION: faction chat
  ALLIANCE: alliance chat
  TRUCE: truce chat
  PUBLIC: public chat
  MOD: mod chat
ECON:
  'OFF': no %s
  FORMAT: '###,###.###'
RELATION:
  MEMBER:
    SINGULAR: member
    PLURAL: members
  ALLY:
    SINGULAR: ally
    PLURAL: allies
  TRUCE:
    SINGULAR: truce
    PLURAL: truces
  NEUTRAL:
    SINGULAR: neutral
    PLURAL: neutrals
  ENEMY:
    SINGULAR: enemy
    PLURAL: enemies
ROLE:
  ADMIN: admin
  MODERATOR: moderator
  NORMAL: normal member
  RECRUIT: recruit
REGION:
  SAFEZONE: safezone
  WARZONE: warzone
  WILDERNESS: wilderness
  PEACEFUL: peaceful territory
PLAYER:
  CANTHURT: '&7You may not harm other players in %s'
  SAFEAUTO: '&7This land is now a safe zone.'
  WARAUTO: '&7This land is now a war zone.'
  OUCH: '&cOuch, that is starting to hurt. You should give it a rest.'
  USE:
    WILDERNESS: '&cYou can''t use &c%s&c in the wilderness.'
    SAFEZONE: '&cYou can''t use &c%s&c in a safe zone.'
    WARZONE: '&cYou can''t use &c%s&c in a war zone.'
    TERRITORY: '&cYou can''t &c%s&c in the territory of &c%s&c.'
    OWNED: '&cYou can''t use &c%s&c in this territory, it is owned by: %s&c.'
  COMMAND:
    WARZONE: '&cYou can''t use the command ''%s'' in warzone.'
    NEUTRAL: '&cYou can''t use the command ''%s'' in neutral territory.'
    ENEMY: '&cYou can''t use the command ''%s'' in enemy territory.'
    PERMANENT: '&cYou can''t use the command ''%s'' because you are in a permanent faction.'
    ALLY: '&cYou can''t use the command ''%s'' in ally territory.'
    WILDERNESS: '&cYou can''t use the command ''%s'' in the wilderness.'
  POWER:
    NOLOSS:
      PEACEFUL: '&7You didn''t lose any power since you are in a peaceful faction.'
      WORLD: '&7You didn''t lose any power due to the world you died in.'
      WILDERNESS: '&7You didn''t lose any power since you were in the wilderness.'
      WARZONE: '&7You didn''t lose any power since you were in a war zone.'
    LOSS:
      WARZONE: |-
        '&cThe world you are in has power loss normally disabled, but you still lost power since you were in a war zone.'
        '&7Your power is now &c%d / %d'
    NOW: '&7Your power is now &c%d / %d'
  PVP:
    LOGIN: '&7You can''t hurt other players for %d seconds after logging in.'
    REQUIREFACTION: '&7You can''t hurt other players until you join a faction.'
    FACTIONLESS: '&7You can''t hurt players who are not currently in a faction.'
    PEACEFUL: '&7Peaceful players cannot participate in combat.'
    NEUTRAL: '&7You can''t hurt neutral factions. Declare them as an enemy.'
    CANTHURT: '&7You can''t hurt %s&7.'
    NEUTRALFAIL: '&7You can''t hurt %s&7 in their own territory unless you declare
      them as an enemy.'
    TRIED: '%s&7 tried to hurt you.'
NOPAGES: '&7Sorry. No Pages available.'
INVALIDPAGE: '&7Invalid page. Must be between 1 and %1$d'
title: '&bFactions &0|&r'
wilderness: '&2Wilderness'
wilderness-description: ''
warzone: '&4Warzone'
warzone-description: 'Not the safest place to be.'
safezone: '&6Safezone'
safezone-description: 'Free from pvp and monsters.'
toggle-sb: 'You now have scoreboards set to {value}'
faction-leave: '&7Leaving %1$s, &7Entering %2$s'
faction-announcement-top: '&d--Unread Faction Announcements--'
faction-announcement-bottom: '&d--Unread Faction Announcements--'
default-prefix: '{relationcolor}[{faction}] &r'
faction-login: '&e%1$s &9logged in.'
faction-logout: '&e%1$s &9logged out.'
nofactions-prefix: '&7-&r'
date-format: MM/d/yy h:ma
raidable-true: 'true'
raidable-false: 'false'
WARMUPS:
  NOTIFY:
    TELEPORT: '&eYou will teleport to &d%1$s &ein &d%2$d &eseconds.'
    FLIGHT: '&eFlight will enable in &d%2$d &eseconds.'
  ALREADY: '&cYou are already warming up.'
  CANCELLED: '&cYou have cancelled your warmup.'
```

**NOTE:** In a recent update, the `lang.yml` has been changed to color codes and not <> variables. This is a template, not the official file.