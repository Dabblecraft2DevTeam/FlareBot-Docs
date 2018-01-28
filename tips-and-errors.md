# Tips
Some tips on how to get information for FlareBot.

## How To Get a User's ID
1. You can do `_userinfo [user]` to find your (or another users) ID, you will see an `ID: <numbers>` under `User Info`, the numbers are the user's ID.
2. To get a User ID simply enable developer mode by going to User `Settings > Appearance > Developer Mode` then just right click the user and click `Copy ID`

## How To Get a Guild ID
1. You can do `_serverinfo` and in the footer you will see an `ID: <numbers>`, the numbers are the guild ID.
2. To get your Guild ID simply enable developer mode by going to `User Settings > Appearance > Developer Mode` then just right click your guild icon and click `Copy ID`

# Common Errors
Some common errors, what they mean and how to solve them.

## User Not Found
The `User not found` error (or similar) is usually caused by them not being in your guild **and** us not sharing a guild with the requested user. What we do when you pass something like a name or tag is we search for the guilds we're in and then can handle that person. What you can do (in most cases) is use a person's ID (Not `username#discrim` - That's a tag) and this will make us query Discord to get any info we need about the user otherwise we will just handle them with the ID.