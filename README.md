# These groups only contain permission nodes.
#
# **** You can NOT add anything other than permission nodes ****
# **** This is NOT where you set up the groups which you give to users! ****
# **** goto groupmanager/worlds/worldname/groups.yml if you want to set the actual groups! ****
#
# These collections are to be inherited in your different worlds groups.yml's
# They can also be added as one of a users subgroups, but NOT as a primary group.
# These collections are available to ALL group and user yml's.
#
# Add to and customize these groups to fit your needs.

groups:

# Permission nodes for GroupManager
# by ElgarL, snowleo, continued from gabrielcouto's original
# http://wiki.ess3.net

  g:groupmanager_default:
    permissions:
    - groupmanager.notify.self

  g:groupmanager_moderator:
    permissions:
    - groupmanager.listgroups
    - groupmanager.mandemote
    - groupmanager.manpromote
    - groupmanager.manselect
    - groupmanager.manuadd
    - groupmanager.manudel
    - groupmanager.manwhois
    - groupmanager.notify.other

  g:groupmanager_admin:
    permissions:
    - groupmanager.mantogglevalidate
    - groupmanager.mansave
    - groupmanager.mangcheckp
    - groupmanager.manglistp
    - groupmanager.manucheckp
    - groupmanager.manulistp

# Permission nodes for CraftBukkit
# by many devs and contributors
# http://dl.bukkit.org/

  g:bukkit_default:
    permissions:
    - bukkit.broadcast.user
    - -bukkit.command.plugins
    - essentials.msg
    - essentials.helpop.receive

  g:bukkit_moderator:
    permissions:
    - bukkit.command.ban
    - bukkit.command.ban.ip
    - bukkit.command.ban.player
    - bukkit.command.gamemode
    - bukkit.command.kick
    - bukkit.command.unban
    - bukkit.command.unban.ip
    - bukkit.command.unban.player

  g:bukkit_admin:
    permissions:
    - bukkit.broadcast
    - bukkit.broadcast.admin
    - bukkit.command.give
    - bukkit.command.help
    - bukkit.command.kill
    - bukkit.command.list
    - bukkit.command.me
    - -bukkit.command.op
    - -bukkit.command.op.give
    - -bukkit.command.op.take
    - bukkit.command.plugins
    - bukkit.command.reload
    - bukkit.command.save
    - bukkit.command.save.disable
    - bukkit.command.save.enable
    - bukkit.command.save.perform
    - bukkit.command.say
    - bukkit.command.stop
    - bukkit.command.teleport
    - bukkit.command.tell
    - bukkit.command.time
    - bukkit.command.time.add
    - bukkit.command.time.set
    - bukkit.command.version
    - bukkit.command.whitelist
    - bukkit.command.whitelist.add
    - bukkit.command.whitelist.disable
    - bukkit.command.whitelist.enable
    - bukkit.command.whitelist.list
    - bukkit.command.whitelist.reload
    - bukkit.command.whitelist.remove

