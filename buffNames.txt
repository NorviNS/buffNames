## 茗依插件buff数据（自存）
	整理By 双一纵月好看又彩笔的军娘-妄想言绫

### 操作
1. 打开茗依插件设置面板
2. 进入目标tab页面
3. 选择buff监控
4. 单击导入
5. 选择下方自己觉得有需要的代码复制粘贴导入

### buff配置说明
![image](http://ormehfj6q.bkt.clouddn.com/DA4FC426-0B18-4708-9C0A-7E99C9EBAF78.png)

### 插件效果说明
1. 在勾选了buff名称之后不知道为什么还是看不到buff名称，很迷，除非勾选倒计时条
2. 只能展示buff剩余时间，像山河这种每秒刷新的buff就会一直闪烁
3. 暂时不知道怎么监控重要技能cd

### buff代码
* 监控自身重要buff
	* 说明：这个建议根据自己需求，在插件界面手动加buff名称，这里只给个样例
	* 复制内容
		
	```
		{cdBarWidth=240,showBuffName=true,maxLineCount=16,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,caption="重要自身buff",hideVoidBuff=true,cdBar=false,hideOthers=true,anchor={y=261.54742431641,x=23.090599060059,s="LEFTCENTER",r="LEFTCENTER"},target="CLIENT_PLAYER",enable=true,monitors={[10026]={{iconid=13,buffname="疾如风",ids={},enable=true},{iconid=13,buffname="守如山",ids={},enable=true},{iconid=13,buffname="啸如虎",ids={},enable=true}}}}
		
	```
	
	
	* 预览

<pre>
	{
		cdBarWidth=240,
		showBuffName=true,
		maxLineCount=16,
		scale=1,
		boxBgUITex="UI/Image/Common/Box.UITex|44",
		cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
		dragable=true,
		caption="重要自身buff",
		hideVoidBuff=true,
		cdBar=false,
		hideOthers=true,
		anchor={
			y=261.54742431641,
			x=23.090599060059,
			s="LEFTCENTER",
			r="LEFTCENTER"
		},
		target="CLIENT_PLAYER",
		enable=true,
		monitors={
			[10026]={
				{iconid=13,buffname="疾如风",ids={},enable=true},
				{iconid=13,buffname="守如山",ids={},enable=true},
				{iconid=13,buffname="啸如虎",ids={},enable=true}
			}
		}
	}
</pre>

* 监控目标（一股脑儿全部有的版本）
	* 说明（一定要看！）
		* 这个数据有个问题，因为太太太长，所以黏贴进去会有系统卡顿，耐心等一下，如果本身电脑就很卡动不动死机的，放弃使用这个数据或者自己酌情删减
		* 这个数据强烈建议调整到合适的位置后，勾选【隐藏已消失buff】，否则你的界面会很可怕
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="无敌",showBuffName=true,monitors={common={{iconid=13,buffname="镇山河",ids={},enable=true},{iconid=13,buffname="太虚",ids={},enable=true},{iconid=13,buffname="回神",ids={},enable=true},{iconid=13,buffname="鬼斧神工",ids={},enable=true},{iconid=13,buffname="御",ids={},enable=true},{iconid=13,buffname="冥泽",ids={},enable=true},{iconid=13,buffname="散流霞",ids={},enable=true},{iconid=13,buffname="剑飞惊天",ids={},enable=true},{iconid=13,buffname="沉默",ids={},enable=true},{iconid=13,buffname="兰摧玉折",ids={},enable=true},{iconid=13,buffname="怖畏暗刑",ids={},enable=true},{iconid=13,buffname="雷云",ids={},enable=true},{iconid=13,buffname="井仪",ids={},enable=true},{iconid=13,buffname="余音",ids={},enable=true},{iconid=13,buffname="风切",ids={},enable=true},{iconid=13,buffname="星楼月影",ids={},enable=true},{iconid=13,buffname="折骨",ids={},enable=true},{iconid=13,buffname="素衿",ids={},enable=true},{iconid=13,buffname="力拔",ids={},enable=true},{iconid=13,buffname="纵轻骑",ids={},enable=true},{iconid=13,buffname="转乾坤",ids={},enable=true},{iconid=13,buffname="生死之交",ids={},enable=true},{iconid=13,buffname="不工",ids={},enable=true},{iconid=13,buffname="玉泉鱼跃",ids={},enable=true},{iconid=13,buffname="梦泉虎跑",ids={},enable=true},{iconid=13,buffname="蛊虫狂暴",ids={},enable=true},{iconid=13,buffname="风蜈献祭",ids={},enable=true},{iconid=13,buffname="碧蝶献祭",ids={},enable=true},{iconid=13,buffname="圣体",ids={},enable=true},{iconid=13,buffname="灵辉",ids={},enable=true},{iconid=13,buffname="超然",ids={},enable=true},{iconid=13,buffname="出渊",ids={},enable=true},{iconid=13,buffname="飞将",ids={},enable=true},{iconid=13,buffname="零落",ids={},enable=true},{iconid=13,buffname="吞日月",ids={},enable=true},{iconid=13,buffname="迷心蛊",ids={},enable=true},{iconid=13,buffname="菩提身",ids={},enable=true},{iconid=13,buffname="青阳",ids={},enable=true},{iconid=13,buffname="笑醉狂",ids={},enable=true},{iconid=13,buffname="烟雨行",ids={},enable=true},{iconid=13,buffname="龙跃于渊",ids={},enable=true},{iconid=13,buffname="酒中仙",ids={},enable=true},{iconid=13,buffname="流火飞星",ids={},enable=true},{iconid=13,buffname="霸体",ids={},enable=true},{iconid=13,buffname="蛊虫献祭",ids={},enable=true},{iconid=13,buffname="绝伦逸群",ids={},enable=true},{iconid=13,buffname="无惧",ids={},enable=true},{iconid=13,buffname="盾墙",ids={},enable=true},{iconid=13,buffname="千险",ids={},enable=true},{iconid=13,buffname="水月无间",ids={},enable=true},{iconid=13,buffname="劫化",ids={},enable=true},{iconid=13,buffname="盾毅",ids={},enable=true},{iconid=13,buffname="捍卫",ids={},enable=true},{iconid=13,buffname="青蒂",ids={},enable=true},{iconid=13,buffname="净果",ids={},enable=true},{iconid=13,buffname="捣衣",ids={},enable=true},{iconid=13,buffname="圣法光明",ids={},enable=true},{iconid=13,buffname="鹊踏枝",ids={},enable=true},{iconid=13,buffname="音韵",ids={},enable=true},{iconid=13,buffname="石间意",ids={},enable=true},{iconid=13,buffname="孤影",ids={},enable=true},{iconid=13,buffname="探梅",ids={},enable=true},{iconid=13,buffname="破重围",ids={},enable=true},{iconid=13,buffname="尘身",ids={},enable=true},{iconid=13,buffname="西楚悲歌",ids={},enable=true},{iconid=13,buffname="临渊蹈河",ids={},enable=true},{iconid=13,buffname="生太极",ids={},enable=true},{iconid=13,buffname="啸日",ids={},enable=true},{iconid=13,buffname="眩晕",ids={},enable=true},{iconid=13,buffname="致盲",ids={},enable=true},{iconid=13,buffname="五蕴皆空",ids={},enable=true},{iconid=13,buffname="繁音急节",ids={},enable=true},{iconid=13,buffname="大狮子吼",ids={},enable=true},{iconid=13,buffname="雷霆震怒",ids={},enable=true},{iconid=13,buffname="突",ids={},enable=true},{iconid=13,buffname="断魂刺",ids={},enable=true},{iconid=13,buffname="中注",ids={},enable=true},{iconid=13,buffname="醉月",ids={},enable=true},{iconid=13,buffname="鹤归孤山",ids={},enable=true},{iconid=13,buffname="碧王",ids={},enable=true},{iconid=13,buffname="峰插云景",ids={},enable=true},{iconid=13,buffname="日劫",ids={},enable=true},{iconid=13,buffname="无明魂锁",ids={},enable=true},{iconid=13,buffname="镇魔",ids={},enable=true},{iconid=13,buffname="幻光步",ids={},enable=true},{iconid=13,buffname="虎贲",ids={},enable=true},{iconid=13,buffname="弩击",ids={},enable=true},{iconid=13,buffname="善护",ids={},enable=true},{iconid=13,buffname="净世破魔击",ids={},enable=true},{iconid=13,buffname="醉逍遥",ids={},enable=true},{iconid=13,buffname="北斗",ids={},enable=true},{iconid=13,buffname="危楼",ids={},enable=true},{iconid=13,buffname="日影",ids={},enable=true},{iconid=13,buffname="伏夜·晕",ids={},enable=true},{iconid=13,buffname="撼地",ids={},enable=true},{iconid=13,buffname="盾毅",ids={},enable=true},{iconid=13,buffname="盾猛",ids={},enable=true},{iconid=13,buffname="裁骨",ids={},enable=true},{iconid=13,buffname="三才化生",ids={},enable=true},{iconid=13,buffname="影痕",ids={},enable=true},{iconid=13,buffname="止水",ids={},enable=true},{iconid=13,buffname="锁足",ids={},enable=true},{iconid=13,buffname="五方行尽",ids={},enable=true},{iconid=13,buffname="百足迷心",ids={},enable=true},{iconid=13,buffname="天蛛献祭",ids={},enable=true},{iconid=13,buffname="吐故纳新",ids={},enable=true},{iconid=13,buffname="滞",ids={},enable=true},{iconid=13,buffname="禁缚",ids={},enable=true},{iconid=13,buffname="太乙",ids={},enable=true},{iconid=13,buffname="百足",ids={},enable=true},{iconid=13,buffname="太阴指",ids={},enable=true},{iconid=13,buffname="碎冰",ids={},enable=true},{iconid=13,buffname="伏夜·缠",ids={},enable=true},{iconid=13,buffname="铁爪",ids={},enable=true},{iconid=13,buffname="落雁",ids={},enable=true},{iconid=13,buffname="断筋",ids={},enable=true},{iconid=13,buffname="钻心刺骨",ids={},enable=true},{iconid=13,buffname="剑·羽",ids={},enable=true},{iconid=13,buffname="钟林毓秀",ids={},enable=true},{iconid=13,buffname="琴音",ids={},enable=true},{iconid=13,buffname="太阴指",ids={},enable=true},{iconid=13,buffname="傍花随柳",ids={},enable=true},{iconid=13,buffname="帝骖龙翔",ids={},enable=true},{iconid=13,buffname="大道无术",ids={},enable=true},{iconid=13,buffname="七星拱瑞",ids={},enable=true},{iconid=13,buffname="芙蓉并蒂",ids={},enable=true},{iconid=13,buffname="完骨",ids={},enable=true},{iconid=13,buffname="破势",ids={},enable=true},{iconid=13,buffname="同归",ids={},enable=true},{iconid=13,buffname="定身",ids={},enable=true},{iconid=13,buffname="松涛",ids={},enable=true},{iconid=13,buffname="绛唇珠袖",ids={},enable=true},{iconid=13,buffname="丝牵",ids={},enable=true},{iconid=13,buffname="金针",ids={},enable=true},{iconid=13,buffname="天绝地灭",ids={},enable=true},{iconid=13,buffname="迷影",ids={},enable=true},{iconid=13,buffname="幻蛊",ids={},enable=true},{iconid=13,buffname="伏夜·定",ids={},enable=true},{iconid=13,buffname="疾如风",ids={},enable=true},{iconid=13,buffname="青荷",ids={},enable=true},{iconid=13,buffname="紫气东来",ids={},enable=true},{iconid=13,buffname="弱水",ids={},enable=true},{iconid=13,buffname="香疏影",ids={},enable=true},{iconid=13,buffname="乱洒",ids={},enable=true},{iconid=13,buffname="酒中仙",ids={},enable=true},{iconid=13,buffname="渊",ids={},enable=true},{iconid=13,buffname="莺鸣",ids={},enable=true},{iconid=13,buffname="扬威",ids={},enable=true},{iconid=13,buffname="灵蛇献祭",ids={},enable=true},{iconid=13,buffname="贯木流年",ids={},enable=true},{iconid=13,buffname="疏狂",ids={},enable=true},{iconid=13,buffname="重激",ids={},enable=true},{iconid=13,buffname="守如山",ids={},enable=true},{iconid=13,buffname="转乾坤",ids={},enable=true},{iconid=13,buffname="无相诀",ids={},enable=true},{iconid=13,buffname="春泥护花",ids={},enable=true},{iconid=13,buffname="雾体",ids={},enable=true},{iconid=13,buffname="御天",ids={},enable=true},{iconid=13,buffname="天地低昂",ids={},enable=true},{iconid=13,buffname="贪魔体",ids={},enable=true},{iconid=13,buffname="零落",ids={},enable=true},{iconid=13,buffname="正骨",ids={},enable=true},{iconid=13,buffname="玄水蛊",ids={},enable=true},{iconid=13,buffname="笑醉狂",ids={},enable=true},{iconid=13,buffname="脑户",ids={},enable=true},{iconid=13,buffname="龙啸九天",ids={},enable=true},{iconid=13,buffname="圣手织天",ids={},enable=true},{iconid=13,buffname="金屋",ids={},enable=true},{iconid=13,buffname="蝶戏水",ids={},enable=true},{iconid=13,buffname="护体",ids={},enable=true},{iconid=13,buffname="盾壁",ids={},enable=true},{iconid=13,buffname="盾墙",ids={},enable=true},{iconid=13,buffname="荣辉",ids={},enable=true},{iconid=13,buffname="盾护",ids={},enable=true},{iconid=13,buffname="捍卫",ids={},enable=true},{iconid=13,buffname="无我",ids={},enable=true},{iconid=13,buffname="绝歌",ids={},enable=true},{iconid=13,buffname="杯水留影",ids={},enable=true},{iconid=13,buffname="震八方",ids={},enable=true},{iconid=13,buffname="梅花三弄",ids={},enable=true},{iconid=13,buffname="破釜沉舟",ids={},enable=true},{iconid=13,buffname="惊鸿游龙",ids={},enable=true},{iconid=13,buffname="云栖松",ids={},enable=true},{iconid=13,buffname="风吹荷",ids={},enable=true},{iconid=13,buffname="醉逍遥",ids={},enable=true},{iconid=13,buffname="御风而行",ids={},enable=true},{iconid=13,buffname="两生",ids={},enable=true},{iconid=13,buffname="霹雳",ids={},enable=true},{iconid=13,buffname="穿心弩",ids={},enable=true},{iconid=13,buffname="穿心",ids={},enable=true},{iconid=13,buffname="无相",ids={},enable=true},{iconid=13,buffname="恒河劫沙",ids={},enable=true},{iconid=13,buffname="百足枯残",ids={},enable=true},{iconid=13,buffname="蝎蛰",ids={},enable=true},{iconid=13,buffname="月劫",ids={},enable=true},{iconid=13,buffname="神龙降世",ids={},enable=true},{iconid=13,buffname="盾击",ids={},enable=true},{iconid=13,buffname="楚济",ids={},enable=true},{iconid=13,buffname="吞楚",ids={},enable=true},{iconid=13,buffname="太乙",ids={},enable=true},{iconid=13,buffname="减速",ids={},enable=true},{iconid=13,buffname="穿",ids={},enable=true},{iconid=13,buffname="玄一",ids={},enable=true},{iconid=13,buffname="步迟",ids={},enable=true},{iconid=13,buffname="缠足",ids={},enable=true},{iconid=13,buffname="生太极",ids={},enable=true},{iconid=13,buffname="抱残式",ids={},enable=true},{iconid=13,buffname="少阳指",ids={},enable=true},{iconid=13,buffname="剑主天地",ids={},enable=true},{iconid=13,buffname="惊涛",ids={},enable=true},{iconid=13,buffname="千丝",ids={},enable=true},{iconid=13,buffname="冰封",ids={},enable=true},{iconid=13,buffname="毒蒺藜",ids={},enable=true},{iconid=13,buffname="业海罪缚",ids={},enable=true},{iconid=13,buffname="火舞长空",ids={},enable=true},{iconid=13,buffname="雪中行",ids={},enable=true},{iconid=13,buffname="业力",ids={},enable=true},{iconid=13,buffname="山阵",ids={},enable=true},{iconid=13,buffname="埋骨",ids={},enable=true},{iconid=13,buffname="暴雨梨花针",ids={},enable=true},{iconid=13,buffname="刖足",ids={},enable=true},{iconid=13,buffname="伏夜·缓",ids={},enable=true},{iconid=13,buffname="盾墙",ids={},enable=true},{iconid=13,buffname="卷云",ids={},enable=true},{iconid=13,buffname="难行",ids={},enable=true},{iconid=13,buffname="禁缚",ids={},enable=true},{iconid=13,buffname="轰雷",ids={},enable=true},{iconid=13,buffname="剑·宫",ids={},enable=true},{iconid=13,buffname="风入松",ids={},enable=true},{iconid=13,buffname="伏尘",ids={},enable=true},{iconid=13,buffname="击鼎",ids={},enable=true},{iconid=13,buffname="傍花随柳",ids={},enable=true},{iconid=13,buffname="龙魂",ids={},enable=true},{iconid=13,buffname="徐如林",ids={},enable=true},{iconid=13,buffname="啸如虎",ids={},enable=true},{iconid=13,buffname="声趣",ids={},enable=true},{iconid=13,buffname="倒地",ids={},enable=true},{iconid=13,buffname="无声",ids={},enable=true},{iconid=13,buffname="追命无声",ids={},enable=true},{iconid=13,buffname="圣月佑",ids={},enable=true},{iconid=13,buffname="虚回",ids={},enable=true},{iconid=13,buffname="风过无痕",ids={},enable=true},{iconid=13,buffname="临风",ids={},enable=true},{iconid=13,buffname="行气血",ids={},enable=true},{iconid=13,buffname="枭泣",ids={},enable=true},{iconid=13,buffname="鹰目",ids={},enable=true},{iconid=13,buffname="泉凝月",ids={},enable=true},{iconid=13,buffname="风虎",ids={},enable=true},{iconid=13,buffname="牧云",ids={},enable=true},{iconid=13,buffname="天地根",ids={},enable=true},{iconid=13,buffname="影捷",ids={},enable=true},{iconid=13,buffname="锋针",ids={},enable=true},{iconid=13,buffname="善护",ids={},enable=true},{iconid=13,buffname="雾外江山",ids={},enable=true},{iconid=13,buffname="雨集",ids={},enable=true},{iconid=13,buffname="恶狗拦路",ids={},enable=true},{iconid=13,buffname="冲阴阳",ids={},enable=true},{iconid=13,buffname="日月灵魂",ids={},enable=true},{iconid=13,buffname="日月同辉",ids={},enable=true},{iconid=13,buffname="女娲补天",ids={},enable=true},{iconid=13,buffname="罗汉金身",ids={},enable=true},{iconid=13,buffname="渊",ids={},enable=true},{iconid=13,buffname="荆天棘地",ids={},enable=true},{iconid=13,buffname="盾立",ids={},enable=true},{iconid=13,buffname="沃土",ids={},enable=true},{iconid=13,buffname="玉蟾献祭",ids={},enable=true},{iconid=13,buffname="急曲",ids={},enable=true},{iconid=13,buffname="叠刃",ids={},enable=true},{iconid=13,buffname="活祭",ids={},enable=true},{iconid=13,buffname="狂绝",ids={},enable=true},{iconid=13,buffname="盾飞",ids={},enable=true},{iconid=13,buffname="毫针",ids={},enable=true},{iconid=13,buffname="缓深",ids={},enable=true},{iconid=13,buffname="息疗",ids={},enable=true},{iconid=13,buffname="日月齐光",ids={},enable=true},{iconid=13,buffname="清歌",ids={},enable=true},{iconid=13,buffname="映日",ids={},enable=true},{iconid=13,buffname="平笃",ids={},enable=true},{iconid=13,buffname="江逐月天",ids={},enable=true},{iconid=13,buffname="超然物外",ids={},enable=true},{iconid=13,buffname="迴光",ids={},enable=true},{iconid=13,buffname="迴梦",ids={},enable=true},{iconid=13,buffname="放歌",ids={},enable=true},{iconid=13,buffname="扬旌沙场",ids={},enable=true},{iconid=13,buffname="风入松",ids={},enable=true},{iconid=13,buffname="梦未醒",ids={},enable=true},{iconid=13,buffname="啸吒",ids={},enable=true},{iconid=13,buffname="剑鸣",ids={},enable=true},{iconid=13,buffname="抢珠式",ids={},enable=true},{iconid=13,buffname="剑心通明",ids={},enable=true},{iconid=13,buffname="八卦洞玄",ids={},enable=true},{iconid=13,buffname="剑破虚空",ids={},enable=true},{iconid=13,buffname="梅花针",ids={},enable=true},{iconid=13,buffname="凄切",ids={},enable=true},{iconid=13,buffname="蟾啸迷心",ids={},enable=true},{iconid=13,buffname="清音长啸",ids={},enable=true},{iconid=13,buffname="苍龙",ids={},enable=true},{iconid=13,buffname="青君",ids={},enable=true},{iconid=13,buffname="千叶长生",ids={},enable=true},{iconid=13,buffname="碎魂",ids={},enable=true},{iconid=13,buffname="焚海",ids={},enable=true},{iconid=13,buffname="火龙沥泉",ids={},enable=true},{iconid=13,buffname="紫龙寂地",ids={},enable=true},{iconid=13,buffname="摧城",ids={},enable=true},{iconid=13,buffname="初尘",ids={},enable=true},{iconid=13,buffname="溯流",ids={},enable=true},{iconid=13,buffname="吞虹",ids={},enable=true},{iconid=13,buffname="碧落",ids={},enable=true},{iconid=13,buffname="断鬼",ids={},enable=true},{iconid=13,buffname="落凤",ids={},enable=true},{iconid=13,buffname="墨颠",ids={},enable=true},{iconid=13,buffname="吞吴",ids={},enable=true},{iconid=13,buffname="蛟影",ids={},enable=true},{iconid=13,buffname="雪名",ids={},enable=true},{iconid=13,buffname="周流星位",ids={},enable=true},{iconid=13,buffname="玉清玄明",ids={},enable=true},{iconid=13,buffname="留情",ids={},enable=true},{iconid=13,buffname="赤霄红莲",ids={},enable=true},{iconid=13,buffname="渊微指玄",ids={},enable=true},{iconid=13,buffname="幽月·乱花",ids={},enable=true},{iconid=13,buffname="赤练蓝翼",ids={},enable=true},{iconid=13,buffname="干将·莫邪",ids={},enable=true},{iconid=13,buffname="寒声·寂影",ids={},enable=true},{iconid=13,buffname="龙木金藤",ids={},enable=true},{iconid=13,buffname="白骨碎云",ids={},enable=true},{iconid=13,buffname="燃木",ids={},enable=true},{iconid=13,buffname="浮心·劫",ids={},enable=true},{iconid=13,buffname="白衣焚天",ids={},enable=true},{iconid=13,buffname="西天",ids={},enable=true},{iconid=13,buffname="莲心观佛",ids={},enable=true},{iconid=13,buffname="莲华·缘",ids={},enable=true},{iconid=13,buffname="织炎断尘",ids={},enable=true},{iconid=13,buffname="碧王",ids={},enable=true},{iconid=13,buffname="太阿",ids={},enable=true},{iconid=13,buffname="弱水",ids={},enable=true},{iconid=13,buffname="浴凰",ids={},enable=true},{iconid=13,buffname="青冥",ids={},enable=true},{iconid=13,buffname="太上忘情",ids={},enable=true},{iconid=13,buffname="绛玉拨云",ids={},enable=true},{iconid=13,buffname="地渊沉星",ids={},enable=true},{iconid=13,buffname="鸢翔天",ids={},enable=true},{iconid=13,buffname="凤尾天机",ids={},enable=true},{iconid=13,buffname="碎屏沉星",ids={},enable=true},{iconid=13,buffname="孔雀羽",ids={},enable=true},{iconid=13,buffname="含沙射影",ids={},enable=true},{iconid=13,buffname="摧山弩",ids={},enable=true},{iconid=13,buffname="造化异轨",ids={},enable=true},{iconid=13,buffname="火魂",ids={},enable=true},{iconid=13,buffname="悲魔饥火",ids={},enable=true},{iconid=13,buffname="明王镇狱",ids={},enable=true},{iconid=13,buffname="残月惊天",ids={},enable=true},{iconid=13,buffname="龙悔",ids={},enable=true},{iconid=13,buffname="浮沉照影",ids={},enable=true},{iconid=13,buffname="焚三世",ids={},enable=true},{iconid=13,buffname="执手",ids={},enable=true},{iconid=13,buffname="壶中乾坤",ids={},enable=true},{iconid=13,buffname="霜月明",ids={},enable=true},{iconid=13,buffname="炙狱邪龙",ids={},enable=true},{iconid=13,buffname="涯风嘲雨",ids={},enable=true},{iconid=13,buffname="血云",ids={},enable=true},{iconid=13,buffname="太初社稷",ids={},enable=true},{iconid=13,buffname="征天",ids={},enable=true},{iconid=13,buffname="题龙旐",ids={},enable=true},{iconid=13,buffname="千仞",ids={},enable=true},{iconid=13,buffname="旧嗜",ids={},enable=true},{iconid=13,buffname="朱轩怀雀",ids={},enable=true},{iconid=13,buffname="修罗鬼面",ids={},enable=true},{iconid=13,buffname="青玉流",ids={},enable=true},{iconid=13,buffname="洞仙引",ids={},enable=true},{iconid=13,buffname="盈缺",ids={},enable=true},{iconid=13,buffname="文姬泪",ids={},enable=true},{iconid=13,buffname="雨岩金莲",ids={},enable=true},{iconid=13,buffname="雪怒",ids={},enable=true},{iconid=13,buffname="血悲",ids={},enable=true},{iconid=13,buffname="新亭侯",ids={},enable=true},{iconid=13,buffname="吞日月",ids={},enable=true},{iconid=13,buffname="千丝迷心",ids={},enable=true},{iconid=13,buffname="迷幻",ids={},enable=true},{iconid=13,buffname="身乏",ids={},enable=true},{iconid=13,buffname="滞影",ids={},enable=true},{iconid=13,buffname="玳弦",ids={},enable=true},{iconid=13,buffname="云景",ids={},enable=true},{iconid=13,buffname="恶狗拦路",ids={},enable=true},{iconid=13,buffname="幻相",ids={},enable=true},{iconid=13,buffname="半步颠",ids={},enable=true},{iconid=13,buffname="步残",ids={},enable=true},{iconid=13,buffname="重围",ids={},enable=true},{iconid=13,buffname="行泽",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="无敌",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="镇山河",ids={},enable=true},
			{iconid=13,buffname="太虚",ids={},enable=true},
			{iconid=13,buffname="回神",ids={},enable=true},
			{iconid=13,buffname="鬼斧神工",ids={},enable=true},
			{iconid=13,buffname="御",ids={},enable=true},
			{iconid=13,buffname="冥泽",ids={},enable=true},
			{iconid=13,buffname="散流霞",ids={},enable=true},
			{iconid=13,buffname="剑飞惊天",ids={},enable=true},
			{iconid=13,buffname="沉默",ids={},enable=true},
			{iconid=13,buffname="兰摧玉折",ids={},enable=true},
			{iconid=13,buffname="怖畏暗刑",ids={},enable=true},
			{iconid=13,buffname="雷云",ids={},enable=true},
			{iconid=13,buffname="井仪",ids={},enable=true},
			{iconid=13,buffname="余音",ids={},enable=true},
			{iconid=13,buffname="风切",ids={},enable=true},
			{iconid=13,buffname="星楼月影",ids={},enable=true},
			{iconid=13,buffname="折骨",ids={},enable=true},
			{iconid=13,buffname="素衿",ids={},enable=true},
			{iconid=13,buffname="力拔",ids={},enable=true},
			{iconid=13,buffname="纵轻骑",ids={},enable=true},
			{iconid=13,buffname="转乾坤",ids={},enable=true},
			{iconid=13,buffname="生死之交",ids={},enable=true},
			{iconid=13,buffname="不工",ids={},enable=true},
			{iconid=13,buffname="玉泉鱼跃",ids={},enable=true},
			{iconid=13,buffname="梦泉虎跑",ids={},enable=true},
			{iconid=13,buffname="蛊虫狂暴",ids={},enable=true},
			{iconid=13,buffname="风蜈献祭",ids={},enable=true},
			{iconid=13,buffname="碧蝶献祭",ids={},enable=true},
			{iconid=13,buffname="圣体",ids={},enable=true},
			{iconid=13,buffname="灵辉",ids={},enable=true},
			{iconid=13,buffname="超然",ids={},enable=true},
			{iconid=13,buffname="出渊",ids={},enable=true},
			{iconid=13,buffname="飞将",ids={},enable=true},
			{iconid=13,buffname="零落",ids={},enable=true},
			{iconid=13,buffname="吞日月",ids={},enable=true},
			{iconid=13,buffname="迷心蛊",ids={},enable=true},
			{iconid=13,buffname="菩提身",ids={},enable=true},
			{iconid=13,buffname="青阳",ids={},enable=true},
			{iconid=13,buffname="笑醉狂",ids={},enable=true},
			{iconid=13,buffname="烟雨行",ids={},enable=true},
			{iconid=13,buffname="龙跃于渊",ids={},enable=true},
			{iconid=13,buffname="酒中仙",ids={},enable=true},
			{iconid=13,buffname="流火飞星",ids={},enable=true},
			{iconid=13,buffname="霸体",ids={},enable=true},
			{iconid=13,buffname="蛊虫献祭",ids={},enable=true},
			{iconid=13,buffname="绝伦逸群",ids={},enable=true},
			{iconid=13,buffname="无惧",ids={},enable=true},
			{iconid=13,buffname="盾墙",ids={},enable=true},
			{iconid=13,buffname="千险",ids={},enable=true},
			{iconid=13,buffname="水月无间",ids={},enable=true},
			{iconid=13,buffname="劫化",ids={},enable=true},
			{iconid=13,buffname="盾毅",ids={},enable=true},
			{iconid=13,buffname="捍卫",ids={},enable=true},
			{iconid=13,buffname="青蒂",ids={},enable=true},
			{iconid=13,buffname="净果",ids={},enable=true},
			{iconid=13,buffname="捣衣",ids={},enable=true},
			{iconid=13,buffname="圣法光明",ids={},enable=true},
			{iconid=13,buffname="鹊踏枝",ids={},enable=true},
			{iconid=13,buffname="音韵",ids={},enable=true},
			{iconid=13,buffname="石间意",ids={},enable=true},
			{iconid=13,buffname="孤影",ids={},enable=true},
			{iconid=13,buffname="探梅",ids={},enable=true},
			{iconid=13,buffname="破重围",ids={},enable=true},
			{iconid=13,buffname="尘身",ids={},enable=true},
			{iconid=13,buffname="西楚悲歌",ids={},enable=true},
			{iconid=13,buffname="临渊蹈河",ids={},enable=true},
			{iconid=13,buffname="生太极",ids={},enable=true},
			{iconid=13,buffname="啸日",ids={},enable=true},
			{iconid=13,buffname="眩晕",ids={},enable=true},
			{iconid=13,buffname="致盲",ids={},enable=true},
			{iconid=13,buffname="五蕴皆空",ids={},enable=true},
			{iconid=13,buffname="繁音急节",ids={},enable=true},
			{iconid=13,buffname="大狮子吼",ids={},enable=true},
			{iconid=13,buffname="雷霆震怒",ids={},enable=true},
			{iconid=13,buffname="突",ids={},enable=true},
			{iconid=13,buffname="断魂刺",ids={},enable=true},
			{iconid=13,buffname="中注",ids={},enable=true},
			{iconid=13,buffname="醉月",ids={},enable=true},
			{iconid=13,buffname="鹤归孤山",ids={},enable=true},
			{iconid=13,buffname="碧王",ids={},enable=true},
			{iconid=13,buffname="峰插云景",ids={},enable=true},
			{iconid=13,buffname="日劫",ids={},enable=true},
			{iconid=13,buffname="无明魂锁",ids={},enable=true},
			{iconid=13,buffname="镇魔",ids={},enable=true},
			{iconid=13,buffname="幻光步",ids={},enable=true},
			{iconid=13,buffname="虎贲",ids={},enable=true},
			{iconid=13,buffname="弩击",ids={},enable=true},
			{iconid=13,buffname="善护",ids={},enable=true},
			{iconid=13,buffname="净世破魔击",ids={},enable=true},
			{iconid=13,buffname="醉逍遥",ids={},enable=true},
			{iconid=13,buffname="北斗",ids={},enable=true},
			{iconid=13,buffname="危楼",ids={},enable=true},
			{iconid=13,buffname="日影",ids={},enable=true},
			{iconid=13,buffname="伏夜·晕",ids={},enable=true},
			{iconid=13,buffname="撼地",ids={},enable=true},
			{iconid=13,buffname="盾毅",ids={},enable=true},
			{iconid=13,buffname="盾猛",ids={},enable=true},
			{iconid=13,buffname="裁骨",ids={},enable=true},
			{iconid=13,buffname="三才化生",ids={},enable=true},
			{iconid=13,buffname="影痕",ids={},enable=true},
			{iconid=13,buffname="止水",ids={},enable=true},
			{iconid=13,buffname="锁足",ids={},enable=true},
			{iconid=13,buffname="五方行尽",ids={},enable=true},
			{iconid=13,buffname="百足迷心",ids={},enable=true},
			{iconid=13,buffname="天蛛献祭",ids={},enable=true},
			{iconid=13,buffname="吐故纳新",ids={},enable=true},
			{iconid=13,buffname="滞",ids={},enable=true},
			{iconid=13,buffname="禁缚",ids={},enable=true},
			{iconid=13,buffname="太乙",ids={},enable=true},
			{iconid=13,buffname="百足",ids={},enable=true},
			{iconid=13,buffname="太阴指",ids={},enable=true},
			{iconid=13,buffname="碎冰",ids={},enable=true},
			{iconid=13,buffname="伏夜·缠",ids={},enable=true},
			{iconid=13,buffname="铁爪",ids={},enable=true},
			{iconid=13,buffname="落雁",ids={},enable=true},
			{iconid=13,buffname="断筋",ids={},enable=true},
			{iconid=13,buffname="钻心刺骨",ids={},enable=true},
			{iconid=13,buffname="剑·羽",ids={},enable=true},
			{iconid=13,buffname="钟林毓秀",ids={},enable=true},
			{iconid=13,buffname="琴音",ids={},enable=true},
			{iconid=13,buffname="太阴指",ids={},enable=true},
			{iconid=13,buffname="傍花随柳",ids={},enable=true},
			{iconid=13,buffname="帝骖龙翔",ids={},enable=true},
			{iconid=13,buffname="大道无术",ids={},enable=true},
			{iconid=13,buffname="七星拱瑞",ids={},enable=true},
			{iconid=13,buffname="芙蓉并蒂",ids={},enable=true},
			{iconid=13,buffname="完骨",ids={},enable=true},
			{iconid=13,buffname="破势",ids={},enable=true},
			{iconid=13,buffname="同归",ids={},enable=true},
			{iconid=13,buffname="定身",ids={},enable=true},
			{iconid=13,buffname="松涛",ids={},enable=true},
			{iconid=13,buffname="绛唇珠袖",ids={},enable=true},
			{iconid=13,buffname="丝牵",ids={},enable=true},
			{iconid=13,buffname="金针",ids={},enable=true},
			{iconid=13,buffname="天绝地灭",ids={},enable=true},
			{iconid=13,buffname="迷影",ids={},enable=true},
			{iconid=13,buffname="幻蛊",ids={},enable=true},
			{iconid=13,buffname="伏夜·定",ids={},enable=true},
			{iconid=13,buffname="疾如风",ids={},enable=true},
			{iconid=13,buffname="青荷",ids={},enable=true},
			{iconid=13,buffname="紫气东来",ids={},enable=true},
			{iconid=13,buffname="弱水",ids={},enable=true},
			{iconid=13,buffname="香疏影",ids={},enable=true},
			{iconid=13,buffname="乱洒",ids={},enable=true},
			{iconid=13,buffname="酒中仙",ids={},enable=true},
			{iconid=13,buffname="渊",ids={},enable=true},
			{iconid=13,buffname="莺鸣",ids={},enable=true},
			{iconid=13,buffname="扬威",ids={},enable=true},
			{iconid=13,buffname="灵蛇献祭",ids={},enable=true},
			{iconid=13,buffname="贯木流年",ids={},enable=true},
			{iconid=13,buffname="疏狂",ids={},enable=true},
			{iconid=13,buffname="重激",ids={},enable=true},
			{iconid=13,buffname="守如山",ids={},enable=true},
			{iconid=13,buffname="转乾坤",ids={},enable=true},
			{iconid=13,buffname="无相诀",ids={},enable=true},
			{iconid=13,buffname="春泥护花",ids={},enable=true},
			{iconid=13,buffname="雾体",ids={},enable=true},
			{iconid=13,buffname="御天",ids={},enable=true},
			{iconid=13,buffname="天地低昂",ids={},enable=true},
			{iconid=13,buffname="贪魔体",ids={},enable=true},
			{iconid=13,buffname="零落",ids={},enable=true},
			{iconid=13,buffname="正骨",ids={},enable=true},
			{iconid=13,buffname="玄水蛊",ids={},enable=true},
			{iconid=13,buffname="笑醉狂",ids={},enable=true},
			{iconid=13,buffname="脑户",ids={},enable=true},
			{iconid=13,buffname="龙啸九天",ids={},enable=true},
			{iconid=13,buffname="圣手织天",ids={},enable=true},
			{iconid=13,buffname="金屋",ids={},enable=true},
			{iconid=13,buffname="蝶戏水",ids={},enable=true},
			{iconid=13,buffname="护体",ids={},enable=true},
			{iconid=13,buffname="盾壁",ids={},enable=true},
			{iconid=13,buffname="盾墙",ids={},enable=true},
			{iconid=13,buffname="荣辉",ids={},enable=true},
			{iconid=13,buffname="盾护",ids={},enable=true},
			{iconid=13,buffname="捍卫",ids={},enable=true},
			{iconid=13,buffname="无我",ids={},enable=true},
			{iconid=13,buffname="绝歌",ids={},enable=true},
			{iconid=13,buffname="杯水留影",ids={},enable=true},
			{iconid=13,buffname="震八方",ids={},enable=true},
			{iconid=13,buffname="梅花三弄",ids={},enable=true},
			{iconid=13,buffname="破釜沉舟",ids={},enable=true},
			{iconid=13,buffname="惊鸿游龙",ids={},enable=true},
			{iconid=13,buffname="云栖松",ids={},enable=true},
			{iconid=13,buffname="风吹荷",ids={},enable=true},
			{iconid=13,buffname="醉逍遥",ids={},enable=true},
			{iconid=13,buffname="御风而行",ids={},enable=true},
			{iconid=13,buffname="两生",ids={},enable=true},
			{iconid=13,buffname="霹雳",ids={},enable=true},
			{iconid=13,buffname="穿心弩",ids={},enable=true},
			{iconid=13,buffname="穿心",ids={},enable=true},
			{iconid=13,buffname="无相",ids={},enable=true},
			{iconid=13,buffname="恒河劫沙",ids={},enable=true},
			{iconid=13,buffname="百足枯残",ids={},enable=true},
			{iconid=13,buffname="蝎蛰",ids={},enable=true},
			{iconid=13,buffname="月劫",ids={},enable=true},
			{iconid=13,buffname="神龙降世",ids={},enable=true},
			{iconid=13,buffname="盾击",ids={},enable=true},
			{iconid=13,buffname="楚济",ids={},enable=true},
			{iconid=13,buffname="吞楚",ids={},enable=true},
			{iconid=13,buffname="太乙",ids={},enable=true},
			{iconid=13,buffname="减速",ids={},enable=true},
			{iconid=13,buffname="穿",ids={},enable=true},
			{iconid=13,buffname="玄一",ids={},enable=true},
			{iconid=13,buffname="步迟",ids={},enable=true},
			{iconid=13,buffname="缠足",ids={},enable=true},
			{iconid=13,buffname="生太极",ids={},enable=true},
			{iconid=13,buffname="抱残式",ids={},enable=true},
			{iconid=13,buffname="少阳指",ids={},enable=true},
			{iconid=13,buffname="剑主天地",ids={},enable=true},
			{iconid=13,buffname="惊涛",ids={},enable=true},
			{iconid=13,buffname="千丝",ids={},enable=true},
			{iconid=13,buffname="冰封",ids={},enable=true},
			{iconid=13,buffname="毒蒺藜",ids={},enable=true},
			{iconid=13,buffname="业海罪缚",ids={},enable=true},
			{iconid=13,buffname="火舞长空",ids={},enable=true},
			{iconid=13,buffname="雪中行",ids={},enable=true},
			{iconid=13,buffname="业力",ids={},enable=true},
			{iconid=13,buffname="山阵",ids={},enable=true},
			{iconid=13,buffname="埋骨",ids={},enable=true},
			{iconid=13,buffname="暴雨梨花针",ids={},enable=true},
			{iconid=13,buffname="刖足",ids={},enable=true},
			{iconid=13,buffname="伏夜·缓",ids={},enable=true},
			{iconid=13,buffname="盾墙",ids={},enable=true},
			{iconid=13,buffname="卷云",ids={},enable=true},
			{iconid=13,buffname="难行",ids={},enable=true},
			{iconid=13,buffname="禁缚",ids={},enable=true},
			{iconid=13,buffname="轰雷",ids={},enable=true},
			{iconid=13,buffname="剑·宫",ids={},enable=true},
			{iconid=13,buffname="风入松",ids={},enable=true},
			{iconid=13,buffname="伏尘",ids={},enable=true},
			{iconid=13,buffname="击鼎",ids={},enable=true},
			{iconid=13,buffname="傍花随柳",ids={},enable=true},
			{iconid=13,buffname="龙魂",ids={},enable=true},
			{iconid=13,buffname="徐如林",ids={},enable=true},
			{iconid=13,buffname="啸如虎",ids={},enable=true},
			{iconid=13,buffname="声趣",ids={},enable=true},
			{iconid=13,buffname="倒地",ids={},enable=true},
			{iconid=13,buffname="无声",ids={},enable=true},
			{iconid=13,buffname="追命无声",ids={},enable=true},
			{iconid=13,buffname="圣月佑",ids={},enable=true},
			{iconid=13,buffname="虚回",ids={},enable=true},
			{iconid=13,buffname="风过无痕",ids={},enable=true},
			{iconid=13,buffname="临风",ids={},enable=true},
			{iconid=13,buffname="行气血",ids={},enable=true},
			{iconid=13,buffname="枭泣",ids={},enable=true},
			{iconid=13,buffname="鹰目",ids={},enable=true},
			{iconid=13,buffname="泉凝月",ids={},enable=true},
			{iconid=13,buffname="风虎",ids={},enable=true},
			{iconid=13,buffname="牧云",ids={},enable=true},
			{iconid=13,buffname="天地根",ids={},enable=true},
			{iconid=13,buffname="影捷",ids={},enable=true},
			{iconid=13,buffname="锋针",ids={},enable=true},
			{iconid=13,buffname="善护",ids={},enable=true},
			{iconid=13,buffname="雾外江山",ids={},enable=true},
			{iconid=13,buffname="雨集",ids={},enable=true},
			{iconid=13,buffname="恶狗拦路",ids={},enable=true},
			{iconid=13,buffname="冲阴阳",ids={},enable=true},
			{iconid=13,buffname="日月灵魂",ids={},enable=true},
			{iconid=13,buffname="日月同辉",ids={},enable=true},
			{iconid=13,buffname="女娲补天",ids={},enable=true},
			{iconid=13,buffname="罗汉金身",ids={},enable=true},
			{iconid=13,buffname="渊",ids={},enable=true},
			{iconid=13,buffname="荆天棘地",ids={},enable=true},
			{iconid=13,buffname="盾立",ids={},enable=true},
			{iconid=13,buffname="沃土",ids={},enable=true},
			{iconid=13,buffname="玉蟾献祭",ids={},enable=true},
			{iconid=13,buffname="急曲",ids={},enable=true},
			{iconid=13,buffname="叠刃",ids={},enable=true},
			{iconid=13,buffname="活祭",ids={},enable=true},
			{iconid=13,buffname="狂绝",ids={},enable=true},
			{iconid=13,buffname="盾飞",ids={},enable=true},
			{iconid=13,buffname="毫针",ids={},enable=true},
			{iconid=13,buffname="缓深",ids={},enable=true},
			{iconid=13,buffname="息疗",ids={},enable=true},
			{iconid=13,buffname="日月齐光",ids={},enable=true},
			{iconid=13,buffname="清歌",ids={},enable=true},
			{iconid=13,buffname="映日",ids={},enable=true},
			{iconid=13,buffname="平笃",ids={},enable=true},
			{iconid=13,buffname="江逐月天",ids={},enable=true},
			{iconid=13,buffname="超然物外",ids={},enable=true},
			{iconid=13,buffname="迴光",ids={},enable=true},
			{iconid=13,buffname="迴梦",ids={},enable=true},
			{iconid=13,buffname="放歌",ids={},enable=true},
			{iconid=13,buffname="扬旌沙场",ids={},enable=true},
			{iconid=13,buffname="风入松",ids={},enable=true},
			{iconid=13,buffname="梦未醒",ids={},enable=true},
			{iconid=13,buffname="啸吒",ids={},enable=true},
			{iconid=13,buffname="剑鸣",ids={},enable=true},
			{iconid=13,buffname="抢珠式",ids={},enable=true},
			{iconid=13,buffname="剑心通明",ids={},enable=true},
			{iconid=13,buffname="八卦洞玄",ids={},enable=true},
			{iconid=13,buffname="剑破虚空",ids={},enable=true},
			{iconid=13,buffname="梅花针",ids={},enable=true},
			{iconid=13,buffname="凄切",ids={},enable=true},
			{iconid=13,buffname="蟾啸迷心",ids={},enable=true},
			{iconid=13,buffname="清音长啸",ids={},enable=true},
			{iconid=13,buffname="苍龙",ids={},enable=true},
			{iconid=13,buffname="青君",ids={},enable=true},
			{iconid=13,buffname="千叶长生",ids={},enable=true},
			{iconid=13,buffname="碎魂",ids={},enable=true},
			{iconid=13,buffname="焚海",ids={},enable=true},
			{iconid=13,buffname="火龙沥泉",ids={},enable=true},
			{iconid=13,buffname="紫龙寂地",ids={},enable=true},
			{iconid=13,buffname="摧城",ids={},enable=true},
			{iconid=13,buffname="初尘",ids={},enable=true},
			{iconid=13,buffname="溯流",ids={},enable=true},
			{iconid=13,buffname="吞虹",ids={},enable=true},
			{iconid=13,buffname="碧落",ids={},enable=true},
			{iconid=13,buffname="断鬼",ids={},enable=true},
			{iconid=13,buffname="落凤",ids={},enable=true},
			{iconid=13,buffname="墨颠",ids={},enable=true},
			{iconid=13,buffname="吞吴",ids={},enable=true},
			{iconid=13,buffname="蛟影",ids={},enable=true},
			{iconid=13,buffname="雪名",ids={},enable=true},
			{iconid=13,buffname="周流星位",ids={},enable=true},
			{iconid=13,buffname="玉清玄明",ids={},enable=true},
			{iconid=13,buffname="留情",ids={},enable=true},
			{iconid=13,buffname="赤霄红莲",ids={},enable=true},
			{iconid=13,buffname="渊微指玄",ids={},enable=true},
			{iconid=13,buffname="幽月·乱花",ids={},enable=true},
			{iconid=13,buffname="赤练蓝翼",ids={},enable=true},
			{iconid=13,buffname="干将·莫邪",ids={},enable=true},
			{iconid=13,buffname="寒声·寂影",ids={},enable=true},
			{iconid=13,buffname="龙木金藤",ids={},enable=true},
			{iconid=13,buffname="白骨碎云",ids={},enable=true},
			{iconid=13,buffname="燃木",ids={},enable=true},
			{iconid=13,buffname="浮心·劫",ids={},enable=true},
			{iconid=13,buffname="白衣焚天",ids={},enable=true},
			{iconid=13,buffname="西天",ids={},enable=true},
			{iconid=13,buffname="莲心观佛",ids={},enable=true},
			{iconid=13,buffname="莲华·缘",ids={},enable=true},
			{iconid=13,buffname="织炎断尘",ids={},enable=true},
			{iconid=13,buffname="碧王",ids={},enable=true},
			{iconid=13,buffname="太阿",ids={},enable=true},
			{iconid=13,buffname="弱水",ids={},enable=true},
			{iconid=13,buffname="浴凰",ids={},enable=true},
			{iconid=13,buffname="青冥",ids={},enable=true},
			{iconid=13,buffname="太上忘情",ids={},enable=true},
			{iconid=13,buffname="绛玉拨云",ids={},enable=true},
			{iconid=13,buffname="地渊沉星",ids={},enable=true},
			{iconid=13,buffname="鸢翔天",ids={},enable=true},
			{iconid=13,buffname="凤尾天机",ids={},enable=true},
			{iconid=13,buffname="碎屏沉星",ids={},enable=true},
			{iconid=13,buffname="孔雀羽",ids={},enable=true},
			{iconid=13,buffname="含沙射影",ids={},enable=true},
			{iconid=13,buffname="摧山弩",ids={},enable=true},
			{iconid=13,buffname="造化异轨",ids={},enable=true},
			{iconid=13,buffname="火魂",ids={},enable=true},
			{iconid=13,buffname="悲魔饥火",ids={},enable=true},
			{iconid=13,buffname="明王镇狱",ids={},enable=true},
			{iconid=13,buffname="残月惊天",ids={},enable=true},
			{iconid=13,buffname="龙悔",ids={},enable=true},
			{iconid=13,buffname="浮沉照影",ids={},enable=true},
			{iconid=13,buffname="焚三世",ids={},enable=true},
			{iconid=13,buffname="执手",ids={},enable=true},
			{iconid=13,buffname="壶中乾坤",ids={},enable=true},
			{iconid=13,buffname="霜月明",ids={},enable=true},
			{iconid=13,buffname="炙狱邪龙",ids={},enable=true},
			{iconid=13,buffname="涯风嘲雨",ids={},enable=true},
			{iconid=13,buffname="血云",ids={},enable=true},
			{iconid=13,buffname="太初社稷",ids={},enable=true},
			{iconid=13,buffname="征天",ids={},enable=true},
			{iconid=13,buffname="题龙旐",ids={},enable=true},
			{iconid=13,buffname="千仞",ids={},enable=true},
			{iconid=13,buffname="旧嗜",ids={},enable=true},
			{iconid=13,buffname="朱轩怀雀",ids={},enable=true},
			{iconid=13,buffname="修罗鬼面",ids={},enable=true},
			{iconid=13,buffname="青玉流",ids={},enable=true},
			{iconid=13,buffname="洞仙引",ids={},enable=true},
			{iconid=13,buffname="盈缺",ids={},enable=true},
			{iconid=13,buffname="文姬泪",ids={},enable=true},
			{iconid=13,buffname="雨岩金莲",ids={},enable=true},
			{iconid=13,buffname="雪怒",ids={},enable=true},
			{iconid=13,buffname="血悲",ids={},enable=true},
			{iconid=13,buffname="新亭侯",ids={},enable=true},
			{iconid=13,buffname="吞日月",ids={},enable=true},
			{iconid=13,buffname="千丝迷心",ids={},enable=true},
			{iconid=13,buffname="迷幻",ids={},enable=true},
			{iconid=13,buffname="身乏",ids={},enable=true},
			{iconid=13,buffname="滞影",ids={},enable=true},
			{iconid=13,buffname="玳弦",ids={},enable=true},
			{iconid=13,buffname="云景",ids={},enable=true},
			{iconid=13,buffname="恶狗拦路",ids={},enable=true},
			{iconid=13,buffname="幻相",ids={},enable=true},
			{iconid=13,buffname="半步颠",ids={},enable=true},
			{iconid=13,buffname="步残",ids={},enable=true},
			{iconid=13,buffname="重围",ids={},enable=true},
			{iconid=13,buffname="行泽",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标无敌
	* 复制内容
		
	```

		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="无敌",showBuffName=true,monitors={common={{iconid=13,buffname="镇山河",ids={},enable=true},{iconid=13,buffname="太虚",ids={},enable=true},{iconid=13,buffname="回神",ids={},enable=true},{iconid=13,buffname="鬼斧神工",ids={},enable=true},{iconid=13,buffname="御",ids={},enable=true},{iconid=13,buffname="冥泽",ids={},enable=true},{iconid=13,buffname="散流霞",ids={},enable=true}}}}
	
	```
		
	* 预览

<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="无敌",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="镇山河",ids={},enable=true},
			{iconid=13,buffname="太虚",ids={},enable=true},
			{iconid=13,buffname="回神",ids={},enable=true},
			{iconid=13,buffname="鬼斧神工",ids={},enable=true},
			{iconid=13,buffname="御",ids={},enable=true},
			{iconid=13,buffname="冥泽",ids={},enable=true},
			{iconid=13,buffname="散流霞",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标沉默
	* 复制内容
		
	```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="沉默",showBuffName=true,monitors={common={{iconid=13,buffname="剑飞惊天",ids={},enable=true},{iconid=13,buffname="沉默",ids={},enable=true},{iconid=13,buffname="兰摧玉折",ids={},enable=true},{iconid=13,buffname="怖畏暗刑",ids={},enable=true},{iconid=13,buffname="雷云",ids={},enable=true},{iconid=13,buffname="井仪",ids={},enable=true},{iconid=13,buffname="余音",ids={},enable=true},{iconid=13,buffname="风切",ids={},enable=true}}}}
		
	```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="沉默",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="剑飞惊天",ids={},enable=true},
			{iconid=13,buffname="沉默",ids={},enable=true},
			{iconid=13,buffname="兰摧玉折",ids={},enable=true},
			{iconid=13,buffname="怖畏暗刑",ids={},enable=true},
			{iconid=13,buffname="雷云",ids={},enable=true},
			{iconid=13,buffname="井仪",ids={},enable=true},
			{iconid=13,buffname="余音",ids={},enable=true},
			{iconid=13,buffname="风切",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标免控
	* 复制内容
		
	```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="沉默",showBuffName=true,monitors={common={{iconid=13,buffname="星楼月影",ids={},enable=true},{iconid=13,buffname="折骨",ids={},enable=true},{iconid=13,buffname="素衿",ids={},enable=true},{iconid=13,buffname="力拔",ids={},enable=true},{iconid=13,buffname="纵轻骑",ids={},enable=true},{iconid=13,buffname="转乾坤",ids={},enable=true},{iconid=13,buffname="生死之交",ids={},enable=true},{iconid=13,buffname="不工",ids={},enable=true},{iconid=13,buffname="玉泉鱼跃",ids={},enable=true},{iconid=13,buffname="梦泉虎跑",ids={},enable=true},{iconid=13,buffname="蛊虫狂暴",ids={},enable=true},{iconid=13,buffname="风蜈献祭",ids={},enable=true},{iconid=13,buffname="碧蝶献祭",ids={},enable=true},{iconid=13,buffname="圣体",ids={},enable=true},{iconid=13,buffname="灵辉",ids={},enable=true},{iconid=13,buffname="超然",ids={},enable=true},{iconid=13,buffname="出渊",ids={},enable=true},{iconid=13,buffname="飞将",ids={},enable=true},{iconid=13,buffname="零落",ids={},enable=true},{iconid=13,buffname="吞日月",ids={},enable=true},{iconid=13,buffname="迷心蛊",ids={},enable=true},{iconid=13,buffname="菩提身",ids={},enable=true},{iconid=13,buffname="青阳",ids={},enable=true},{iconid=13,buffname="笑醉狂",ids={},enable=true},{iconid=13,buffname="烟雨行",ids={},enable=true},{iconid=13,buffname="龙跃于渊",ids={},enable=true},{iconid=13,buffname="酒中仙",ids={},enable=true},{iconid=13,buffname="流火飞星",ids={},enable=true},{iconid=13,buffname="霸体",ids={},enable=true},{iconid=13,buffname="蛊虫献祭",ids={},enable=true},{iconid=13,buffname="绝伦逸群",ids={},enable=true},{iconid=13,buffname="无惧",ids={},enable=true},{iconid=13,buffname="盾墙",ids={},enable=true},{iconid=13,buffname="千险",ids={},enable=true},{iconid=13,buffname="水月无间",ids={},enable=true},{iconid=13,buffname="劫化",ids={},enable=true},{iconid=13,buffname="盾毅",ids={},enable=true},{iconid=13,buffname="捍卫",ids={},enable=true},{iconid=13,buffname="青蒂",ids={},enable=true},{iconid=13,buffname="净果",ids={},enable=true},{iconid=13,buffname="捣衣",ids={},enable=true},{iconid=13,buffname="圣法光明",ids={},enable=true},{iconid=13,buffname="鹊踏枝",ids={},enable=true},{iconid=13,buffname="音韵",ids={},enable=true},{iconid=13,buffname="石间意",ids={},enable=true},{iconid=13,buffname="孤影",ids={},enable=true},{iconid=13,buffname="探梅",ids={},enable=true},{iconid=13,buffname="破重围",ids={},enable=true},{iconid=13,buffname="尘身",ids={},enable=true},{iconid=13,buffname="西楚悲歌",ids={},enable=true},{iconid=13,buffname="临渊蹈河",ids={},enable=true},{iconid=13,buffname="生太极",ids={},enable=true},{iconid=13,buffname="啸日",ids={},enable=true}}}}
		
	```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="沉默",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="星楼月影",ids={},enable=true},
			{iconid=13,buffname="折骨",ids={},enable=true},
			{iconid=13,buffname="素衿",ids={},enable=true},
			{iconid=13,buffname="力拔",ids={},enable=true},
			{iconid=13,buffname="纵轻骑",ids={},enable=true},
			{iconid=13,buffname="转乾坤",ids={},enable=true},
			{iconid=13,buffname="生死之交",ids={},enable=true},
			{iconid=13,buffname="不工",ids={},enable=true},
			{iconid=13,buffname="玉泉鱼跃",ids={},enable=true},
			{iconid=13,buffname="梦泉虎跑",ids={},enable=true},
			{iconid=13,buffname="蛊虫狂暴",ids={},enable=true},
			{iconid=13,buffname="风蜈献祭",ids={},enable=true},
			{iconid=13,buffname="碧蝶献祭",ids={},enable=true},
			{iconid=13,buffname="圣体",ids={},enable=true},
			{iconid=13,buffname="灵辉",ids={},enable=true},
			{iconid=13,buffname="超然",ids={},enable=true},
			{iconid=13,buffname="出渊",ids={},enable=true},
			{iconid=13,buffname="飞将",ids={},enable=true},
			{iconid=13,buffname="零落",ids={},enable=true},
			{iconid=13,buffname="吞日月",ids={},enable=true},
			{iconid=13,buffname="迷心蛊",ids={},enable=true},
			{iconid=13,buffname="菩提身",ids={},enable=true},
			{iconid=13,buffname="青阳",ids={},enable=true},
			{iconid=13,buffname="笑醉狂",ids={},enable=true},
			{iconid=13,buffname="烟雨行",ids={},enable=true},
			{iconid=13,buffname="龙跃于渊",ids={},enable=true},
			{iconid=13,buffname="酒中仙",ids={},enable=true},
			{iconid=13,buffname="流火飞星",ids={},enable=true},
			{iconid=13,buffname="霸体",ids={},enable=true},
			{iconid=13,buffname="蛊虫献祭",ids={},enable=true},
			{iconid=13,buffname="绝伦逸群",ids={},enable=true},
			{iconid=13,buffname="无惧",ids={},enable=true},
			{iconid=13,buffname="盾墙",ids={},enable=true},
			{iconid=13,buffname="千险",ids={},enable=true},
			{iconid=13,buffname="水月无间",ids={},enable=true},
			{iconid=13,buffname="劫化",ids={},enable=true},
			{iconid=13,buffname="盾毅",ids={},enable=true},
			{iconid=13,buffname="捍卫",ids={},enable=true},
			{iconid=13,buffname="青蒂",ids={},enable=true},
			{iconid=13,buffname="净果",ids={},enable=true},
			{iconid=13,buffname="捣衣",ids={},enable=true},
			{iconid=13,buffname="圣法光明",ids={},enable=true},
			{iconid=13,buffname="鹊踏枝",ids={},enable=true},
			{iconid=13,buffname="音韵",ids={},enable=true},
			{iconid=13,buffname="石间意",ids={},enable=true},
			{iconid=13,buffname="孤影",ids={},enable=true},
			{iconid=13,buffname="探梅",ids={},enable=true},
			{iconid=13,buffname="破重围",ids={},enable=true},
			{iconid=13,buffname="尘身",ids={},enable=true},
			{iconid=13,buffname="西楚悲歌",ids={},enable=true},
			{iconid=13,buffname="临渊蹈河",ids={},enable=true},
			{iconid=13,buffname="生太极",ids={},enable=true},
			{iconid=13,buffname="啸日",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标眩晕
	* 复制内容
		
	```
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="眩晕",showBuffName=true,monitors={common={{iconid=13,buffname="眩晕",ids={},enable=true},{iconid=13,buffname="致盲",ids={},enable=true},{iconid=13,buffname="五蕴皆空",ids={},enable=true},{iconid=13,buffname="繁音急节",ids={},enable=true},{iconid=13,buffname="大狮子吼",ids={},enable=true},{iconid=13,buffname="雷霆震怒",ids={},enable=true},{iconid=13,buffname="突",ids={},enable=true},{iconid=13,buffname="断魂刺",ids={},enable=true},{iconid=13,buffname="中注",ids={},enable=true},{iconid=13,buffname="醉月",ids={},enable=true},{iconid=13,buffname="鹤归孤山",ids={},enable=true},{iconid=13,buffname="碧王",ids={},enable=true},{iconid=13,buffname="峰插云景",ids={},enable=true},{iconid=13,buffname="日劫",ids={},enable=true},{iconid=13,buffname="无明魂锁",ids={},enable=true},{iconid=13,buffname="镇魔",ids={},enable=true},{iconid=13,buffname="幻光步",ids={},enable=true},{iconid=13,buffname="虎贲",ids={},enable=true},{iconid=13,buffname="弩击",ids={},enable=true},{iconid=13,buffname="善护",ids={},enable=true},{iconid=13,buffname="净世破魔击",ids={},enable=true},{iconid=13,buffname="醉逍遥",ids={},enable=true},{iconid=13,buffname="北斗",ids={},enable=true},{iconid=13,buffname="危楼",ids={},enable=true},{iconid=13,buffname="日影",ids={},enable=true},{iconid=13,buffname="伏夜·晕",ids={},enable=true},{iconid=13,buffname="撼地",ids={},enable=true},{iconid=13,buffname="盾毅",ids={},enable=true},{iconid=13,buffname="盾猛",ids={},enable=true},{iconid=13,buffname="裁骨",ids={},enable=true}}}}
		
	```
	
	

	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="眩晕",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="眩晕",ids={},enable=true},
			{iconid=13,buffname="致盲",ids={},enable=true},
			{iconid=13,buffname="五蕴皆空",ids={},enable=true},
			{iconid=13,buffname="繁音急节",ids={},enable=true},
			{iconid=13,buffname="大狮子吼",ids={},enable=true},
			{iconid=13,buffname="雷霆震怒",ids={},enable=true},
			{iconid=13,buffname="突",ids={},enable=true},
			{iconid=13,buffname="断魂刺",ids={},enable=true},
			{iconid=13,buffname="中注",ids={},enable=true},
			{iconid=13,buffname="醉月",ids={},enable=true},
			{iconid=13,buffname="鹤归孤山",ids={},enable=true},
			{iconid=13,buffname="碧王",ids={},enable=true},
			{iconid=13,buffname="峰插云景",ids={},enable=true},
			{iconid=13,buffname="日劫",ids={},enable=true},
			{iconid=13,buffname="无明魂锁",ids={},enable=true},
			{iconid=13,buffname="镇魔",ids={},enable=true},
			{iconid=13,buffname="幻光步",ids={},enable=true},
			{iconid=13,buffname="虎贲",ids={},enable=true},
			{iconid=13,buffname="弩击",ids={},enable=true},
			{iconid=13,buffname="善护",ids={},enable=true},
			{iconid=13,buffname="净世破魔击",ids={},enable=true},
			{iconid=13,buffname="醉逍遥",ids={},enable=true},
			{iconid=13,buffname="北斗",ids={},enable=true},
			{iconid=13,buffname="危楼",ids={},enable=true},
			{iconid=13,buffname="日影",ids={},enable=true},
			{iconid=13,buffname="伏夜·晕",ids={},enable=true},
			{iconid=13,buffname="撼地",ids={},enable=true},
			{iconid=13,buffname="盾毅",ids={},enable=true},
			{iconid=13,buffname="盾猛",ids={},enable=true},
			{iconid=13,buffname="裁骨",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标锁足
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="锁足",showBuffName=true,monitors={common={{iconid=13,buffname="三才化生",ids={},enable=true},{iconid=13,buffname="影痕",ids={},enable=true},{iconid=13,buffname="止水",ids={},enable=true},{iconid=13,buffname="锁足",ids={},enable=true},{iconid=13,buffname="五方行尽",ids={},enable=true},{iconid=13,buffname="百足迷心",ids={},enable=true},{iconid=13,buffname="天蛛献祭",ids={},enable=true},{iconid=13,buffname="吐故纳新",ids={},enable=true},{iconid=13,buffname="滞",ids={},enable=true},{iconid=13,buffname="禁缚",ids={},enable=true},{iconid=13,buffname="太乙",ids={},enable=true},{iconid=13,buffname="百足",ids={},enable=true},{iconid=13,buffname="太阴指",ids={},enable=true},{iconid=13,buffname="碎冰",ids={},enable=true},{iconid=13,buffname="伏夜·缠",ids={},enable=true},{iconid=13,buffname="铁爪",ids={},enable=true},{iconid=13,buffname="落雁",ids={},enable=true},{iconid=13,buffname="断筋",ids={},enable=true},{iconid=13,buffname="钻心刺骨",ids={},enable=true},{iconid=13,buffname="剑·羽",ids={},enable=true},{iconid=13,buffname="钟林毓秀",ids={},enable=true},{iconid=13,buffname="琴音",ids={},enable=true}}}}
		
		```
		
* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="锁足",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="三才化生",ids={},enable=true},
			{iconid=13,buffname="影痕",ids={},enable=true},
			{iconid=13,buffname="止水",ids={},enable=true},
			{iconid=13,buffname="锁足",ids={},enable=true},
			{iconid=13,buffname="五方行尽",ids={},enable=true},
			{iconid=13,buffname="百足迷心",ids={},enable=true},
			{iconid=13,buffname="天蛛献祭",ids={},enable=true},
			{iconid=13,buffname="吐故纳新",ids={},enable=true},
			{iconid=13,buffname="滞",ids={},enable=true},
			{iconid=13,buffname="禁缚",ids={},enable=true},
			{iconid=13,buffname="太乙",ids={},enable=true},
			{iconid=13,buffname="百足",ids={},enable=true},
			{iconid=13,buffname="太阴指",ids={},enable=true},
			{iconid=13,buffname="碎冰",ids={},enable=true},
			{iconid=13,buffname="伏夜·缠",ids={},enable=true},
			{iconid=13,buffname="铁爪",ids={},enable=true},
			{iconid=13,buffname="落雁",ids={},enable=true},
			{iconid=13,buffname="断筋",ids={},enable=true},
			{iconid=13,buffname="钻心刺骨",ids={},enable=true},
			{iconid=13,buffname="剑·羽",ids={},enable=true},
			{iconid=13,buffname="钟林毓秀",ids={},enable=true},
			{iconid=13,buffname="琴音",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标定身
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="定身",showBuffName=true,monitors={common={{iconid=13,buffname="太阴指",ids={},enable=true},{iconid=13,buffname="傍花随柳",ids={},enable=true},{iconid=13,buffname="帝骖龙翔",ids={},enable=true},{iconid=13,buffname="大道无术",ids={},enable=true},{iconid=13,buffname="七星拱瑞",ids={},enable=true},{iconid=13,buffname="芙蓉并蒂",ids={},enable=true},{iconid=13,buffname="完骨",ids={},enable=true},{iconid=13,buffname="破势",ids={},enable=true},{iconid=13,buffname="同归",ids={},enable=true},{iconid=13,buffname="定身",ids={},enable=true},{iconid=13,buffname="松涛",ids={},enable=true},{iconid=13,buffname="绛唇珠袖",ids={},enable=true},{iconid=13,buffname="丝牵",ids={},enable=true},{iconid=13,buffname="金针",ids={},enable=true},{iconid=13,buffname="天绝地灭",ids={},enable=true},{iconid=13,buffname="迷影",ids={},enable=true},{iconid=13,buffname="幻蛊",ids={},enable=true},{iconid=13,buffname="伏夜·定",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="定身",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="太阴指",ids={},enable=true},
			{iconid=13,buffname="傍花随柳",ids={},enable=true},
			{iconid=13,buffname="帝骖龙翔",ids={},enable=true},
			{iconid=13,buffname="大道无术",ids={},enable=true},
			{iconid=13,buffname="七星拱瑞",ids={},enable=true},
			{iconid=13,buffname="芙蓉并蒂",ids={},enable=true},
			{iconid=13,buffname="完骨",ids={},enable=true},
			{iconid=13,buffname="破势",ids={},enable=true},
			{iconid=13,buffname="同归",ids={},enable=true},
			{iconid=13,buffname="定身",ids={},enable=true},
			{iconid=13,buffname="松涛",ids={},enable=true},
			{iconid=13,buffname="绛唇珠袖",ids={},enable=true},
			{iconid=13,buffname="丝牵",ids={},enable=true},
			{iconid=13,buffname="金针",ids={},enable=true},
			{iconid=13,buffname="天绝地灭",ids={},enable=true},
			{iconid=13,buffname="迷影",ids={},enable=true},
			{iconid=13,buffname="幻蛊",ids={},enable=true},
			{iconid=13,buffname="伏夜·定",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标爆发
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="爆发",showBuffName=true,monitors={common={{iconid=13,buffname="疾如风",ids={},enable=true},{iconid=13,buffname="青荷",ids={},enable=true},{iconid=13,buffname="紫气东来",ids={},enable=true},{iconid=13,buffname="繁音急节",ids={},enable=true},{iconid=13,buffname="弱水",ids={},enable=true},{iconid=13,buffname="香疏影",ids={},enable=true},{iconid=13,buffname="乱洒",ids={},enable=true},{iconid=13,buffname="酒中仙",ids={},enable=true},{iconid=13,buffname="渊",ids={},enable=true},{iconid=13,buffname="莺鸣",ids={},enable=true},{iconid=13,buffname="扬威",ids={},enable=true},{iconid=13,buffname="灵蛇献祭",ids={},enable=true},{iconid=13,buffname="贯木流年",ids={},enable=true},{iconid=13,buffname="疏狂",ids={},enable=true},{iconid=13,buffname="重激",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="爆发",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="疾如风",ids={},enable=true},
			{iconid=13,buffname="青荷",ids={},enable=true},
			{iconid=13,buffname="紫气东来",ids={},enable=true},
			{iconid=13,buffname="繁音急节",ids={},enable=true},
			{iconid=13,buffname="弱水",ids={},enable=true},
			{iconid=13,buffname="香疏影",ids={},enable=true},
			{iconid=13,buffname="乱洒",ids={},enable=true},
			{iconid=13,buffname="酒中仙",ids={},enable=true},
			{iconid=13,buffname="渊",ids={},enable=true},
			{iconid=13,buffname="莺鸣",ids={},enable=true},
			{iconid=13,buffname="扬威",ids={},enable=true},
			{iconid=13,buffname="灵蛇献祭",ids={},enable=true},
			{iconid=13,buffname="贯木流年",ids={},enable=true},
			{iconid=13,buffname="疏狂",ids={},enable=true},
			{iconid=13,buffname="重激",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标减伤
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="减伤",showBuffName=true,monitors={common={{iconid=13,buffname="守如山",ids={},enable=true},{iconid=13,buffname="转乾坤",ids={},enable=true},{iconid=13,buffname="无相诀",ids={},enable=true},{iconid=13,buffname="春泥护花",ids={},enable=true},{iconid=13,buffname="雾体",ids={},enable=true},{iconid=13,buffname="御天",ids={},enable=true},{iconid=13,buffname="天地低昂",ids={},enable=true},{iconid=13,buffname="贪魔体",ids={},enable=true},{iconid=13,buffname="零落",ids={},enable=true},{iconid=13,buffname="正骨",ids={},enable=true},{iconid=13,buffname="玄水蛊",ids={},enable=true},{iconid=13,buffname="笑醉狂",ids={},enable=true},{iconid=13,buffname="脑户",ids={},enable=true},{iconid=13,buffname="龙啸九天",ids={},enable=true},{iconid=13,buffname="圣手织天",ids={},enable=true},{iconid=13,buffname="金屋",ids={},enable=true},{iconid=13,buffname="蝶戏水",ids={},enable=true},{iconid=13,buffname="护体",ids={},enable=true},{iconid=13,buffname="盾壁",ids={},enable=true},{iconid=13,buffname="盾墙",ids={},enable=true},{iconid=13,buffname="荣辉",ids={},enable=true},{iconid=13,buffname="盾护",ids={},enable=true},{iconid=13,buffname="捍卫",ids={},enable=true},{iconid=13,buffname="无我",ids={},enable=true},{iconid=13,buffname="绝歌",ids={},enable=true},{iconid=13,buffname="杯水留影",ids={},enable=true},{iconid=13,buffname="震八方",ids={},enable=true},{iconid=13,buffname="梅花三弄",ids={},enable=true},{iconid=13,buffname="破釜沉舟",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="减伤",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="守如山",ids={},enable=true},
			{iconid=13,buffname="转乾坤",ids={},enable=true},
			{iconid=13,buffname="无相诀",ids={},enable=true},
			{iconid=13,buffname="春泥护花",ids={},enable=true},
			{iconid=13,buffname="雾体",ids={},enable=true},
			{iconid=13,buffname="御天",ids={},enable=true},
			{iconid=13,buffname="天地低昂",ids={},enable=true},
			{iconid=13,buffname="贪魔体",ids={},enable=true},
			{iconid=13,buffname="零落",ids={},enable=true},
			{iconid=13,buffname="正骨",ids={},enable=true},
			{iconid=13,buffname="玄水蛊",ids={},enable=true},
			{iconid=13,buffname="笑醉狂",ids={},enable=true},
			{iconid=13,buffname="脑户",ids={},enable=true},
			{iconid=13,buffname="龙啸九天",ids={},enable=true},
			{iconid=13,buffname="圣手织天",ids={},enable=true},
			{iconid=13,buffname="金屋",ids={},enable=true},
			{iconid=13,buffname="蝶戏水",ids={},enable=true},
			{iconid=13,buffname="护体",ids={},enable=true},
			{iconid=13,buffname="盾壁",ids={},enable=true},
			{iconid=13,buffname="盾墙",ids={},enable=true},
			{iconid=13,buffname="荣辉",ids={},enable=true},
			{iconid=13,buffname="盾护",ids={},enable=true},
			{iconid=13,buffname="捍卫",ids={},enable=true},
			{iconid=13,buffname="无我",ids={},enable=true},
			{iconid=13,buffname="绝歌",ids={},enable=true},
			{iconid=13,buffname="杯水留影",ids={},enable=true},
			{iconid=13,buffname="震八方",ids={},enable=true},
			{iconid=13,buffname="梅花三弄",ids={},enable=true},
			{iconid=13,buffname="破釜沉舟",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标闪避
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="闪避",showBuffName=true,monitors={common={{iconid=13,buffname="惊鸿游龙",ids={},enable=true},{iconid=13,buffname="云栖松",ids={},enable=true},{iconid=13,buffname="风吹荷",ids={},enable=true},{iconid=13,buffname="醉逍遥",ids={},enable=true},{iconid=13,buffname="御风而行",ids={},enable=true},{iconid=13,buffname="两生",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="闪避",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="惊鸿游龙",ids={},enable=true},
			{iconid=13,buffname="云栖松",ids={},enable=true},
			{iconid=13,buffname="风吹荷",ids={},enable=true},
			{iconid=13,buffname="醉逍遥",ids={},enable=true},
			{iconid=13,buffname="御风而行",ids={},enable=true},
			{iconid=13,buffname="两生",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标减疗
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="减疗",showBuffName=true,monitors={common={{iconid=13,buffname="霹雳",ids={},enable=true},{iconid=13,buffname="穿心弩",ids={},enable=true},{iconid=13,buffname="穿心",ids={},enable=true},{iconid=13,buffname="无相",ids={},enable=true},{iconid=13,buffname="恒河劫沙",ids={},enable=true},{iconid=13,buffname="百足枯残",ids={},enable=true},{iconid=13,buffname="蝎蛰",ids={},enable=true},{iconid=13,buffname="月劫",ids={},enable=true},{iconid=13,buffname="神龙降世",ids={},enable=true},{iconid=13,buffname="盾击",ids={},enable=true},{iconid=13,buffname="楚济",ids={},enable=true},{iconid=13,buffname="吞楚",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="减疗",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="霹雳",ids={},enable=true},
			{iconid=13,buffname="穿心弩",ids={},enable=true},
			{iconid=13,buffname="穿心",ids={},enable=true},
			{iconid=13,buffname="无相",ids={},enable=true},
			{iconid=13,buffname="恒河劫沙",ids={},enable=true},
			{iconid=13,buffname="百足枯残",ids={},enable=true},
			{iconid=13,buffname="蝎蛰",ids={},enable=true},
			{iconid=13,buffname="月劫",ids={},enable=true},
			{iconid=13,buffname="神龙降世",ids={},enable=true},
			{iconid=13,buffname="盾击",ids={},enable=true},
			{iconid=13,buffname="楚济",ids={},enable=true},
			{iconid=13,buffname="吞楚",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标减速
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="减速",showBuffName=true,monitors={common={{iconid=13,buffname="太乙",ids={},enable=true},{iconid=13,buffname="减速",ids={},enable=true},{iconid=13,buffname="穿",ids={},enable=true},{iconid=13,buffname="玄一",ids={},enable=true},{iconid=13,buffname="步迟",ids={},enable=true},{iconid=13,buffname="缠足",ids={},enable=true},{iconid=13,buffname="生太极",ids={},enable=true},{iconid=13,buffname="抱残式",ids={},enable=true},{iconid=13,buffname="少阳指",ids={},enable=true},{iconid=13,buffname="剑主天地",ids={},enable=true},{iconid=13,buffname="惊涛",ids={},enable=true},{iconid=13,buffname="千丝",ids={},enable=true},{iconid=13,buffname="冰封",ids={},enable=true},{iconid=13,buffname="毒蒺藜",ids={},enable=true},{iconid=13,buffname="业海罪缚",ids={},enable=true},{iconid=13,buffname="火舞长空",ids={},enable=true},{iconid=13,buffname="雪中行",ids={},enable=true},{iconid=13,buffname="业力",ids={},enable=true},{iconid=13,buffname="山阵",ids={},enable=true},{iconid=13,buffname="埋骨",ids={},enable=true},{iconid=13,buffname="暴雨梨花针",ids={},enable=true},{iconid=13,buffname="刖足",ids={},enable=true},{iconid=13,buffname="伏夜·缓",ids={},enable=true},{iconid=13,buffname="盾墙",ids={},enable=true},{iconid=13,buffname="卷云",ids={},enable=true},{iconid=13,buffname="难行",ids={},enable=true},{iconid=13,buffname="禁缚",ids={},enable=true},{iconid=13,buffname="轰雷",ids={},enable=true},{iconid=13,buffname="剑·宫",ids={},enable=true},{iconid=13,buffname="风入松",ids={},enable=true},{iconid=13,buffname="伏尘",ids={},enable=true},{iconid=13,buffname="击鼎",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="减速",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="太乙",ids={},enable=true},
			{iconid=13,buffname="减速",ids={},enable=true},
			{iconid=13,buffname="穿",ids={},enable=true},
			{iconid=13,buffname="玄一",ids={},enable=true},
			{iconid=13,buffname="步迟",ids={},enable=true},
			{iconid=13,buffname="缠足",ids={},enable=true},
			{iconid=13,buffname="生太极",ids={},enable=true},
			{iconid=13,buffname="抱残式",ids={},enable=true},
			{iconid=13,buffname="少阳指",ids={},enable=true},
			{iconid=13,buffname="剑主天地",ids={},enable=true},
			{iconid=13,buffname="惊涛",ids={},enable=true},
			{iconid=13,buffname="千丝",ids={},enable=true},
			{iconid=13,buffname="冰封",ids={},enable=true},
			{iconid=13,buffname="毒蒺藜",ids={},enable=true},
			{iconid=13,buffname="业海罪缚",ids={},enable=true},
			{iconid=13,buffname="火舞长空",ids={},enable=true},
			{iconid=13,buffname="雪中行",ids={},enable=true},
			{iconid=13,buffname="业力",ids={},enable=true},
			{iconid=13,buffname="山阵",ids={},enable=true},
			{iconid=13,buffname="埋骨",ids={},enable=true},
			{iconid=13,buffname="暴雨梨花针",ids={},enable=true},
			{iconid=13,buffname="刖足",ids={},enable=true},
			{iconid=13,buffname="伏夜·缓",ids={},enable=true},
			{iconid=13,buffname="盾墙",ids={},enable=true},
			{iconid=13,buffname="卷云",ids={},enable=true},
			{iconid=13,buffname="难行",ids={},enable=true},
			{iconid=13,buffname="禁缚",ids={},enable=true},
			{iconid=13,buffname="轰雷",ids={},enable=true},
			{iconid=13,buffname="剑·宫",ids={},enable=true},
			{iconid=13,buffname="风入松",ids={},enable=true},
			{iconid=13,buffname="伏尘",ids={},enable=true},
			{iconid=13,buffname="击鼎",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标其他
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="其他",showBuffName=true,monitors={common={{iconid=13,buffname="傍花随柳",ids={},enable=true},{iconid=13,buffname="龙魂",ids={},enable=true},{iconid=13,buffname="徐如林",ids={},enable=true},{iconid=13,buffname="啸如虎",ids={},enable=true},{iconid=13,buffname="声趣",ids={},enable=true},{iconid=13,buffname="倒地",ids={},enable=true},{iconid=13,buffname="无声",ids={},enable=true},{iconid=13,buffname="追命无声",ids={},enable=true},{iconid=13,buffname="圣月佑",ids={},enable=true},{iconid=13,buffname="虚回",ids={},enable=true},{iconid=13,buffname="风过无痕",ids={},enable=true},{iconid=13,buffname="临风",ids={},enable=true},{iconid=13,buffname="行气血",ids={},enable=true},{iconid=13,buffname="枭泣",ids={},enable=true},{iconid=13,buffname="鹰目",ids={},enable=true},{iconid=13,buffname="泉凝月",ids={},enable=true},{iconid=13,buffname="风虎",ids={},enable=true},{iconid=13,buffname="牧云",ids={},enable=true},{iconid=13,buffname="天地根",ids={},enable=true},{iconid=13,buffname="影捷",ids={},enable=true},{iconid=13,buffname="锋针",ids={},enable=true},{iconid=13,buffname="善护",ids={},enable=true},{iconid=13,buffname="繁音急节",ids={},enable=true},{iconid=13,buffname="雾外江山",ids={},enable=true},{iconid=13,buffname="雨集",ids={},enable=true},{iconid=13,buffname="恶狗拦路",ids={},enable=true},{iconid=13,buffname="冲阴阳",ids={},enable=true},{iconid=13,buffname="日月灵魂",ids={},enable=true},{iconid=13,buffname="日月同辉",ids={},enable=true},{iconid=13,buffname="女娲补天",ids={},enable=true},{iconid=13,buffname="罗汉金身",ids={},enable=true},{iconid=13,buffname="渊",ids={},enable=true},{iconid=13,buffname="荆天棘地",ids={},enable=true},{iconid=13,buffname="盾立",ids={},enable=true},{iconid=13,buffname="沃土",ids={},enable=true},{iconid=13,buffname="玉蟾献祭",ids={},enable=true},{iconid=13,buffname="急曲",ids={},enable=true},{iconid=13,buffname="叠刃",ids={},enable=true},{iconid=13,buffname="活祭",ids={},enable=true},{iconid=13,buffname="狂绝",ids={},enable=true},{iconid=13,buffname="盾飞",ids={},enable=true},{iconid=13,buffname="毫针",ids={},enable=true},{iconid=13,buffname="缓深",ids={},enable=true},{iconid=13,buffname="息疗",ids={},enable=true},{iconid=13,buffname="日月齐光",ids={},enable=true},{iconid=13,buffname="清歌",ids={},enable=true},{iconid=13,buffname="映日",ids={},enable=true},{iconid=13,buffname="平笃",ids={},enable=true},{iconid=13,buffname="江逐月天",ids={},enable=true},{iconid=13,buffname="超然物外",ids={},enable=true},{iconid=13,buffname="迴光",ids={},enable=true},{iconid=13,buffname="迴梦",ids={},enable=true},{iconid=13,buffname="放歌",ids={},enable=true},{iconid=13,buffname="扬旌沙场",ids={},enable=true},{iconid=13,buffname="风入松",ids={},enable=true},{iconid=13,buffname="梦未醒",ids={},enable=true},{iconid=13,buffname="啸吒",ids={},enable=true},{iconid=13,buffname="剑鸣",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="其他",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="傍花随柳",ids={},enable=true},
			{iconid=13,buffname="龙魂",ids={},enable=true},
			{iconid=13,buffname="徐如林",ids={},enable=true},
			{iconid=13,buffname="啸如虎",ids={},enable=true},
			{iconid=13,buffname="声趣",ids={},enable=true},
			{iconid=13,buffname="倒地",ids={},enable=true},
			{iconid=13,buffname="无声",ids={},enable=true},
			{iconid=13,buffname="追命无声",ids={},enable=true},
			{iconid=13,buffname="圣月佑",ids={},enable=true},
			{iconid=13,buffname="虚回",ids={},enable=true},
			{iconid=13,buffname="风过无痕",ids={},enable=true},
			{iconid=13,buffname="临风",ids={},enable=true},
			{iconid=13,buffname="行气血",ids={},enable=true},
			{iconid=13,buffname="枭泣",ids={},enable=true},
			{iconid=13,buffname="鹰目",ids={},enable=true},
			{iconid=13,buffname="泉凝月",ids={},enable=true},
			{iconid=13,buffname="风虎",ids={},enable=true},
			{iconid=13,buffname="牧云",ids={},enable=true},
			{iconid=13,buffname="天地根",ids={},enable=true},
			{iconid=13,buffname="影捷",ids={},enable=true},
			{iconid=13,buffname="锋针",ids={},enable=true},
			{iconid=13,buffname="善护",ids={},enable=true},
			{iconid=13,buffname="繁音急节",ids={},enable=true},
			{iconid=13,buffname="雾外江山",ids={},enable=true},
			{iconid=13,buffname="雨集",ids={},enable=true},
			{iconid=13,buffname="恶狗拦路",ids={},enable=true},
			{iconid=13,buffname="冲阴阳",ids={},enable=true},
			{iconid=13,buffname="日月灵魂",ids={},enable=true},
			{iconid=13,buffname="日月同辉",ids={},enable=true},
			{iconid=13,buffname="女娲补天",ids={},enable=true},
			{iconid=13,buffname="罗汉金身",ids={},enable=true},
			{iconid=13,buffname="渊",ids={},enable=true},
			{iconid=13,buffname="荆天棘地",ids={},enable=true},
			{iconid=13,buffname="盾立",ids={},enable=true},
			{iconid=13,buffname="沃土",ids={},enable=true},
			{iconid=13,buffname="玉蟾献祭",ids={},enable=true},
			{iconid=13,buffname="急曲",ids={},enable=true},
			{iconid=13,buffname="叠刃",ids={},enable=true},
			{iconid=13,buffname="活祭",ids={},enable=true},
			{iconid=13,buffname="狂绝",ids={},enable=true},
			{iconid=13,buffname="盾飞",ids={},enable=true},
			{iconid=13,buffname="毫针",ids={},enable=true},
			{iconid=13,buffname="缓深",ids={},enable=true},
			{iconid=13,buffname="息疗",ids={},enable=true},
			{iconid=13,buffname="日月齐光",ids={},enable=true},
			{iconid=13,buffname="清歌",ids={},enable=true},
			{iconid=13,buffname="映日",ids={},enable=true},
			{iconid=13,buffname="平笃",ids={},enable=true},
			{iconid=13,buffname="江逐月天",ids={},enable=true},
			{iconid=13,buffname="超然物外",ids={},enable=true},
			{iconid=13,buffname="迴光",ids={},enable=true},
			{iconid=13,buffname="迴梦",ids={},enable=true},
			{iconid=13,buffname="放歌",ids={},enable=true},
			{iconid=13,buffname="扬旌沙场",ids={},enable=true},
			{iconid=13,buffname="风入松",ids={},enable=true},
			{iconid=13,buffname="梦未醒",ids={},enable=true},
			{iconid=13,buffname="啸吒",ids={},enable=true},
			{iconid=13,buffname="剑鸣",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标封内
	* 复制内容
	
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="封内",showBuffName=true,monitors={common={{iconid=13,buffname="抢珠式",ids={},enable=true},{iconid=13,buffname="剑心通明",ids={},enable=true},{iconid=13,buffname="八卦洞玄",ids={},enable=true},{iconid=13,buffname="剑破虚空",ids={},enable=true},{iconid=13,buffname="梅花针",ids={},enable=true},{iconid=13,buffname="凄切",ids={},enable=true},{iconid=13,buffname="蟾啸迷心",ids={},enable=true},{iconid=13,buffname="清音长啸",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="封内",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="抢珠式",ids={},enable=true},
			{iconid=13,buffname="剑心通明",ids={},enable=true},
			{iconid=13,buffname="八卦洞玄",ids={},enable=true},
			{iconid=13,buffname="剑破虚空",ids={},enable=true},
			{iconid=13,buffname="梅花针",ids={},enable=true},
			{iconid=13,buffname="凄切",ids={},enable=true},
			{iconid=13,buffname="蟾啸迷心",ids={},enable=true},
			{iconid=13,buffname="清音长啸",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标橙武
	* 复制内容
	
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="橙武",showBuffName=true,monitors={common={{iconid=13,buffname="苍龙",ids={},enable=true},{iconid=13,buffname="青君",ids={},enable=true},{iconid=13,buffname="千叶长生",ids={},enable=true},{iconid=13,buffname="碎魂",ids={},enable=true},{iconid=13,buffname="焚海",ids={},enable=true},{iconid=13,buffname="火龙沥泉",ids={},enable=true},{iconid=13,buffname="紫龙寂地",ids={},enable=true},{iconid=13,buffname="摧城",ids={},enable=true},{iconid=13,buffname="初尘",ids={},enable=true},{iconid=13,buffname="溯流",ids={},enable=true},{iconid=13,buffname="吞虹",ids={},enable=true},{iconid=13,buffname="碧落",ids={},enable=true},{iconid=13,buffname="断鬼",ids={},enable=true},{iconid=13,buffname="落凤",ids={},enable=true},{iconid=13,buffname="墨颠",ids={},enable=true},{iconid=13,buffname="吞吴",ids={},enable=true},{iconid=13,buffname="蛟影",ids={},enable=true},{iconid=13,buffname="雪名",ids={},enable=true},{iconid=13,buffname="周流星位",ids={},enable=true},{iconid=13,buffname="玉清玄明",ids={},enable=true},{iconid=13,buffname="留情",ids={},enable=true},{iconid=13,buffname="赤霄红莲",ids={},enable=true},{iconid=13,buffname="渊微指玄",ids={},enable=true},{iconid=13,buffname="幽月·乱花",ids={},enable=true},{iconid=13,buffname="赤练蓝翼",ids={},enable=true},{iconid=13,buffname="干将·莫邪",ids={},enable=true},{iconid=13,buffname="寒声·寂影",ids={},enable=true},{iconid=13,buffname="龙木金藤",ids={},enable=true},{iconid=13,buffname="白骨碎云",ids={},enable=true},{iconid=13,buffname="燃木",ids={},enable=true},{iconid=13,buffname="浮心·劫",ids={},enable=true},{iconid=13,buffname="白衣焚天",ids={},enable=true},{iconid=13,buffname="西天",ids={},enable=true},{iconid=13,buffname="莲心观佛",ids={},enable=true},{iconid=13,buffname="莲华·缘",ids={},enable=true},{iconid=13,buffname="织炎断尘",ids={},enable=true},{iconid=13,buffname="碧王",ids={},enable=true},{iconid=13,buffname="太阿",ids={},enable=true},{iconid=13,buffname="弱水",ids={},enable=true},{iconid=13,buffname="浴凰",ids={},enable=true},{iconid=13,buffname="青冥",ids={},enable=true},{iconid=13,buffname="太上忘情",ids={},enable=true},{iconid=13,buffname="绛玉拨云",ids={},enable=true},{iconid=13,buffname="地渊沉星",ids={},enable=true},{iconid=13,buffname="鸢翔天",ids={},enable=true},{iconid=13,buffname="凤尾天机",ids={},enable=true},{iconid=13,buffname="碎屏沉星",ids={},enable=true},{iconid=13,buffname="孔雀羽",ids={},enable=true},{iconid=13,buffname="含沙射影",ids={},enable=true},{iconid=13,buffname="摧山弩",ids={},enable=true},{iconid=13,buffname="造化异轨",ids={},enable=true},{iconid=13,buffname="火魂",ids={},enable=true},{iconid=13,buffname="悲魔饥火",ids={},enable=true},{iconid=13,buffname="明王镇狱",ids={},enable=true},{iconid=13,buffname="残月惊天",ids={},enable=true},{iconid=13,buffname="龙悔",ids={},enable=true},{iconid=13,buffname="浮沉照影",ids={},enable=true},{iconid=13,buffname="焚三世",ids={},enable=true},{iconid=13,buffname="执手",ids={},enable=true},{iconid=13,buffname="壶中乾坤",ids={},enable=true},{iconid=13,buffname="霜月明",ids={},enable=true},{iconid=13,buffname="炙狱邪龙",ids={},enable=true},{iconid=13,buffname="涯风嘲雨",ids={},enable=true},{iconid=13,buffname="血云",ids={},enable=true},{iconid=13,buffname="太初社稷",ids={},enable=true},{iconid=13,buffname="征天",ids={},enable=true},{iconid=13,buffname="题龙旐",ids={},enable=true},{iconid=13,buffname="千仞",ids={},enable=true},{iconid=13,buffname="旧嗜",ids={},enable=true},{iconid=13,buffname="朱轩怀雀",ids={},enable=true},{iconid=13,buffname="修罗鬼面",ids={},enable=true},{iconid=13,buffname="青玉流",ids={},enable=true},{iconid=13,buffname="洞仙引",ids={},enable=true},{iconid=13,buffname="盈缺",ids={},enable=true},{iconid=13,buffname="文姬泪",ids={},enable=true},{iconid=13,buffname="雨岩金莲",ids={},enable=true},{iconid=13,buffname="雪怒",ids={},enable=true},{iconid=13,buffname="血悲",ids={},enable=true},{iconid=13,buffname="新亭侯",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="橙武",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="苍龙",ids={},enable=true},
			{iconid=13,buffname="青君",ids={},enable=true},
			{iconid=13,buffname="千叶长生",ids={},enable=true},
			{iconid=13,buffname="碎魂",ids={},enable=true},
			{iconid=13,buffname="焚海",ids={},enable=true},
			{iconid=13,buffname="火龙沥泉",ids={},enable=true},
			{iconid=13,buffname="紫龙寂地",ids={},enable=true},
			{iconid=13,buffname="摧城",ids={},enable=true},
			{iconid=13,buffname="初尘",ids={},enable=true},
			{iconid=13,buffname="溯流",ids={},enable=true},
			{iconid=13,buffname="吞虹",ids={},enable=true},
			{iconid=13,buffname="碧落",ids={},enable=true},
			{iconid=13,buffname="断鬼",ids={},enable=true},
			{iconid=13,buffname="落凤",ids={},enable=true},
			{iconid=13,buffname="墨颠",ids={},enable=true},
			{iconid=13,buffname="吞吴",ids={},enable=true},
			{iconid=13,buffname="蛟影",ids={},enable=true},
			{iconid=13,buffname="雪名",ids={},enable=true},
			{iconid=13,buffname="周流星位",ids={},enable=true},
			{iconid=13,buffname="玉清玄明",ids={},enable=true},
			{iconid=13,buffname="留情",ids={},enable=true},
			{iconid=13,buffname="赤霄红莲",ids={},enable=true},
			{iconid=13,buffname="渊微指玄",ids={},enable=true},
			{iconid=13,buffname="幽月·乱花",ids={},enable=true},
			{iconid=13,buffname="赤练蓝翼",ids={},enable=true},
			{iconid=13,buffname="干将·莫邪",ids={},enable=true},
			{iconid=13,buffname="寒声·寂影",ids={},enable=true},
			{iconid=13,buffname="龙木金藤",ids={},enable=true},
			{iconid=13,buffname="白骨碎云",ids={},enable=true},
			{iconid=13,buffname="燃木",ids={},enable=true},
			{iconid=13,buffname="浮心·劫",ids={},enable=true},
			{iconid=13,buffname="白衣焚天",ids={},enable=true},
			{iconid=13,buffname="西天",ids={},enable=true},
			{iconid=13,buffname="莲心观佛",ids={},enable=true},
			{iconid=13,buffname="莲华·缘",ids={},enable=true},
			{iconid=13,buffname="织炎断尘",ids={},enable=true},
			{iconid=13,buffname="碧王",ids={},enable=true},
			{iconid=13,buffname="太阿",ids={},enable=true},
			{iconid=13,buffname="弱水",ids={},enable=true},
			{iconid=13,buffname="浴凰",ids={},enable=true},
			{iconid=13,buffname="青冥",ids={},enable=true},
			{iconid=13,buffname="太上忘情",ids={},enable=true},
			{iconid=13,buffname="绛玉拨云",ids={},enable=true},
			{iconid=13,buffname="地渊沉星",ids={},enable=true},
			{iconid=13,buffname="鸢翔天",ids={},enable=true},
			{iconid=13,buffname="凤尾天机",ids={},enable=true},
			{iconid=13,buffname="碎屏沉星",ids={},enable=true},
			{iconid=13,buffname="孔雀羽",ids={},enable=true},
			{iconid=13,buffname="含沙射影",ids={},enable=true},
			{iconid=13,buffname="摧山弩",ids={},enable=true},
			{iconid=13,buffname="造化异轨",ids={},enable=true},
			{iconid=13,buffname="火魂",ids={},enable=true},
			{iconid=13,buffname="悲魔饥火",ids={},enable=true},
			{iconid=13,buffname="明王镇狱",ids={},enable=true},
			{iconid=13,buffname="残月惊天",ids={},enable=true},
			{iconid=13,buffname="龙悔",ids={},enable=true},
			{iconid=13,buffname="浮沉照影",ids={},enable=true},
			{iconid=13,buffname="焚三世",ids={},enable=true},
			{iconid=13,buffname="执手",ids={},enable=true},
			{iconid=13,buffname="壶中乾坤",ids={},enable=true},
			{iconid=13,buffname="霜月明",ids={},enable=true},
			{iconid=13,buffname="炙狱邪龙",ids={},enable=true},
			{iconid=13,buffname="涯风嘲雨",ids={},enable=true},
			{iconid=13,buffname="血云",ids={},enable=true},
			{iconid=13,buffname="太初社稷",ids={},enable=true},
			{iconid=13,buffname="征天",ids={},enable=true},
			{iconid=13,buffname="题龙旐",ids={},enable=true},
			{iconid=13,buffname="千仞",ids={},enable=true},
			{iconid=13,buffname="旧嗜",ids={},enable=true},
			{iconid=13,buffname="朱轩怀雀",ids={},enable=true},
			{iconid=13,buffname="修罗鬼面",ids={},enable=true},
			{iconid=13,buffname="青玉流",ids={},enable=true},
			{iconid=13,buffname="洞仙引",ids={},enable=true},
			{iconid=13,buffname="盈缺",ids={},enable=true},
			{iconid=13,buffname="文姬泪",ids={},enable=true},
			{iconid=13,buffname="雨岩金莲",ids={},enable=true},
			{iconid=13,buffname="雪怒",ids={},enable=true},
			{iconid=13,buffname="血悲",ids={},enable=true},
			{iconid=13,buffname="新亭侯",ids={},enable=true}
		}
	}
}
</pre>

* 监控目标封轻功
	* 复制内容
		
		```
		
		{cdBarWidth=240,target="TARGET",enable=true,scale=1,boxBgUITex="UI/Image/Common/Box.UITex|44",cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",dragable=true,maxLineCount=16,hideVoidBuff=false,cdBar=false,hideOthers=false,anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},caption="封轻功",showBuffName=true,monitors={common={{iconid=13,buffname="吞日月",ids={},enable=true},{iconid=13,buffname="千丝迷心",ids={},enable=true},{iconid=13,buffname="迷幻",ids={},enable=true},{iconid=13,buffname="身乏",ids={},enable=true},{iconid=13,buffname="滞影",ids={},enable=true},{iconid=13,buffname="玳弦",ids={},enable=true},{iconid=13,buffname="云景",ids={},enable=true},{iconid=13,buffname="恶狗拦路",ids={},enable=true},{iconid=13,buffname="幻相",ids={},enable=true},{iconid=13,buffname="半步颠",ids={},enable=true},{iconid=13,buffname="步残",ids={},enable=true},{iconid=13,buffname="重围",ids={},enable=true},{iconid=13,buffname="行泽",ids={},enable=true}}}}
		
		```
		
	* 预览
<pre>
{
	cdBarWidth=240,
	target="TARGET",
	enable=true,
	scale=1,
	boxBgUITex="UI/Image/Common/Box.UITex|44",
	cdBarUITex="./Interface/MY/MY_!Base/image/ST_UI.UITex|7",
	dragable=true,
	maxLineCount=16,
	hideVoidBuff=false,
	cdBar=false,
	hideOthers=false,
	anchor={y=152,x=-343,s="TOPLEFT",r="CENTER"},
	caption="封轻功",
	showBuffName=true,
	monitors={
		common={
			{iconid=13,buffname="吞日月",ids={},enable=true},
			{iconid=13,buffname="千丝迷心",ids={},enable=true},
			{iconid=13,buffname="迷幻",ids={},enable=true},
			{iconid=13,buffname="身乏",ids={},enable=true},
			{iconid=13,buffname="滞影",ids={},enable=true},
			{iconid=13,buffname="玳弦",ids={},enable=true},
			{iconid=13,buffname="云景",ids={},enable=true},
			{iconid=13,buffname="恶狗拦路",ids={},enable=true},
			{iconid=13,buffname="幻相",ids={},enable=true},
			{iconid=13,buffname="半步颠",ids={},enable=true},
			{iconid=13,buffname="步残",ids={},enable=true},
			{iconid=13,buffname="重围",ids={},enable=true},
			{iconid=13,buffname="行泽",ids={},enable=true}
		}
	}
}
</pre>