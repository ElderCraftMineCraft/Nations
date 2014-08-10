Nations
=======

Name: Nations

Version: 1.5

Creator: Templar3lf

Server: ElderCraft

Description: Nation Plugin for ElderCraft Minecraft server. For more information please visit our website at www.eldercraft.comxa.com.

commands:
-ncreate:
description: Creates a Nation.
usage: /ncreate <nation name>
permission: nations.create
-ndelete:
description: Deletes your current Nation.
usage: /ndelete
permission: nations.admin.delete
-nname:
description: Changes your Nation name.
usage: /nname [nation name]
permission: nations.admin.changename
-npromote:
description: Promotes a user within your Nation.
usage: /npromote <player name>
permission: nations.admin.promote
-ndemote:
description: Demotes a user within your Nation.
usage: /ndemote <player name>
permission: nations.admin.demote
-nlist:
description: Lists all current Nations.
usage: /nlist
permission: nations.list
-nshow:
description: Shows info for a Nation.
usage: /nshow <nation name>
permission: nations.show
-ncolour:
description: Changes your Nations colour.
usage: /ncolour <colour>
permission: nations.admin.colour
-ncolor:
description: Alias for ncolour.
usage: /ncolour <color>
permission: nations.admin.colour
-nkick:
description: Kicks a player from your Nation.
usage: /nkick <player name> [reason]
permission: nations.admin.kick
-ninherit:
description: Gives control of the Nation to the specified user.
usage: /ninherit <player name>
permission: nations.admin.inherit
-njoin:
description: Joins the Nation you specify.
usage: /njoin <nation name>
permission: nations.join
-nleave:
description: Leaves the Nation you are in.
usage: /nleave
permission: nations.leave
-nrecruit:
description: Sets the Nation recruitment status.
usage: /nrecruit <true|false>
permission: nations.admin.recruit
-nsetspawn:
description: Sets the Nation Spawnpoint.
usage: /nsetspawn
permission: nations.admin.setspawn
-nspawn:
description: Goes to your Nations Spawnpoint.
usage: /nspawn
permission: nations.spawn
-nchat:
description: Enables and disabled Nation chat.
usage: /nchat
permission: nations.chat
-nclaim:
description: Adds a chunk to the Nation claimed land.
usage: /nclaim
permission: nations.admin.claim
-nabandon:
description: Removes a chunk from the Nation claimed land.
usage: /nabandon
permission: nations.admin.abandon
-nstatus:
description: Sets the Nation aggression status.
usage: /nstatus <aggressive|peaceful>
permission: nations.status
-nmessage:
description: Sets the Nation land enter message.
usage: /nmessage <message>
permission: nations.admin.message

I'd suggest giving lowest level players the nations.admin.*, as these commands can only be executed when the player is a Nation Admin or Owner, and should not depend on Server rank.

ChangeLog:

09/08/2014 [3]:
- Added /nmessage to change the message displayed to a player when entering claimed land.
- Default message stored in the config file and can be changed.
- These messages are now in Nation colour, for convenience.
- Added /nname command to let a Nation owner change the name of the Nation.
- Squashed more bugs, including an error when a percentage sign is said in chat.
- Fixed up and neatened the /nkick command.

09/08/2014 [2]:
- Finished /nstatus command.
- Updated entity-hurt-entity event to react to Nation statuses.
- Added global broadcasts when Nations change statuses, including recruitment.
- Introduced proper permission handling instead of the nonsense there before.

09/08/2014:
- Added in claim land command.
- Added in player events to catch when a player moves between claimed lands.
- Added in player block creation and destruction in player land and restrictions.
- Added in the concept of aggression and peace.
- Started work on /nstatus [aggressive/peaceful].

07/08/2014:
- First proper update for Nations Plugin.
- Finished complete re-write using objects and structured programming.
- Most commands complete including new command nchat and others.
- Most errors crushed and bugs squashed.

??/??/2013:
- Started early plugin development.
- Finished initial version; missing many features.
- Gained sufficient knowledge of Bukkit API to re-write.
