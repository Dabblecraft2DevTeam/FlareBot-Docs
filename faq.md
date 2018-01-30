# Frequently Asked Questions
These are the most asked questions we get about FlareBot.

## Music Questions
#### How Do I Play Music
Simply join a voice channel and type `_play <search/url>`

#### How Do I Make The Bot Join A Private Voice Chat
That would be Discord perms my friend, of witch you can find a nice tutorial [here](https://support.discordapp.com/hc/en-us/articles/206029707-How-do-I-set-up-Permissions-) witch is written by Discord themselves. To Give you a brief rundown of what you need to do is you need to giver FlareBot it's self permissions to connect and speak in the channel, or you need to give a Role FlareBot is in permissions to connect and speak in the channel.

#### Can I Keep The Bot In A Voice Channel
tl;dr no

So the reason we don't allow this and most bots don't is because CPU usage. Just being in a voice chat uses more CPU then you think due to the threads for that voice chat still needing to be open. We also don't want FlareBot to get lonely, no one should be lonely :(

#### Why Isn't The Bot Playing X Song
Chances are the song is ether protected by copyright, or not available in France where the bot is hosted. Without knowing what song it is I can't give you a 100% for sure answer of why, but this is a good starting point. (FYI VEVO usually has their songs blocked due to us not seeing ads; some artists do still allow it though!)

#### Can I Load A Youtube Playlist?
Of course! Just make sure it is public, and run `_play <playlistURL>`.

#### How Can I Make A Playlist
The first thing you want to do is load a bunch of songs with `_play` and then simply do `_save <name>`. (not the best we know, but wait a bit ;) )

#### How Can I Add/Remove A Song From A Playlist
So we don't have a way to do this direct so you you need to do is load it with `_load <name>`and then do `_play <term/url>` to add and to remove do `_queue` and then `_queue remove <number>` and finally re-save the playlist with `_save <name>`.

#### Can I Play Spotify Playlists
No because it would be agents their ToS (Terms of Service). If you see any bot that does play Spotify playlists they either break Spotify ToS, or get the info on the song then get the song from Youtube. We may do this in the future but have no plans as of now.

#### How Can I Turn Of Skip Voting
You can't. If you want to skip without a vote you can do `_skip force`. If you want everyone to be able to do this you can add the `flarebot.skip.force` permission to the `Default` group. Go to the [Permissions page](/permissions) for info on this.

#### Can I Change The Volume
Nope, because of similar reasons to why you can't keep the bot in a voice channel. Sadly it is not a light task to decode the audio, change volume and re-encode all the time. 

## Moderation Questions
#### How Do I Add X Perm To Someone
Take a look at our [Permissions page](/permissions)!

#### Why Won't Selfassign/Autoassign Let Me Add A Role
High chances are it's because the role your trying to add is above the highest role Flarebot has. To fix this simply go into your server setting and move the FlareBot role up above the highest role you want to selfassign/autoassign.

#### Why Doesn't Mute Work
So the first thing to check for is the thing I mentioned in the last question. FlareBot's highest role need to be higher than the Muted role, and it needs to be higher then the highest role of the person you want to mute.

Now if they have the muted role and it's not working that because it didn't add channel overrides properly. This could be because you made the muted role your self or because the muted role is fairly low down on the list. So if you made the muted role your self you need to go to all your channels and override the muted role so it doesn't have speak perms. If the muted role is fairly low on the role list then It might be because the roles that user has that are higher then the muted role override it, so move the muted role up.

#### Why Can't I Do X To Someone
Have you been reading the last questions? Just quickly glance through those and you'll probably find the answer.

## Misc Questions
#### How Do I Self Host FlareBot
Short answer: You don't.
Long answer:
So FlareBot is open source and always will be. You can find it's code [here](https://github.com/FlareBot/FlareBot). That's the best I can give you. FlareBot has quite a few moving parts and quite a bit of required data needed to run including a Cassandra Cluster. Instead of creating quite complex self-hosting instructions which we'd need to maintain and help people with we instead just do not support it. We spend quite a bit of money to make sure FlareBot can run smoothly and for free to all our users. We run out of pocket and on the generous donations of our users. If you wish to donate then you can help us improve hardware and maybe you wont need to self-host :) For information on donating go [here](/donate).
