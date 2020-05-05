# [Isabelle Documentation](https://isabelle.gg, "Isabelle Website")
## Preface
This documents usage for all of Isabelle's commands, if you have any questions please see the [support server](https://isabelle.gg/discord).
Arguments inside of < > mean they are not required to run the command, arguments inside [ ] will be required to run the command.
### Quick Links
[Information](#Information-Documentation)\
[Music](#Music-Documentation)\
[Moderation](#Moderation-Documentation)\
[Miscellaneous](#Miscellaneous-Documentation)\
[Server](#Server-Documentation)

### Information Documentation
- \~help \<command\> || Sends the sender a DM containing all of Isabelle's commands. If *\<command\>* exists, it will send information about the specified command. This is the only command that works inside of DMs.
```
Usage:

~help
~help mute
```
- \~donate || Sends an embed that contains information regarding donating to the project.
```
Usage:

~donate
```
- \~info || Sends an embed regarding information about Isabelle.
```
Usage:

~info
```
- \~ping || Pings the client and the Discord API, returns the recorded latency.
```
Usage:

~ping
```
- \~support || Sends an embed for the support discord server.
```
Usage:

~support
```
- \~uptime || Sends a message returning the uptime of Isabelle
```
Usage:

~uptime
```
- \~changelog || Sends an embed with the latest version of Isabelle's changelog. This command shows recent changes, features, bugfixes, etc.
```
Usage:

~changelog
```
### Music Documentation
- \~play \[link / title\] || If Isabelle is not already connected to a Voice Channel, it will join the one the sender is in and add *\[link / title\]* to the queue. Supports SoundCloud, YouTube, and Http (basically mp3 files that are hosted on a server). If Isabelle is already playing music, you must be in the same VC as the bot to use this.
```
Usage:

~play https://soundcloud.com/chriswrightotj/everything-is-backwards
~play https://isabelle.gg/cloudmacarchive/vibes..mp3
~play https://www.youtube.com/watch?v=fiPR0vpxdas
~play Ice Cube - It Was A Good Day
```
- \~stop || If Isabelle is connected to a Voice Channel, it will leave. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~stop
```
- \~shuffle || Shuffles the guild's queue, if it exists. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~shuffle
```
- \~nowplaying || If there is a song playing in the guild, Isabelle will send an embed containing what track is playing.
```
Usage:

~nowplaying
```
- \~nowplaying || If Isabelle is playing music, this command will display the current queue of tracks/songs for the guild. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~queue
```
- \~remove \[track q#] || If Isabelle is playing music, and has a queue greater than 1, this will remove whichever the index for *\[track q#\]*. You can check the indexes of songs via *\~queue*. If this is used with only one song, and that song is the one playing, Isabelle will leave the VC. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~remove 1
```
- \~skip || If Isabelle is playing music, this will skip the currently playing track. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~skip
```
- \~pause || If Isabelle is playing music, this will pause the currently playing track. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~pause
```
- \~resume || If Isabelle is paused, this will resume the currently playing track. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~resume
```
- \~devpicks || If Isabelle is not connected to the VC, it will join. If it is, you must be in the same one to use this command. This will queue up a playlist selected by myself.
```
Usage:

~devpicks
```
- \~volume \[num 1-100\] || If Isabelle is playing music, this will set the volume to *\[num 1-100\]*. Must be inside the VC Isabelle is in to use this command.
```
Usage:

~volume 45
```
### Moderation Documentation
- \~addrole \[user\] \[role\] || Requires **MANAGE_ROLES**. If *\[role\]* exists in the guild and *\[user\]* exists in the guild, it will be given to the mentioned *\[user\]*.
```
Usage:

~addrole @Azurilex#0001
~addrole @Azurilex#0001 Administrator
```
- \~removerole \[user\] \[role\] || Requires **MANAGE_ROLES**. If *\[role\]* exists in the guild and *\[user\]* has it, it will be taken away from the mentioned *\[user\]*.
```
Usage:

~removerole @Azurilex#0001
~removerole @Azurilex#0001 Administrator
```
- \~ban \[user\] \<reason\> || Requires **BAN_MEMBERS**. If *\[user\]* exists in the guild and Isabelle has proper privileges to ban them, they will be banned. This will send a message to the user saying they've been banned, as well as a chat message. Both messages will contain *\<reason\>*, if it exists.
```
Usage:

~ban @Azurilex#0001
~ban @Azurilex#0001 too cool for school :sunglasses:
```
- \~unban \[user\] \<reason\> || Requires **BAN_MEMBERS**. If *\[user\]* exists (usually user id works best for this command) and Isabelle has proper privileges to unban them, they will be unbanned. This will send a message to the user saying they've been unbanned, as well as a chat message. Both messages will contain *\<reason\>*, if it exists.
```
Usage:

~unban <@504028264839512104>
~unban <@504028264839512104> too cool for school :sunglasses:
```
- \~softban \[user\] \<reason\> || Requires **BAN_MEMBERS**. If *\[user\]* exists in the guild and Isabelle has proper privileges to ban them, they will be banned. Immediately after, they will be unbanned - this command basically just deletes their messages and kicks them. This will send a message to the user saying they've been softbanned, as well as a chat message. Both messages will contain *\<reason\>*, if it exists.
```
Usage:

~softban @Azurilex#0001
~softban @Azurilex#0001 y u so cool dude, our server can't handle ur iq
```
- \~kick \[user\] \<reason\> || Requires **KICK_MEMBERS**. If *\[user\]* exists in the guild and Isabelle has proper privileges to kick them, they will be kicked. This will send a message to the user saying they've been kicked, as well as a chat message. Both messages will contain *\<reason\>*, if it exists.
```
Usage:

~kick @Azurilex#0001
~kick @Azurilex#0001 too cool for this server :sunglasses:
```
- \~mute \[user\] \<reason\> || Requires **MANAGE_MESSAGES**. If *\[user\]* exists in the guild and Isabelle has proper privileges to add a role to them, they will be muted. This will send a message to the user saying they've been muted, as well as a chat message. Both messages will contain *\<reason\>*, if it exists.
```
Usage:

~mute @Azurilex#0001
~mute @Azurilex#0001 u suck bro
```
- \~unmute \[user\] \<reason\> || Requires **MANAGE_MESSAGES**. If *\[user\]* exists in the guild and Isabelle has proper privileges to add a role to them, they will be unmuted. This will send a message to the user saying they've been unmuted, as well as a chat message. Both messages will contain *\<reason\>*, if it exists.
```
Usage:

~unmute @Azurilex#0001
~unmute @Azurilex#0001 jk
```
- \~purge \[number\] || Requires **MANAGE_MESSAGES**. If *\[number\]* exists, it will mass-delete *\[number\]* messages in the channel the command was executed in. Due to Discord API limitations, this cannot delete messages older than 14 days.
```
Usage:

~purge 100
```
- \~warn \[user\] \[reason\] || Requires **MANAGE_MESSAGES**. If *\[user\]* exists in the guild and *\[reason\]* was provided, *\[user\]* will be warned. This will send a message to the user saying they've been warned, as well as a chat message. Both messages will contain *\[reason\]*.
```
Usage:

~warn @Azurilex#0001 lol stop spamming ~shawty
```
- \~warnings \<user\> || If *\<user\>* doesn't exist, it will default to the sender of the message. This will send an embed containing *\<user\>*'s warnings.
```
Usage:

~warnings
~warnings @Azurilex#0001
```
- \~clearwarns \[user\] || Requires **MANAGE_MESSAGES**. Clears *\[user\]*'s warnings. Gives them a clean slate :)
```
Usage:

~clearwarns @Azurilex#0001
```
### Miscellaneous Documentation
- \~coronavirus \<country name / initials\> || If *\<country name / initials\>* doesn't exist, it will default to the United States. Sends an embed containing the current COVID-19 statistics for  *\<country name / initials\>*.
```
Usage:

~coronavirus
~coronavirus S. Korea
```
- \~avatar \<user\> || If *\<user\>* doesn't exist, it will default to the sender. Sends an embed containing *\<user\>*'s Discord profile picture.
```
Usage:

~avatar
~avatar @Azurilex#0001
```
- \~btc || Sends an embed containing the current BTC/USD rate. BTC = Bitcoin
```
Usage:

~btc
```
- \~eth || Sends an embed containing the current ETH/USD rate. ETH = Ethereum
```
Usage:

~eth
```
- \~xrp || Sends an embed containing the current XRP/USD rate. XRP = Ripple
```
Usage:

~xrp
```
- \~embedsay \[message\] || Requires **MANAGE_MESSAGES**. Sends an embed containing *\[message\]*.
```
Usage:

~embedsay isabelle is a cool bot
```
- \~say \[message\] || Requires **MANAGE_MESSAGES**. Sends a message containing *\[message\]*.
```
Usage:

~say isabelle is a dope bot
```
- \~serverinfo || Sends an embed containing information about the server.
```
Usage:

~serverinfo
```
- \~userinfo \[user\] || If *\[user\]* exists in the guild, Isabelle will send an embed containing information about *\[user\]*.
```
Usage:

~userinfo @Azurilex#0001
```
- \~shawty || Sends an embed with a shawty. My personal favorite.
```
Usage:

~shawty
```
### Server Documentation
- \~prefix \[string\] || If *\[string\]* exists, Isabelle's prefix for the guild will be set to *\[string\]*.
```
Usage:

~prefix !
```
- \~welcomemsg || If this command is run by itself, it will display the current guild settings for welcome messages.
    - \<on/off\> || Turns Isabelle welcome messages *\<on/off\>*.
    - \<msg\> || Sets Isabelle welcome messages to *\<msg\>*. You can mention the user in the *\<msg\>* by using *{user}* wherever you want to message them.
    - \<channel\> || Sets Isabelle welcome messages channel to *\<channel\>*.
```
Usage:

~welcomemsg on
~welcomemsg welcome to the server {user}!
~welcomemsg #welcome-log
```
- \~userxp \[on/off\] || Turns guild member experience to *\[on/off\]*. This is off by default, if turned on, members can gather XP just by chatting.
```
Usage:

~userxp on
```
- \~leaderboard || If guild userxp is on, this will display the top 10 users in the guild with the highest XP count.
```
Usage:

~leaderboard
```
