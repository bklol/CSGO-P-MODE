# CSGO-P-MODE
CSGO 练习模式汉化插件

一般命令
.setup 显示练习模式菜单
.prac启动练习模式并显示.setup菜单
.help：显示此页面
.settings：打开客户端设置菜单
保存手榴弹位置
.nades [filter]：显示一个菜单，用于选择已保存的手榴弹位置。.nades不带参数将显示所有裸体。filter可以是以下各项之一：裸身ID，类别名称，玩家名称或手榴弹名称的一部分
.cats ：按类别显示所有已保存手榴弹的菜单
.save <name>：使用给定名称将当前位置保存为手榴弹位置
.goto <grenadeid>：将您传送到玩家已保存的手榴弹（如果未命名玩家，则为您自己的手榴弹）
.delete：删除您使用.goto（或.nades）传送到的最后一个手榴弹
.find <text>：在所有手榴弹名称中搜索文字匹配项
修改已保存的手榴弹
以下所有命令只能上使用您的手榴弹。他们将应用到你去的时候，无论是通过上次保存的手榴弹.save，.nades或.goto。
.desc <description>：在您的最后一个手榴弹中添加一个手榴弹描述
.rename <new name>：重命名您的最后一枚手榴弹
.addcat <category> ...：在您的最后一颗手榴弹上添加一个类别
.removecat <category>：从您的最后一颗手榴弹中删除一个类别
.clearcats：删除您最后一颗手榴弹上的所有类别
.deletecat <category>：从所有已保存的手榴弹中删除类别
.copy <username> <grenadeid>：复制其他用户的手榴弹并将其保存为您
.setdelay <delay>：设置您的最后一枚手榴弹的延迟时间。仅在对类别使用.throw时使用
测试手榴弹
.last：将你传送回你投掷最后一枚手榴弹的地方
.back：传送您回到手榴弹历史上的位置（例如，您也可以移动.back 5到投掷的第五枚手榴弹）
.forward：传送您在手榴弹历史上的位置
.flash：保存您的位置以对其进行测试。在您想致盲的地方使用此命令，然后移动并扔出闪光灯。您将被传送回该位置，并查看闪光灯的效果。使用.stop取消。
.throw [filter]：自动抛出所有与过滤器匹配的手榴弹。没有过滤器，投掷您投掷的最后一枚手榴弹。
.noflash：做到这一点，这样就不会有闪光弹会蒙蔽您（他们仍然蒙蔽其他人）
生成命令
.respawn：使您在站立的位置重生（.stop取消）
.spawn <number>：使用团队的出生点（CT或T）将您传送到出生点。如果没有给出参数，则使用最近的出生点
.ctspawn <number>：与.spawn相同，但无论您在哪个团队中，都仅使用CT
.tspawn <number>：与.spawn相同，但无论您在哪个团队中，都仅使用T
.namespawn <name>：使用名称保存最接近的出生点，然后可以通过 .spawn <name>
.bestspawn：将您从当前位置传送到团队最接近的出生点
.worstspawn：将您从当前位置传送到团队最远的出生点
Bot命令
.bots：打开机器人菜单，以便更轻松地访问以下大多数命令
.bot：在您站立（或蹲伏！）的地方添加一个机器人；.crouchbot强迫蹲伏机器人
.ctbot，.tbot：与相同.bot，但会迫使漫游器团队进入CT或T
.botplace：在您要查看的位置添加一个机器人（类似于bot_place命令）
.boost：产生一个机器人来助您一臂之力（如果您卧虎藏龙的话会大举提高）；.crouchboost强迫蹲伏机器人
.swapbot：与最近的漫游器交换您的位置（暂时，漫游器仍会在原始位置重新生成）
.movebot：将您放置的最后一个机器人移到当前位置
.nobot：删除您瞄准的机器人（也可以使用.kickbot或.removebot）
.nobots：清除所有机器人（.clearbots，.removebots，.kickbots也包括工作）
.savebots：将所有当前的机器人保存到文件中
.loadbots：从文件中加载机器人（由last编写.savebots）
杂项命令
.map：更改地图（您可以使用地图名称，例如.map de_dust2或仅.map用于获取菜单）
.dryrun：禁用大多数练习模式设置（保留无限量），重新开始轮次，并将冻结时间设置为sm_practicemode_dry_run_freeze_time（默认值6）-您也可以使用.dry
.savepos：暂时保存一个位置，以便您可以.back使用它（这会将位置添加到您抛出的手榴弹位置列表中）
.god：切换上帝模式（god控制台中命令的别名；要求打开sv_cheats）
.endround：结束回合（endround控制台中命令的别名；要求打开sv_cheats）
.break：破坏所有func_breakable实体（大多数窗口）
.stop：取消当前操作（这可以停止很多事情：.flash命令，.repeat命令和.timer命令）
.spec，.t，.ct：加入一个团队
Bot重播命令
.replays：打开重放模式菜单
.replay：打开重播模式菜单，或打开的上一个重播/角色菜单
.namereplay：命名您当前正在处理的重放
.namerole：命名您当前正在处理的角色
.finish：完成并保存当前记录
.cancel：取消当前的重放/记录
.play <id> [role]：播放重播ID（所有角色），或播放重播中的单个角色
