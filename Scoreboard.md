## Enabling the scoreboard
In the config.yml, go to the `scoreboard` section. In there, there will be two parts: f-info and the default scoreboard. The f-info variable is when you walk into a faction's territory, it will show you information about that faction. To enable it, set `finfo-enabled:` to `true`.

```yaml
  finfo-enabled: false
```

The other variable is the default scoreboard. This is constantly there, unlike f-info. To enable it, change `default-enabled:` to `true`.

```yaml
  default-enabled: false
```

## Configuring the scoreboards
To set the expiration for the f-info scoreboard, change it to whatever number you want.

```yaml
 scoreboard:
  also-send-chat: true
  expiration: 7
```

To change what f-info says, change each line in the quotation marks to what you want. Accepts color codes.

```yaml
  finfo:
    - "&6Power"
    - "{power}"
    - "&3Members"
    - "{online}/{members}"
    - "&4Leader"
    - "{leader}"
    - "&bTerritory"
    - "{chunks}"
```

To show faction relations and faction names in the tablist, set `default-prefixes:` to `true`. The scoreboard must be enabled for it to work. To change the title and format of the default scoreboard, change what's inside the quotation marks to whatever you want in it. Placeholders do not work in the title. Accepts color codes.

```yaml
default-prefixes: false
default-title: "i love drt"
default-update-interval: 1
  default:
    - "&cFaction"
    - "&7{faction}"
    - "&3Your Power"
    - "{power}"
    - "&aBalance"
    - "${balance}"
```

The variable below it, `factionless`, only shows if you do not have a faction and when you set `factionless-enabled` to `true`. Configure this to what you want to show them. Accepts color codes.

```yaml
  factionless-enabled: false
  factionless:
    - "Make a new Faction"
    - "Use /f create"
```

Scoreboards support internal and third-party ([PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) and [MVdW](https://www.spigotmc.org/resources/mvdwplaceholderapi.11182/)) placeholders.

**NOTE:** Restarting will create the scoreboard, /f reload will not.