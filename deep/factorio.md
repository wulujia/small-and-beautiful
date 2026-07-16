# Factorio / Wube Software（Michal Kovařík "kovarex" & Tomáš Kozelek）

> 一个人 2012 年在布拉格开写的工厂自动化游戏，先靠官网自售 11 万份熬到 Steam，再用"永不打折、只涨价"的定价纪律和 360 期连续不断更的周五开发日志，做成 400 万份级的长销品 ｜ factorio.com ｜ Michal Kovařík (kovarex) & Tomáš Kozelek ｜ 2012 开始开发、2014-09 成立公司（布拉格）[1] ｜ 31 人（2024-02）[1] ｜ PC/主机工厂建造模拟 ｜ 官方口径 350 万份（2022-12），年销约 50 万份 [11]；第三方估算 2024 年前已破 400 万、Steam 累计 500 万+ [26]；Space Age DLC 首周 40 万份 [13]；累计流水估算超 25 亿捷克克朗（约 1 亿美元+）[18]

## 缝隙切入点

- 2012 年春，程序员 Michal Kovařík 辞职全职做 Factorio——他想深玩"自动化 + 物流 + 军事"的游戏，市面上不存在，于是自己做 [20]。灵感直接来自 Minecraft 的工业 mod（IndustrialCraft、BuildCraft）[1]：mod 的流行已经验证了需求，但没人把"自动化工厂"做成一款独立、完整、打磨过的游戏。
- 他对风险的计算非常朴素：一个人开发，投入的基本只有时间，"回本门槛很低"；同时清楚"这类项目绝大多数会失败，我做好了失败的准备" [20]。缝隙创业的起点不是宏大判断，而是低成本可承受的试错。

## 时机

- **赶上众筹窗口，但成绩平平**：Indiegogo 众筹 2013-01-31 至 03-03，目标 €17,000，最终 €21,626，勉强超额 [1][2]。这笔钱的意义不是资金而是许可——证明有人愿意为一个 2D 工厂游戏付钱。
- **在 EA 声誉最差的年代做成 EA 标杆**：2016-02-25 上 Steam 早访问时，EA 模式已被大量弃坑项目拖臭。Factorio 反向操作：上架时已在官网卖了三年、迭代到相当稳定，EA 期间年销约 50 万份、好评率长期 98% 上下（压倒性好评）[1][11][26]。
- **给巨头让路的档期决策**：1.0 原定 2020-09-25 发布，Cyberpunk 2077 改期到 9-17 后，Wube 判断"任何贴着它的发布都会被吸走全部注意力"，把 1.0 提前五周到 2020-08-14 [19]。小团队不赌正面碰撞，赌自己的节奏。
- **Space Age 踩准自己的节奏**：2024-10-21 发布，理由直白——夏休后有时间打磨、圣诞假期前留足 bugfix 窗口 [12]。发布周登顶 Steam 全球畅销榜 [18]，同时在线 118,674 人破历史纪录（此前峰值 2020 年的 34,700）[13]。

## 差异化

- **定价即人格**：不打折（下节详述）、不用 .99 定价——kovarex 说整数定价是因为不想"用心理把戏骗顾客" [3][17]。
- **无 DRM + 免费 demo + 对盗版宽容**：kovarex 在论坛公开表态，不在乎玩家是不是先下了盗版试玩再买，官方靠自动更新、稳定发布这些"服务"让正版更值 [27]。免费 demo 承担了促销和盗版的双重替代品角色。
- **深度优先于画面**：坚持 2D，把工程力花在模拟规模和性能优化上；FFF 里的多线程、内存访问优化文章本身成了程序员圈的传播素材 [8]。
- **发布日期永远让位于质量**：从开工到 1.0 用了 8.5 年 [7]；扩展包开发 3.5 年以上，目标是"感觉和整个本体一样大" [10]。

## 第一批用户/冷启动

- 众筹结束后不停售：官网持续直售 alpha 版，边卖边开发，价格随游戏成熟逐步上调 [1][4]。
- Wube 自认 2014 年 4 月发布的游戏 trailer 是早期销量的关键拐点 [1]。
- 上 Steam 前，官网已累计卖出约 11 万份（社区披露口径）[23]。
- Steam 放大器效应：FFF-171（2016 年末）自述"全部销量的 85% 发生在过去 12 个月"（即 Steam 上线首年），当年年底逼近 100 万份 [24]。

## 收入与定价

