## Enabling the scoreboard
You might've tried doing /f sb and it saying "The scoreboard is not enabled!", well here's a guide to help you with that.

In the config.yml, go to the `Scoreboard` section. In there, there will be two parts: F-info and the default scoreboard. The f-info variable is when you walk into a faction's territory, it will show you information about that faction. To enable it, set `finfo-enabled:` to `true`.

The other variable is the default scoreboard. This will constantly show. To enable it, change `default-enabled:` to `true`

## Configuring the scoreboards
The f-info scoreboard has an option to expire after a certain amount of time. You can set how long it stays when entering in the `expiration` section.

The default scoreboard has an option to enable `default-prefixes`, which in turn changes the tablist showing your faction and relation to that faction. The scoreboard must be enabled for it to work. You can also change the title of the scoreboard in the variable `default-title`. The variable below it, `factionless-enabled` only shows if you do not have a faction.

Both of these sections support internal and third-party ([PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) and [MVdW](https://www.spigotmc.org/resources/mvdwplaceholderapi.11182/)) placeholders.

**NOTE:** it may take time to update, so restart it once you're done configuring it and wait patiently.