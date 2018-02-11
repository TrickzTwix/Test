All commands in alphabetical order.

Command | Permission | Usage
--- | --- | ---
/f admin <target> |	factions.admin |	Set new player as leader of your faction.
/f ahome <target> |	factions.ahome |	Teleport to a player's faction's home
/f announce <message…>	| factions.announce |	Send a message to players in your faction
/f autoclaim [faction] |	factions.autoclaim |	Auto-claim land when you walk over wilderness for your faction. Admins can specify other factions and claim for them.
/f autohelp |	none |	Show help for all commands.
/f boom [on/off] |	factions.noboom	| Toggle peaceful explosions in your faction's territory on or off.
/f bypass |	factions.bypass | Set yourself to bypass Faction permission checks
/f chat <mode>	| factions.chat	| Toggle chat modes. Or specify which channel you want to be in (public, alliance, faction, truce)
/f chatspy |	factions.chatspy |	Enable spying on all private chat channels
/f claim [radius] [faction] |	factions.claim	| Claim land for your faction given an optional radius. Admins can specify other factions.
/f claimline <chunks> [direction] [faction] |	factions.claimline |	Claim land in a line for your Faction given an optional length and direction. Admins can specify other factions.
/f config <setting> <value> |	factions.config |	Set configuration values in the conf.json
/f convert <backend> |	console only |	Convert from your current backend to a new backend (JSON). New backends will be added in the future (MYSQL)
/f create <tag> |	factions.create |	Create a Faction with the given tag
/f defaultrole <role> | factions.defaultrank | Set the default rank new members get when joining your Faction
/f deinvite [name] |	factions.deinvite |	Revoke an invite from a player. If no player defined, lists all players with pending invites with click to revoke.
/f delwarp <name> |	factions.setwarp |	Delete a warp
/f demote <name> |	factions.promote |	Demote a player 1 rank
/f desc <description…> |	factions.description |	Set your faction's new description
/f disband |	factions.disband |	Disband your faction
/f warp [warp] [password] |	factions.warp |	Go to a Faction warp. Specify password if needed.
/f help <page> |	factions.help |	List help pages for things
/f home |	factions.home |	Go to your faction's home
/f invite <target> |	factions.invite |	Invite a player to your faction
/f join <faction> |	factions.join |	Join a defined Faction
/f kick <target> |	factions.kick |	Kick a player from your faction
/f leave	| factions.leave	| Leave your faction
/f list	| factions.list |	List top Factions by players
/f lock	| factions.lock |	Lock datafiles from being overwritten. Will make anything on the server not get saved.
/f logins |	factions.monitorlogins |	Toggle monitoring of logins for your Faction
/f map [on/off]	| factions.map |	View the Faction map of your area
/f mapheight [value] | factions.mapheight | Set how many lines your /f map will show
/f mod [name] |	factions.mod |	Promote a player in your Faction to mod
/f modifypower <name> <power>	| factions.modifypower	| Modify a player's power. Adds <power> to the player's current power.
/f money |	none |	Show help for money commands
/f money balance [faction] |	factions.money.balance	| Check a faction's balance. Defaults to your own faction.
/f money deposit <amount> [faction] |	factions.money.deposit |	Deposit money into your faction. Admins can specify other factions.
/f money ff <amount> <factionfrom> <factionto>	| factions.money.f2f |	Transfer money from one faction to another
/f money fp <amount> <factionfrom> <playerto> |	factions.money.f2p |	Transfer money from one faction to a player
/f money pf <amount> <playerfrom> <factionto> |	factions.money.pf2 |	Transfer money from one player to a faction
/f money withdraw <amount> [faction] |	factions.money.withdraw |	Withdraw money from your faction. Admins can specify any faction.
/f open	| factions.open |	Toggle allowing anyone being able to join the faction
/f owner [name]	| factions.owner |	Set claim ownership for this chunk. Admins can specify a target player.
/f ownerlist |	factions.ownerlist |	Get the current owner of the chunk you're in if it's your faction
/f peaceful <faction> |	factions.peaceful |	Set a Faction to being peaceful
/f perm [relation] [action] [access] |	factions.permissions |	Manage permissions for your Faction. Example /f perm recruit build deny
/f permanent <faction> |	factions.permanent |	Set a Faction to permanent status. This will make the Faction say if there are 0 members.
/f permanentpower <faction> [power] |	factions.setpermanentpower |	Set permanent power to a Faction
/f power <player> |	factions.power |	Check power of a player. Defaults to yourself.
/f powerboost <player/faction> <name> <number>	| factions.powerboost |	Set powerboost of a player or Faction. <player/faction> can be 'f' or 'p' to let us know if you're specifying a player or Faction.
/f promote <name> |	factions.promote |	Promote a player in your Faction one rank. Will not let you promote them to admin / owner.
/f rel <relation> <faction> |	factions.relation	| Request to change your Faction's relationship with a target Faction. Relations can be ally, truce, neutral, enemy.
/f reload |	factions.reload |	Reload configurations (lang.yml, config.yml, conf.json). This does not reload factions saved data from disk.
/f safeunclaimall [world] |	factions.managesafezone	| Safely unclaim all territories in your world. Can specify another world.
/f saveall	| factions.save	| Force save all Factions data to disk
/f sb	| factions.scoreboard |	Toggle the Factions scoreboard on or off
/f sc |	factions.seechunk	| See outlines around the border of the chunk you're standing in. No one else can see the outlines.
/f defaultrole <role> |	factions.defaultrank |	Set the default role that new members will get when they join your Faction
/f setwarp <name> [password] |	factions.setwarp |	Set a warp with an optional password to your location
/f sethome	| factions.sethome |	Set your faction's home
/f setmaxvaults <faction> <number> |	factions.setmaxvaults	| Set the max vaults a Faction can have
/f show [faction] |	factions.show |	Show info about a Faction. Defaults to yours.
/f showinvites |	factions.showinvites |	Show pending invites for your Faction
/f status |	factions.status	| Show status of all players in your Faction
/f stuck	| factions.stuck	| Attempts to teleport you to the nearest wilderness chunk
/f tag <tag>	| factions.tag	| Change your faction's tag
/f title <player> [title] |	factions.title	| Set a player's custom title. Will charge them if enabled.
/f togglealliancechat |	factions.togglealliancechat	| Toggle ignoring alliance chat
/f top <criteria> [page] |	factions.top	| List top factions by criteria (members, start, power, land, online, money)
/f unclaim [radius] [faction] |	factions.unclaim	| Unclaim for your faction. Optionally define the radius. Admins can specify other factions.
/f unclaimall |	factions.unclaimall |	Unclaim all of your faction's land.
/f vault [number] |	factions.vault |	Open your faction's vault. If no vault is defined, it will list available vaults.
/f version |	factions.version	| Show the version string for FactionsUUID
/f warunclaimall	| factions.managewarzone |	Unclaim all warzone