- **价格只升不降**：$20（2016 Steam EA）→ $30（2018-04-16）→ $35（2023-01-26，官方理由是"对齐 2016 年以来的通胀"）[4][5]。Space Age DLC 定价 $35，与本体同价——定价锚是"内容量等于一个本体"，不是成本或竞品 [10][12]。
- **"永不打折"是书面政策**：2018 年官方博客白纸黑字"We have a strict no sale policy. The game will not go on sale on Steam or any other platform"，并说明"4 月 16 日前购买是唯一比新价便宜的方式" [4]。上 Steam 十年零折扣，连 10% 都没有过 [3][5]。
- kovarex 2016 年的完整论述："Not having a sale ever is part of our philosophy. In short term, they are good and bring extra money, but we are targeting long term. I believe that searching for sales is wasted time, and people should decide on the price and value."（永不打折是哲学的一部分；促销短期赚钱，但我们做长期；让用户花时间蹲折扣是方程式里坏的那部分）[3]
- **不打折的商业效果被自己验证**：FFF-247 展示销量曲线——"consistent week-on-week sales since our Steam launch"，没有促销依赖的脉冲-饥荒周期 [25]；kovarex 称近年稳定日销约 1000 份 [17]。
- **里程碑**：100 万（2017 初）[24] → 200 万（2020 初）→ 250 万（2021-02）[9] → 310 万（2022-02）→ 350 万（2022-12）[1][11]；此后维持年销 50 万节奏 [11]。Space Age 首周 40 万份 [13]，第三方估至 2025 年约 120 万份、毛收入约 $30M [26]。
- **食言的代价也照单全收**：2018 年承诺"这是最后一次调价（除非发生不可预见的事）" [4]，2023 年以通胀为由再涨 $5，老玩家在论坛翻出旧承诺质疑，但整体反应正面，甚至有人为表支持多买一份 [5]。
- **堵套利而不是搞促销**：发现有人用 GOG 俄区定价（约 $8.3）买 key 转卖 $20 后，直接取消区域定价 [25]。一以贯之：全世界一个价。
- 早期披露过单位经济：每卖一份净得约 $10，30 万份时已入账约 7100 万克朗 [18]。

## 内容与增长

- **Friday Facts 是这家公司唯一的营销机器**：2013-09-27 第 1 期由 Tomáš 发出，承诺"每个周五总结本周进展" [6]；到 2020-08-14 第 360 期——恰好是 1.0 发布日——七年间 360 个周五无一缺席（FFF-200 自述"200 fridays in a row with no misses"）[6][7][8]。
- 1.0 后停止周更；2023-08-25 为宣布 Space Age 恢复周更，到 2024-11-22 FFF-438 又是 66 期连续，官方自述"一年多的持续周更"后因"修 bug 写不出有趣内容"暂停 [1][14]。
- 内容深度是护城河：从传送带算法、内存访问优化、GUI 重写，到联合创始人在 FFF-356 里写自己失去开发意义、又在陪儿子玩游戏时找回来的心路 [8]。技术圈把 FFF 当博客读，玩家把它当连载追——每周五本身成了社区仪式。
- 营销开支约等于零：无广告投放，增长靠口碑、免费 demo 和 FFF 的固定节拍 [17][20]。
- 内容营销的反面也在 FFF 上发生（见下节）。

## 创始人风格：直言的红利与代价

- 2021-06-18 的 FFF-366 里，kovarex 推荐 Uncle Bob（Robert Martin）的 Clean Code 系列。Reddit 有用户提醒 Uncle Bob 有性别歧视争议、建议加免责声明，kovarex 回复："Take the cancel culture mentality and shove it up your ass."（把取消文化那套塞回你自己屁股里）[15]
- 他拒绝退让的论证方式同样直接：我不关心他的私生活和观点；难道我链接一篇斯大林写的编程建议，你们就会自动继承他的全部意识形态？[15]
- 抵制反噬：风波一周内游戏新增 1000+ 好评，同时在线冲到 Steam 第 63 名 [15]；kovarex 事后受访主题就叫"取消文化与私下支持" [16]。
- 同一种直言对着用户就是资产："别等打折，不会有"（don't wait for discount because there won't be any）[17]；"别在大考或重要作业前买，这游戏危险" [17]。游戏里的铀浓缩配方干脆以他命名——"Kovarex enrichment process"，人格与产品长在一起 [28]。
- 注记：这种风格与"永不打折"同源——把内部判断不加公关缓冲地说出口。这次销量反涨是结果，不是必然；它成立的前提是产品好评率 98% 和零股东压力。

## 转型

- **8.5 年 EA → 1.0（2020-08-14）**：不是功能做完了，而是主动决定"1.1 之后原版封版，只做维护" [7][9]。
- **一次性大扩展，拒绝碎片化 DLC**：FFF-365（2021-02）明确否决了免费更新、Factorio 2、多个小 DLC 三条路，选"一个和本体一样大的扩展包" [9][10]。Space Age 开发 3.5+ 年，随行的 2.0 引擎大版本对所有玩家免费 [12]。
- **收编 mod 生态做扩展**：2021 年雇下最大 mod（Space Exploration）作者 Earendel，头衔是概念画师，实际横跨地形生成、游戏设计、美术方向和引擎代码，最终成为 Space Age 的主架构者 [21][22]。
- **主动收官**：2026-05 官宣 2.1 是"游戏将获得的最后一个大版本"，Earendel 离职做自己的游戏 [1][21]；kovarex 的下一步兴趣是自研语言"K++"和一款 RPG，并称待 DLC 稳定后考虑开源 Factorio [17]。一款游戏做十四年、赚够之后主动封版，不硬造第二曲线。

