Xenonauts 中文计划
==================

Xenonauts 是一个复刻 X-COM 的游戏 http://store.steampowered.com/app/223830/ 。官方没有中文版，但官方鼓励爱好者自己汉化。
参见官方论坛的翻译板块：http://www.goldhawkinteractive.com/forums/forumdisplay.php/18-Translation-Discussion

如果直接翻译英文 xml 文本，单个文本很大，不利于协同工作。所以在这个项目里，使用了一个简单的 Lua 脚本把原始文本拆分开，并提供一个脚本合并。

这里已经把 xenopedia.eng.xml 这个原始文本拆分到 xenopedia 目录下，可以独立翻译。

利用 
```
lua pack.lua xenopedia
```
可以合并成 xenopedia.chn.xml

-----
翻译的范例可以看 **冰岛事件** 。

在 xenopedia 目录下有一个 IcelandIncident.txt 文件，用文本编辑器打开后是这样的：

```xml
<index>IcelandIncident</index>
<name>Iceland Incident</name>
<cname>冰岛事件</cname>
<type>Extraterrestrials</type>
<ctype>外星人</ctype>
<desc>The 1958 Iceland Incident was our first contact with extraterrestrial life. An alien craft entered our atmosphere above the Atlantic in what we now believe was a scouting mission. It was detected and intercepted by NATO jets operating under the assumption it was an experimental Soviet aircraft.&#10;&#10;Visual sighting of the UFO rapidly dispelled that myth - the craft was far larger than its radar signature suggested, more akin to an airborne warship than an aircraft. Attempts to communicate elicited a barrage of energy weapon fire that disintegrated half of the squadron and left the remaining jets limping back to base with severe damage. Several subsequent attempts were made by NATO fighter squadrons to intercept the alien vessel, costing them a number of aircraft but inflicting no appreciable damage on the target. When the UFO abruptly changed course and began heading for the eastern coast of the United States, the decision was made to deploy nuclear weapons. &#10;&#10;Twenty minutes later, half a dozen nuclear-tipped ICBM ignited the sky above an uninhabited part of Iceland.  Astonishingly, the UFO survived the blast - but it crash-landed, almost intact, shortly afterwards. At this point, the NATO forces made the decision to inform their Soviet counterparts about the alien vessel and seek their assistance in securing the vessel and the technology within. This decision was seemingly motivated more by self-preservation rather than altruism; the Soviets were furious at the large unexplained nuclear detonations and were apparently close to launching missiles of their own.&#10;&#10;A joint ground operation was launched to capture the alien craft, but numerous extraterrestrials had survived the crash and put up stiff resistance. Human forces took significant losses during the operation, but slowly secured the area around the craft. What happened next is uncertain - all we know is that the alien craft was destroyed in an enormous explosion, almost certainly caused by the craft's power source. This explosion annihilated the UFO itself and wiped out all ground forces within a ten mile radius (the only survivors were those at the distant command post). There was nothing left; the UFO was gone and only a handful of those who had sighted an extraterrestrial were left alive.&#10;&#10;The aftermath of the Incident involved a large scale cover-up. The official explanation was that of a Soviet invasion of Iceland thwarted by nuclear weapons, with heavy losses on both sides. But behind closed doors, the two superpowers were collaborating - a joint black ops organisation was formed, drawing from the resources of both. Unofficially dubbed the &quot;Xenonauts&quot;, it was tasked with defending the planet against alien invasion. The absence of an obvious alien threat has made us look rather irrelevant for the past twenty years, Commander - but we had little doubt we would be needed some day. It seems that day has come.&#10;&#10;&lt;i&gt;(The free novella Xenonauts: Crimson Dagger tells the story of the Iceland Incident and is included with the game under the &quot;Extras&quot; button of the game launcher)&lt;/i&gt;</desc>
<cdesc>1958年冰岛事件是我们第一次接触地外生命。一艘外星飞船进入大西洋上空的大气层，现在我们确信那是一次侦察行动。它被北约的喷气机当成苏联的试验飞机侦察到并试图拦截。&#10;&#10;当看到ＵＦＯ后，立刻就明白了那并非是苏联飞机——飞行器远比在雷达上标记出来的大，更像是一艘空中战舰而不是飞船。在尝试于之沟通时对方开火摧毁了一半编队，剩下的编队损伤严重返回。接下来北约战斗机编队试图拦截下外星人飞船，花了不少飞机也没有对目标造成太大损伤。当ＵＦＯ突然改变航向开始驶向美国东海岸时，下达了部署核武器的决定。&#10;&#10;二十分钟后，半打带有核弹头的洲际弹道导弹射入冰岛无人区上空。令人惊讶地是，ＵＦＯ居然没被摧毁——不过随后就迫降了，几乎未受损。这时候，北约军方决定将外星飞船的事情通知苏联，寻求他们的帮助来搜寻外星飞船以及其中的科技。这个决定的动机更像是出于自卫意识而非利他；苏联人对大量不明原因的核爆炸非常愤怒，差点发射自己的导弹。&#10;&#10;接下来是一次联合地面行动搜捕外星飞船，但是遭到了在坠机中活下来的外星人的顽强抵抗。人类军队在行动中遭受了巨大的损失，但终于慢慢的控制了飞船周边地区。接下来发生的事情就不确定了——我们只知道外星飞船在一次剧烈的爆炸中被摧毁了，爆炸主要是由飞船的动力源导致的。这次爆炸覆没了ＵＦＯ并摧毁了半径十英里内的所有地面部队（只有那些在远方指挥所中的人幸存下来）。结果什么也没留下来；ＵＦＯ没了，只有屈指可数的几个地外生命的目击者。&#10;&#10; 事件的余波是大规模的掩盖。官方解释是苏联入侵冰岛，被核武器击败，双方都承受了惨重的损失。但关上门后，两大超级力量开始合作——一个联合黑色行动组织成立，双方都投入了资源。非正式的名称是“Xenonauts”，它的任务是抵抗外星人入侵保卫地球。在过去二十年里并没有出现明显的外星人威胁使得我们看起来无关紧要，指挥官——我们都有点怀疑是否真用得上我们。现在看起来这一天到了。&#10;&#10;&lt;i&gt;（免费的中篇小说 Xenonauts: 深红匕首讲述了冰岛事件的故事，它在游戏启动菜单的“Extras”按钮下&lt;/i&gt;。</cdesc>
```

其中 cname ctype cdesc 是对 name type desc 的翻译。对于没有翻译的文本，这三项是空的。需要做的就是逐个翻译这些 txt 文件。

协作
======

因为这个项目是大家协作，所以在自由选择自己想翻译的段落前，最后可以先看一下 pull requests 里有没有和其他人的冲突。

一般提交 PR 我会做一些简单的校对，提出个人意见，达成一致后才会合并。这里的时间差请考虑进去。

另外，尽量避免提交很大的 PR ，方便大家协作，和单独校对。

