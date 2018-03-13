# 4.2 the cleanup update
## Changes
  - Lots of back-end work (more info below)
  - Permissions
    - The default group no longer exists.
      - Users have the default perms without needing the "Default" group.
    - Negative perms can now be used to remove permissions from a user.
    - Group hierarchy has been implemented meaning groups higher will override groups below them.
  - Buttons!
    - `_song` and `_skip` have buttons now. More to come in the future
    - Pages now have buttons for easy navigation.
  - Pages
    - Most pages should now be smaller and a bit bettee fitting. Most will also have buttons!
## Back-end
  - Cleaned up a lot of messy code.
  - Re-organized code so it's easier for other developers to pick up.
  - Added JavaDocs to pretty much everything.
  - Made a page system.
  - Changed perms over to hierarchy and negation system.
  - Moved a lot of stuff over to managers.

