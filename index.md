# Welcome to FlareBot Docs
FlareBot is a free Discord music and server administration bot that delivers high-quality music to your Discord server while also providing tools to run your server with ease. FlareBot can be easily added into your Discord server with no setup or configuration required.

## Setting up the bot
FlareBot is made to be super simple to use! Getting FlareBot running on your server is easy, you can invite FlareBot by authenticating it with using [this](https://goo.gl/NfYi94) link. Bear in mind that you must have `Manage Server` permissions to be able to do this. From there you are good to go with being able to use music and moderators should be able to use any moderation commands they need. We have a very flexible permission system which you can also use to limit what certain users can do, check it out [here](/docs/permissions).

## Main Commands
> Note that if you changed the prefix from `_` then you will need to use your server prefix. You can check your prefix with `_prefix` or mentioning the bot.
> You can also do `_help` for a list of all the commands (You have access to) in your server!

> Key: 
> <> = required
> [] = optional

| Command | Description | Usage |
| ------- | ----------- | ----- |
| \_help [category] | Show all the commands or a certain category if specified. | \_help<br/> \_help Music<br/> \_help Moderation |
| \_join | Make the bot join the Voice Channel you're currently in.<br/> To make the bot join your Voice Channel when it is already in one you need the `flarebot.join.other` permission. | \_join |
| \_leave | Make the bot leave the Voice Channel it's currently in.<br/> If the bot is already in a Voice Channel which you're not in to make it leave you need the `flarebot.leave.other` permission. | \_leave |
| \_play <term/url> | Search YouTube for a term or directly with a URL to find and play a video!<br/> If FlareBot is not in a channel and you're in one when the command is done it will join yours! | \_play Alan Walker - Faded<br/> \_play https://www.youtube.com/watch?v=60ItHLz5WEA |
| \_search <term> | Search for the top 5 results of your term on YouTube and then pick which one to play. | \_search Faded |
| \_skip [force] | Vote to skip the currently playing song with this command, it allows people in the voice channel to do `_skip yes/no` and vote to skip or leave it.<br/> If you have the `flarebot.skip.force` permission you can do `_skip force` and skip the song without the vote! | \_skip<br/> \_skip yes<br/> \_skip force |
| \_song | Gets the current playing song information. This will return the song name, how long it has been playing (and has left). | \_song |
| \_stop | Stops the current playing song and clears the playlist. If you want to just pause the music you can use the `_pause` command. | \_stop |
| \_queue [here] \_queue clear \_queue remove <item> | Get the current queue sent to you in DMs or in the channel you executed the command (in case of  `_queue here`).<br/> To remove all the songs in the current queue you can do `_queue clear`. Requires: `flarebot.playlist.clear`.<br/> You can remove an item from the queue with `_queue remove <item>` just do `_queue` get the number and supply that as the item argument! Requires: `flarebot.playlist.remove`. | \_queue<br/> \_queue clear<br/> \_queue remove 10 |
| \_loop | Loop the current queue, this will do a continuous loop of the entire playlist. If you wish to repeat a song you can use `_repeat`. | \_loop |
| \_shuffle | Shuffle the order of the current queue. | \_shuffle |
| \_ban <user> [reason] | Ban a user from the server, this can be done by mentioning the user, putting their username or their full tag.<br/> Note that usernames are not unique so a mention or tag (Username#discrim) is more reliable!<br/> After the username you can also put a reason for banning the user which will be put into the ban message, the modlog and the server audit log.<br/> Can tempban with `_tempban <user> <duration> [reason]` | \_ban Walshy<br/> \_ban Walshy#9060 Being too cool. |
| \_kick <user> [reason] | Kick a user from the server, this can be done by mentioning the user, putting their username or their full tag.<br/> Note that usernames are not unique so a mention or tag (Username#discrim) is more reliable!<br/> After the username you can also put a reason for banning the user which will be put into the ban message, the modlog and the server audit log. | \_kick Walshy<br/> \_kick Walshy#9060 Too hot for our blood. |
| \_mute <user> [reason] | Kick a user from the server, this can be done by mentioning the user, putting their username or their full tag.<br/> Note that usernames are not unique so a mention or tag (Username#discrim) is more reliable!<br/> After the username you can also put a reason for banning the user which will be put into the ban message, the modlog and the server audit log.<br/> Can tempmute with `_tempmute <user> <duration> [reason]` | \_mute Walshy<br/> \_mute Walshy#9060 Spamming v3 memes. |

## Adding music to the queue
Adding music to the queue is pretty simple. To start playing a song, use the `_play command`. Here are two examples:
```
_play Alan Walker - Faded
_play https://www.youtube.com/watch?v=60ItHLz5WEA
```
You can search for a term which in this case is `Alan Walker - Faded` or directly by a URL which above is `_play https://www.youtube.com/watch?v=60ItHLz5WEA`.

> FlareBot will not be able to play tracks blocked in France (usually due to copyright infringements on YouTube).

**Supported sites:**

* YouTube 

We will be expanding our supported sites into a lot more very soon, including but not limited to Twitch, Mixer, SoundCloud and Radio Stations. If you want to request any others head over to our [Discord Server](https://flarebot.stream/support-server)!

## Join FlareBot Server!
We invite everyone to join FlareBot Official Server, which is a place to discuss suggestions, report bugs and request for support. We're very open to any suggestions you may have, some of our most used features came from you guys! [Click here to join!](https://flarebot.stream/support-server)

## Support
Before you do anything, please [read our FAQ](/docs/faq).

You can join either our [Discord server](https://flarebot.stream/support-server) or tweet us at [@DiscordFlareBot](https://twitter.com/DiscordFlareBot).

## Credits
FlareBot is developed by Walshy with the help of contributors on GitHub. Huge thanks to all the work done by BinaryOverload and weeryan17 over the course of the project also!

Special thanks to EJ Technologies for providing us with open source licenses for their [Java profiler](https://www.ej-technologies.com/products/jprofiler/overview.html).

[![JProfiler](https://www.ej-technologies.com/images/product_banners/jprofiler_large.png)](https://www.ej-technologies.com/products/jprofiler/overview.html)

This site is hosted as an open source project on [Netlify](https://www.netlify.com/).
