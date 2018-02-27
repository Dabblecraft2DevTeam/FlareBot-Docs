﻿# 4.2 the cleanup update
## Changes
 - Lots of back-end work (more info below)
 - Permissions
	 - The default group no longer exists.
		 - Users have the default perms without needing groups.
	 - Negative perms can now be used to remove permissions from a user.
	 - Group hierarchy has been implemented meaning groups higher will override groups below them.
 - Buttons!
	 - `_song` and `_skip` have buttons now. more to come in the future
	 - pages now have buttons for easy navigation
 - Pages
	 - They look nicer
	 - Some back-end work
## Back-end
- Cleaned up a lot of messy code
- Re-organized code so it's easier for other developers to pick up
- Added javadocs to pretty much everything
- Made a page system
- Changed perms over to hierarchy and negation system
- Moved a lot of stuff over to managers