# Permission nodes for Essentials
# by ementalo, snowleo, and KHobbits
# http://dev.bukkit.org/server-mods/essentials/

  g:essentials_default:
    permissions:
    - essentials.help
    - essentials.helpop
    - essentials.list
    - essentials.motd
    - essentials.rules
    - essentials.spawn
    - essentials.jail.allow.help
    - essentials.jail.allow.helpop
    - essentials.jail.allow.rules

  g:essentials_builder:
    permissions:
    - essentials.afk
    - essentials.afk.auto
    - essentials.back
    - essentials.back.ondeath
    - essentials.balance
    - essentials.balance.others
    - essentials.balancetop
    - essentials.book
    - essentials.chat.color
    - essentials.chat.format
    - essentials.chat.shout
    - essentials.chat.question
    - essentials.compass
    - essentials.delhome
    - essentials.depth
    - essentials.exp
    - essentials.getpos
    - essentials.hat
    - essentials.home
    - essentials.ignore
    - essentials.itemdb
    - essentials.kit
    - essentials.kits.tools
    - essentials.mail
    - essentials.mail.send
    - essentials.me
    - essentials.msg
    - essentials.msg.color
    - essentials.msg.format
    - essentials.nick
    - essentials.pay
    - essentials.ping
    - essentials.powertool
    - essentials.powertooltoggle
    - essentials.protect
    - essentials.recipe
    - essentials.seen
    - essentials.sethome
    - essentials.sethome.bed
    - essentials.sethome.multiple
    - essentials.signs.use.*
    - essentials.signs.create.disposal
    - essentials.signs.create.mail
    - essentials.signs.create.protection
    - essentials.signs.create.trade
    - essentials.signs.break.disposal
    - essentials.signs.break.mail
    - essentials.signs.break.protection
    - essentials.signs.break.trade
    - essentials.suicide
    - essentials.time
    - essentials.tpa
    - essentials.tpaccept
    - essentials.tpahere
    - essentials.tpdeny
    - essentials.warp
    - essentials.warp.list
    - essentials.worth
    - essentials.jail.allow.mail
    - essentials.jail.allow.ping
    - essentials.jail.allow.seen

  g:essentials_moderator:
    permissions:
    - -essentials.spawner.enderdragon
    - essentials.afk.kickexempt
    - essentials.ban
    - essentials.ban.notify
    - essentials.banip
    - essentials.book.title
    - essentials.book.others
    - essentials.broadcast
    - essentials.chat.url
    - essentials.chat.magic
    - essentials.clearinventory
    - essentials.delwarp
    - essentials.eco.loan
    - essentials.exp.others
    - essentials.ext
    - essentials.fly
    - essentials.fly.safelogin
    - essentials.getpos
    - essentials.getpos.others
    - essentials.helpop.receive
    - essentials.home.others
    - essentials.invsee
    - essentials.jails
    - essentials.jump
    - essentials.kick
    - essentials.kick.notify
    - essentials.kill
    - essentials.kits.*
    - essentials.msg.magic
    - essentials.mute
    - essentials.mute.notify
    - essentials.nick.color
    - essentials.nick.others
    - essentials.realname
    - essentials.seen.banreason
    - essentials.seen.extra
    - essentials.setwarp
    - essentials.signs.create.*
    - essentials.signs.break.*
    - essentials.spawner
    - essentials.spawner.*
    - essentials.thunder
    - essentials.time
    - essentials.time.set
    - essentials.protect.alerts
    - essentials.protect.admin
    - essentials.protect.ownerinfo
    - essentials.ptime
    - essentials.ptime.others
    - essentials.togglejail
    - essentials.top
    - essentials.tp
    - essentials.tp.others
    - essentials.tphere
    - essentials.tppos
    - essentials.tptoggle
    - essentials.unban
    - essentials.unbanip
    - essentials.vanish
    - essentials.vanish.effect
    - essentials.warps.*
    - essentials.weather
    - essentials.whois
    - essentials.workbench
    - essentials.world
    - essentials.worlds.*
    - essentials.jail.allow.jails
    - essentials.jail.allow.togglejail

  g:essentials_admin:
    permissions:
    - -essentials.backup
    - -essentials.essentials
    - -essentials.setspawn
    - -essentials.reloadall
    - -essentials.plugin
    - essentials.*

# Permission nodes for Towny by ElgarL
# http://dev.bukkit.org/server-mods/towny-advanced/

  g:towny_default:
    permissions:
    - towny.chat.local

  g:towny_builder:
    permissions:
    - towny.wild.build.6
    - towny.wild.destroy.6
    - towny.wild.destroy.14
    - towny.wild.destroy.15
    - towny.wild.destroy.16
    - towny.wild.build.17
    - towny.wild.destroy.17
    - towny.wild.destroy.18
    - towny.wild.destroy.21
    - towny.wild.destroy.31
    - towny.wild.destroy.37
    - towny.wild.destroy.38
    - towny.wild.destroy.39
    - towny.wild.destroy.40
    - towny.wild.destroy.50
    - towny.wild.destroy.56
    - towny.wild.destroy.73
    - towny.wild.destroy.74
    - towny.wild.destroy.78
    - towny.wild.destroy.81
    - towny.wild.destroy.82
    - towny.wild.destroy.83
    - towny.wild.destroy.86
    - towny.wild.destroy.103
    - towny.wild.destroy.106
    - towny.wild.destroy.111
    - towny.wild.destroy.115

  g:towny_moderator:
    permissions:
    - towny.chat.mod
    - towny.wild.switch.64
    - towny.wild.build.83
    - towny.wild.build.86
    - towny.wild.build.103
    - towny.wild.build.111
    - towny.wild.build.115

  g:towny_admin:
    permissions:
    - towny.admin
    - -towny.wild.destroy.119
    - -towny.wild.destroy.120
    - towny.chat.admin

# Permission nodes for VanishNoPacket by mbaxter
# http://dev.bukkit.org/server-mods/vanish/

  g:vanish_moderator:
    permissions:
    - -vanish.*
    - vanish.vanish
    - vanish.smokin
    - vanish.nofollow
    - vanish.nopickup
    - vanish.preventincomingdamage
    - vanish.hooks.dynmap.alwayshidden
    - vanish.hooks.essentials.hide

  g:vanish_admin:
    permissions:
    - vanish.silentjoin
    - vanish.silentquit
    - vanish.silentchests
