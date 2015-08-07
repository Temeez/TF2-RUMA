# TF2-RUMA
TF2 RUMA 'Remove Unnecessarily Most Antagonists', is a plugin for Team Fortress 2. It checks each players TF2 total playtime as they are joining the server. If the hour limit, which can be set in the config, is too high for the connecting player, then he/she gets kicked.

## Requirements
 - [Sourcemod](http://www.sourcemod.net/downloads.php) 1.7.2 or higher
 - [SteamTools](https://builds.limetech.org/?p=steamtools) 0.9.1 or higher
 - [Steam API Key](http://steamcommunity.com/dev/apikey)

This plugin uses SQLite to save the accepted users. Make sure that the following code snipped exitst in the following file: 
```\addons\sourcemod\configs\databases.cfg```
```
"storage-local"
{
    "driver"    "sqlite"
    "database"  "sourcemod-local"
}
```

## Server ConVars
 - tf2ruma_version - Displays the plugin version.
 - sm_steam_api_key - Required for the playtime check to work.
 - sm_ruma_kickmsg - You can display the required hours to the kicked player if you wish. [ 1 - 0/1 ]
 - sm_ruma_log_level - Logging for the plugin. [ 1 - 0/2]
 - sm_ruma_hour_limit - The amount of hours required to join the server. [ 10 - 0/inf. ]

## Admin Command

 - sm_ruma_addplayer - Allows admins  to add a player into the DB, so they can join the server even if they don't meet the required playtime limit.