## 如何保持小

- 1 人（2012）→ 2 人（2014 成立公司）→ 31 人（2024-02）[1][20]。十二年只长到三十人，且大部分扩张（2016 年一年招 6 人）发生在 Steam 现金流验证之后 [24]。
- 无投资人、无发行商：Indiegogo 之后全部靠销售现金流，零负债 [17][18]。
- 拒绝出售的理由是控制权而非估值：kovarex 谈收购邀约——"I'd be extremely unhappy if I owned just 10% instead of the 50%."（哪怕更有钱，只持 10% 而不是 50% 会让我极度不爽）[17]
- 日销 1000 份的稳定现金流是所有"任性"的地基：敢让 1.0 晚 8 年、敢十年不打折、敢在舆论风暴里不道歉、敢给摇钱树封版 [17][25]。
- 定价动作全部服务于"不融资也能养团队"：两次涨价的理由分别是产品成熟 [4] 和通胀 [5]，从未用促销换增长。

## 开放问题（值得当面问创始人的）

1. "永不打折"有没有被数据挑战过？Steam 后台能清楚看到愿望单和折扣转化模型——你们内部有没有人算过参加一次夏促的机会成本？如果算过，数字差多少；如果从没算过，这个决策是价值观免检区吗？
2. FFF 连续 360 周不断更，每周谁写、花掉多少核心工程师工时？有没有想停掉的至暗时刻？你们如何看它的归因——它到底带来多少销量，还是主要作用是招聘和社区维系？
3. Uncle Bob 事件短期看好评反涨，但长期呢：招聘漏斗、团队内部（有员工公开或私下反对吗）、与平台方（任天堂、Steam）的关系有没有付出看不见的代价？如果重来一次，还会用同样的措辞吗？
4. 2018 年白纸黑字"最后一次调价"，2023 年以通胀为由食言。对一家把"对用户诚实"当立身之本的公司，这次内部是怎么讨论的？为什么当初要做绝对承诺，而不是只说"短期不变"？
5. 2.1 封版之后，一家 30 人、年入数千万美元的单品公司往哪走——K++ 和 RPG 是 kovarex 的个人退休项目还是 Wube 的第二曲线？有没有想过公司就此缩编甚至解散也是体面结局？

## 来源

