# Fork
+ this fork's main goal is to work on some personal changes that I prefer with the bot and I figured there may be others who like them
+ these issues include: claiming after already having claimed, issues with last minute claims and some other things.

# MudaeAutoBot
MudaeAutoBot is a python bot that auto rolls and attempts to snipe Kakeras and Claims in Mudae

# Features
+ Snipes and claims Kakera in any Discord servers you're in that has Mudae#0807
+ Kakera value sniping as long as kakera value can be determined (e.g. Like Rank, Claim Rank, ## Kakera)
+ Maximizes rolls by tracking roll timers
+ Waifu/Husbando rolling
+ Pokeslot rolling
+ Selective Kakera Reaction Snipes Features(Includes: Soulmate Kak sniping Feature)
+ Mudae emoji reaction event sniping support

## How it works
All this bot needs to work is your Discord _usertoken_ and the channel IDs that you want it to post in

This is intended to be completely automated; it doesn't need to take any input other than initial settings configuration.
You'll be able to leave the window running in the background, and not need to think about it.

## Requirements

+ Python 3.7+
+ discum 1.3+

# Configuration
To configure the bot, you'll edit the variables in the **Settings_Mudae.json** file for your botting needs.

## Bot settings
All settings are set within the Settings_Mudae.json File

+ `token` - The user token for the account you want to bot on. If you need extra assistance on how to obtain it, let me know.
+ `channelids` - Which channels to **roll** and **monitor**  e.g. 807##########948
+ `slash_ids` - Which channels to **Slash roll** e.g. 807##########948 (Please Match Slash_id with slash_guild_id)
+ `slash_guild_ids` - Which Guild to **Slash roll** e.g. 807##########948 (Please Match Guild id with Slash_id)
+ `claim_delay` - _Affects servers w/o $setting instance_ Time in **seconds** to wait before attempting to Claim Characters e.g. 5
+ `kak_delay` - _Affects servers w/o $setting instance_ Time in **seconds** to wait before attempting to snipe Kakeraloot e.g. 8
+ `use_emoji` - This setting only works if you change the Mudaebot.py code by uncommenting out the line (Custom emojis only) e.g.  "<:emoji_name:795############214>"
+ `roll_this` - ($m|$ma|$mg|$w|$wg|$wa|$h|$ha|$hg) If `Rolling` is enabled it will roll this specific command e.g. '$wg'
+ `Rolling` - (True|False) **Case-sensitive**, uses `channelid`
+ `slash Rolling` - (True|False) **Case-sensitive**, uses `Slash_ids`
+ `PkmRolling` - (True|False) Pokeslot rolling enabled, uses `channelid`
+ `series_list` - **Case-sensitive** Name of series of characters you want to claim  e.g. \[ "Honkai Impact 3rd" , "Senran Kagura" \]
+ `name_list` - **Must be exact match** List of specific character names to claim  e.g. \["Raiden Mei", "gOkU" \]
+ `emoji_list` - This is the kakera that will be snipes \[ "KakeraY" , "KakeraO" \] << This example means only snipe Yellow and orange Kakera
+ `min_kak` - A minimum kakera value to snipe a claimable character _regardless of whether it's in the series/name lists_
+ `Last_True` -  (True|False) enable Last Minute Claim windows
+ `last_claim_min` - (1-180) the window the window is open for e.g. 10 means last 10 minutes
+ `min_kak_last_min` - same as min kak but only within the last minute claim window

# Optimize the snipes
Typing $settings in your server with mudae should give you the snipe and kaksnipping timers.
Using these values you usually snipes faster than a "Human" user can react 

Please when settings Delays avoid setting 0 as your delay as it might be to fast for mudae
a minimum of 1 second to let mudae register that a character was rolled as is reacted to.

# Use at your own Risk
This is a Discord **selfbot**. I am not responsible if you get banned using this program. 



