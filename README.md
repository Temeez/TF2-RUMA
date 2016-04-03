# TF2-RUMA
TF2 RUMA 'Remove Unnecessarily Most Antagonists', is a plugin for Team Fortress 2. It checks each players TF2 total playtime as they are joining the server. If the hour limit, which can be set in the config, is too high for the connecting player, then he/she gets kicked.

## Requirements
- [Sourcemod](http://www.sourcemod.net/downloads.php) 1.7.2 at minimum
- [SteamWorks](http://users.alliedmods.net/~kyles/builds/SteamWorks/) build 102 at minimum
- [Steam API Key](http://steamcommunity.com/dev/apikey)

## Server ConVars
- tf2ruma_version - Displays the plugin version.
- sm_steam_api_key - Required for the playtime check to work.
- sm_ruma_kickmsg - You can display the required hours to the kicked player if you wish. [ 1 - 0/1 ]
- sm_ruma_log_level - Logging for the plugin. [ 1 - 0/2]
- sm_ruma_hour_limit - The amount of hours required to join the server. [ 10 - 0/inf. ]
- sm_ruma_strict_mode - Kick player depending on the strict mode and playtime. [ 1 - 0/2 ]
- sm_ruma_kick_msg_text - Custom reject message for the kicked player, max length of this message is 256!

## Admin Command
- sm_ruma_addplayer - Allows admins  to add a player into the DB, so they can join the server even if they don't meet the required playtime limit.
