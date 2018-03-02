# Permissions

## Version 4.2 permissions changes
In version 4.2 we have changed the permissions system to be, we believe, better. Here are some changes:
* There is no longer a default group. We have replaced this with a dynamic system that means that users get default permissions without a group. To list all of the default permissions, please refer to the `_perms list` command!
* We have introduced negation permissions meaning by putting a `-` before a permission will **deny** users access to the permission. This works in terms of group hierarchy; groups at the top will override groups at the bottom. User permissions will also immediately override group permissions.
* As mentioned before, groups now follow a hierarchy (Groups at the top being more important). To allow for this order to be changed we have introduced the command `_perms group <group> move <position>` to move the group up and down the chain. This order can bee seen by doing `_perms groups`!
* We have finally added the ability to do full and accurate permission validation meaning you will never be mistake on a permission again!


## Important Notes
* All FlareBot permissions follow a pattern of `flarebot.command` and `flarebot.command.sub-command` if applicable.
* All the permissions can be listed with `_perms list`. This command also tells you if the permissions are default or not.
* Everyone with `Administrator` Discord permission will have access to **all** commands.
* Everyone already has a select group of permissions to start off with. These are listed in the "Default" section of `_perms list`! To remove these permissions simply add the permission with a `-` before it to a user through user permissions or groups! (There should be no space between the `-` and the permission i.e. `-flarebot.play`)
* The `*` and `flarebot.*` permissions will grant **all** permissions, use it wisely!
* To find a command permission you can either see it on the commands page or do `_usage <command>` on Discord and it will show it in the response. All permissions can be viewed at `_perms list`.

## Some basic starter commands
If you wish to get going quickly these commands will be good to know!<br/>
`_perms group <name> add <permission>` - This will add a permission to a specific group.<br/>
`_perms group <name> remove <permission>` - This will remove a permission from a specific group.<br/>
`_perms group <name> link <role>` - This is how you can link a group to a specific Discord role. More info [here](#group-linking)<br/>

## Groups
FlareBot doesn't go directly off roles, we instead use something called "groups", these groups can be given to a user and control which permissions people have. Negative permissions can be added to groups to negate default permissions or permissions from groups below it.<br/>

You can create a new group with `_perms group <name> create` for example `_perms group Muted create`.<br/>
You can delete a group with `_perms group <name> delete` for example `_perms group Muted delete`.<br/>

## Adding & removing permissions to and from a group
It's super easy to add and remove permissions from a group. Just go to the header below for the command an example usage!

### Adding a permission
You can add a permission by simply doing the command `_perms group <name> add <permission>` for example if we want to add the mute command (which the permission is `flarebot.mute`) to the moderators we could do `_perms group Mods add flarebot.mute`.

### Removing a permission
You can remove a permission by simply doing the command `_perms group <name> remove <permission>` for example if we want to remove the ability to queue songs from Muted users then we could do `_perms group Muted remove flarebot.play`.

### Group linking
Group linking is basically linking a group to a role, this allows for you to add a role to a user __without__ them needing to have the group also added to them. It is a nice way to give a whole bunch of people certain permissions. Let's say we want to assign our `Muted` group to the `Muted` Discord role (which can be created by FlareBot in case of mutes). We can simply do `_perms group Muted link @Muted`, now here we can either mention the muted role or use the role ID (Which can be found in the `_roles` command).

## Users
Users can be given their own permissions individually from groups! These permissions will **always** overwrite group permissions so keep that in mind when checking issues with a permissions setup. Aside from their own permissions, users can also be assigned groups based on roles or manually adding the roles.

For adding groups with roles simply link the group with a role (As shown above) and the user will have access to that groups permissions without any further actions!

To add or remove groups from a user simply use `_perms user <user> group add|remove <group>` to add or remove a group from a user.

### User permissions
Adding and removing permissions is as simple as doing `_perms user <user> permission add|remove <perm>`! If you have trouble adding a permission, remember that you can view all our permissions at any time by doing `_perms list`. To remove *all* permissions from a user you can do `_perms user <user> clear` at anytime!

To list the permissions a specific user has been given, use the command `_perms user <user> permission list`! This will present a list of the permissions a user has been given. **Keep in mind that this is the list of permissions not gained from groups!**

To check the full list of permissions a user has access to, you can use the command `_perms user <user> check` which will list all the permissions (From groups and the user themselves) that they have access to. 