- [1] Wikipedia: Factorio — https://en.wikipedia.org/wiki/Factorio
- [2] Factorio Blog: "Indiegogo campaign just started!"（2013-01）— https://www.factorio.com/blog/post/indiegogo-campaign-just-started
- [3] Factorio Forums: "Factorio is not on Sale (Steam)"（2016-06，kovarex 定价语录）— https://forums.factorio.com/viewtopic.php?t=26991
- [4] Factorio Blog: "Price change"（2018-03-30，$30 与 strict no sale policy）— https://factorio.com/blog/post/016-price-change
- [5] Factorio Forums: "Factorio price increase - 2023/01/26" — https://forums.factorio.com/viewtopic.php?t=104976 ；PC Gamer: "Factorio is getting a price increase in response to inflation" — https://www.pcgamer.com/factorio-is-getting-a-price-increase-in-response-to-inflation/ ；@factoriogame 公告 — https://x.com/factoriogame/status/1616388275169628162
- [6] Factorio Blog: "Friday Facts #1"（2013-09-27）— https://www.factorio.com/blog/post/fff-1
- [7] Factorio Blog: "Friday Facts #360 - 1.0 is here!"（2020-08-14）— https://www.factorio.com/blog/post/fff-360
- [8] William Spies: "Seven Years of Factorio Friday Facts"（2020，含 FFF-200 "200 fridays in a row with no misses"）— https://spieswl.github.io/blog/2020/seven-years-of-factorio-friday-facts
- [9] Factorio Blog: "Friday Facts #365 - Future plans"（2021-02-05，250 万份、扩展包决策）— https://www.factorio.com/blog/post/fff-365
- [10] Factorio Blog: "Friday Facts #367 - Expansion news"（2022-02-04，"as big as vanilla"）— https://www.factorio.com/blog/post/fff-367
- [11] Factorio Blog: "Friday Facts #372 - 2022 recap" — https://www.factorio.com/blog/post/fff-372 ；PC Gamer: "Factorio has sold 3.5 million copies" — https://www.pcgamer.com/factorio-has-sold-35-million-copies/
- [12] Factorio Blog: "Friday Facts #418 - Space Age release date" — https://factorio.com/blog/post/fff-418 ；Neowin: "Factorio: Space Age expansion gets an October release date, cost same as base game" — https://www.neowin.net/news/factorio-space-age-expansion-gets-an-october-release-date-cost-same-price-as-base-game/
- [13] GamingOnLinux: "Factorio: Space Age sold over 400,000 copies and sets a new player count record"（2024-10）— https://www.gamingonlinux.com/2024/10/factorio-space-age-sold-over-400000-copies-and-sets-a-new-player-count-record/ ；SteamDB: "Factorio peaks at 118k players" — https://steamcommunity.com/groups/SteamDB/announcements/detail/4506506224331484095
- [14] Factorio Blog: "Friday Facts #438 - Space Age wrap up"（2024-11-22，625+ bug 修复、88,000 年游玩时长、周更暂停）— https://factorio.com/blog/post/fff-438
- [15] Know Your Meme: Factorio（FFF-366 / Uncle Bob 事件时间线）— https://knowyourmeme.com/memes/subcultures/factorio ；Niche Gamer: "Attempts to Cancel Factorio Dev Backfire, Players and Positive Reviews Swell"（2021-06-20）— https://nichegamer.com/2021/06/20/attempts-to-cancel-factorio-dev-backfire-players-and-positive-reviews-swell/
- [16] Niche Gamer: "Factorio Founder Kovarex Interview; Cancel Culture and Secret Support" — https://nichegamer.com/factorio-founder-kovarex-interview-cancel-culture-and-secret-support/
- [17] r/factorio: "Here is the translated video interview with Kovarex"（2024-09，日销 1000 份、10% vs 50%、K++/开源计划）— https://www.reddit.com/r/factorio/comments/1fd1psh/
- [18] CzechCrunch: "Česká hra Factorio je nejprodávanější na Steamu"（2024-10，累计流水数十亿克朗、Steam 畅销榜第一）— https://cc.cz/cesi-maji-nejprodavanejsi-hru-na-steamu-stvorili-ji-dva-lide-nikdy-nebyla-ve-sleve-a-vydelava-miliardy/ ；CzechCrunch: "Česká nezávislá hra Factorio už autorům vydělala přes 71 milionů korun"（每份净得约 $10）— https://cc.cz/ceska-nezavisla-hra-factorio-uz-autorum-vydelala-pres-71-milionu-korun/
- [19] PC Gamer: "Factorio 1.0 will come a month early to avoid Cyberpunk 2077"（2020-06）— https://www.pcgamer.com/factorio-10-will-come-a-month-earlier-than-expected-to-avoid-cyberpunk-2077/ ；Factorio Blog: "Friday Facts #349 - The 1.0 plan" — https://factorio.com/blog/post/fff-349
- [20] Factorio Forums: "Factorio Developer Interview"（2013，辞职与风险计算）— https://forums.factorio.com/viewtopic.php?t=1120
- [21] Factorio Blog: "Friday Facts #440 - 2.1 plan"（2026-05-29，最后大版本、Earendel 离职）— https://factorio.com/blog/post/fff-440
- [22] Earendel（Patreon）: "I'm a Factorio developer now!"（2021-02）— https://www.patreon.com/posts/im-factorio-now-47218319
- [23] Steam 社区讨论（2016-03，上 Steam 前官网约 11 万份，非官方口径）— https://steamcommunity.com/app/427520/discussions/0/412449508287273362/
- [24] Factorio Blog: "Friday Facts #171 - So long 2016"（2016-12-30，"85% of all sales in the last 12 months"、2016 年增员 6 人）— https://www.factorio.com/blog/post/fff-171 ；TechRaptor: "Factorio Has Sold Over 1 Million Copies" — https://techraptor.net/gaming/news/factorio-has-sold-over-1-million-copies
- [25] Factorio Blog: "Friday Facts #247 - Pricing and its exploits"（2018-06-15，销量曲线与 GOG 区域定价套利）— https://www.factorio.com/blog/post/fff-247
- [26] LEVVVEL: "How many copies did Factorio sell? — 2026 statistics"（第三方估算，Steam 500 万+）— https://levvvel.com/factorio-statistics/ ；Raijin: Factorio: Space Age Sales & Revenue（第三方估算）— https://raijin.gg/app/645390/Factorio_Space_Age/sales-revenue
- [27] Factorio Forums: "Pirating Factorio"（kovarex 盗版表态）— https://forums.factorio.com/viewtopic.php?t=1821 ；"Pirating as a 'demo'. Your opinions?" — https://forums.factorio.com/viewtopic.php?t=4020
- [28] Factorio Wiki: "Kovarex enrichment process" — https://wiki.factorio.com/Kovarex_enrichment_process
