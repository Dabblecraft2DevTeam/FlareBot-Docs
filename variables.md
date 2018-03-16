# Variables
Quite a few messages in FlareBot have variable support, this means that when you add messages you can add things like mentioning the user, mentioning the channel etc. This is a page with all the variables we currently support and a note on the old deprecated ones.

**Note:** Not all these variables will work with every command! Most of them will work with all commands but some may not!

## Deprecated
To kick things off, these are variables people are quite used to but they are now becoming deprecated. Please update your messages to replace these!

`%user%` - User's name
`%mention%` - Mention the user
`%prefix%` - Guild prefix
`%tag%` - The tag used (From the `_tags` command)

## User Variables

  * `{user}` - User's name.
  * `{username}` - User's name.
  * `{nickname}` - User's nickname for a guild or their username if the guild is not passed or they're not a member.
  * `{tag}` - User's name and discrim in tag format - Username#discrim.
  * `{mention}` - User mention.
  * `{user_id}` - User's ID.
  *
<hr />

## Guild Variables

  * `{guild}` - Guild name.
  * `{region}` - Guild region (Pretty name - Amsterdam, Amsterdam (VIP)).
  * `{members}` - Total guild members.
  * `{owner}` - Guild owner's name.
  * `{owner_id}` - Guild owner's ID.
  * `{owner_mention}` - Guild owner mention.

<hr />

## Channel Variables

  * `{channel}` - Channel name.
  * `{channel_mention}` - Channel mention/
  * `{topic}` - Channel topic.
  * `{category}` - Category name or 'no category'