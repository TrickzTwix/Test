## Enabling the scoreboard
In the config.yml, go to the `scoreboard` section. In there, there will be two parts: f-info and the default scoreboard. The f-info variable is when you walk into a faction's territory, it will show you information about that faction. To enable it, set `finfo-enabled:` to `true`.

The other variable is the default scoreboard. This will constantly show. To enable it, change `default-enabled:` to `true`

## Configuring the scoreboards
The f-info scoreboard has an option to expire after a certain amount of time. You can set how long it stays when entering in the `expiration` section.

To show faction relations and faction names in the tablist, enable `default-prefixes`. The scoreboard must be enabled for it to work. To change the title of the scoreboard, add your title to `default-title`. The variable below it, `factionless-enabled`, only shows if you do not have a faction and when it's enabled. Configure this to what you want to show them.

Both of these sections support internal and third-party ([PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) and [MVdW](https://www.spigotmc.org/resources/mvdwplaceholderapi.11182/)) placeholders.

**NOTE:** it may take time to update, so restart it once you're done configuring it and wait patiently.