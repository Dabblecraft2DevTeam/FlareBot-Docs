# 4.2 the cleanup update
## Changes
 - Lots of back-end work (more info below)
 - Permissions
	 - The default group no longer exists.
		 - Users have the default perms without needing groups.
	 - Negative perms can now be used to remove permissions from a user.
	 - Group hierarchy has been implemented meaning groups higher will override groups below them.
	 - Clone and rename have been added for groups
 - Buttons!
	 - `_song` and `_skip` have buttons now. More to come in the future
	 - Pages now have buttons for easy navigation.
 - Pages
	 - They look nicer.
	 - Some back-end work.
 - Nino
	 - It's an anti invite system for your server. You can find everything you need for nino in the `_nino` command
 - Jumbo
	 - Ever wanted bigger emotes? Now you can with the jumbo command.
	 - Supports up the 5 emotes at once, and gives info on emotes
	 - Note: Only works on custom emotes
 - Settings
	 - Guild settings are now a thing!
	 - Settings allows you to blacklist channels and various other things you might want to change about the bot.
## Back-end
- Cleaned up a lot of messy code.
- Re-organized code so it's easier for other developers to pick up.
- Added JavaDocs to pretty much everything.
- Made a page system.
- Changed perms over to hierarchy and negation system.
- Moved a lot of stuff over to managers.

