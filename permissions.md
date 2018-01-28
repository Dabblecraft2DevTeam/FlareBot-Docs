# Permissions

<!-- > ### In 4.2 permissions are changing! Please read the `Permissions (4.2)` page for more info! -->

## Important Notes
* All FlareBot permissions follow a pattern of `flarebot.command` and `flarebot.command.sub-command` if applicable. 
* Everyone with `Administrator` Discord permission will have access to **all** commands.
* Everyone already has a group before you do anything, the group is called `Default`.
* The `*` and `flarebot.*` permissions will grant **all** permissions, use it wisely!
* To find a command permission you can either see it on the commands page or do `_usage <command>` on Discord and it will show it in the response. Note that you cannot find sub-command permissions easily!

## Some basic starter commands
If you wish to get going quickly these commands will be good to know!<br/>
`_perms group <name> add <permission>` - This will add a permission to a specific group.<br/>
`_perms group <name> remove <permission>` - This will remove a permission from a specific group.<br/>
`_perms group <name> link <role>` - This is how you can link a group to a specific Discord role. More info [here](#group-linking)<br/>

## Groups
FlareBot doesn't go directly off roles, we instead use something called "groups", these groups can be given to a user and control which permissions people have. There is one group right off the bat which is called `Default` this is a group everyone has and every new person will get. If you wish to remove a permission from everyone then removing it from the `Default` group is the best way to go.<br/>
You can create a new group with `_perms group <name> create` for example `_perms group Muted create`.<br/>
You can delete a group with `_perms group <name> delete` for example `_perms group Muted delete`.<br/>

## Adding & removing permissions to and from a group
It's super easy to add and remove permissions from a group. Just go to the header below for the command an example usage!

### Adding a permission
You can add a permission by simply doing the command `_perms group <name> add <permission>` for example if we want to add the mute command (which the permission is `flarebot.mute`) to the moderators we could do `_perms group Mods add flarebot.mute`.

### Removing a permission
You can remove a permission by simply doing the command `_perms group <name> remove <permission>` for example if we want to remove the ability to queue songs from Muted users then we could do `_perms group Muted remove flarebot.play`.

## Group linking
Group linking is basically linking a group to a role, this allows for you to add a role to a user __without__ them needing to have the group also added to them. It is a nice way to give a whole bunch of people certain permissions. Let's say we want to assign our `Muted` group to the `Muted` Discord role (which can be created by FlareBot in case of mutes). We can simply do `_perms group Muted link @Muted`, now here we can either mention the muted role or use the role ID (Which can be found in the `_roles` command).
