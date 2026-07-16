# Pieter Levels（Nomad List / PhotoAI）

> 给数字游民和独立开发者做"自己就是第一个用户"的小产品，一个人 + 一群机器人运营 ｜ nomads.com / photoai.com / remoteok.com / levels.io ｜ Pieter Levels（@levelsio，荷兰人）｜ 2014 年起 ｜ 1 人、零员工 ｜ solo / pure-bootstrap / build-in-public / AI 快速转向 ｜ 媒体口径 ~$3M/年，公开面板各产品月收入长期在 $15–30 万区间波动 [23][9]

## 缝隙切入点

- 2014 年他在清迈的网吧里想解决自己的问题：哪个城市房租便宜、WiFi 快、适合远程工作？信息散落在过期的博客和论坛帖里。他做了一张 Google 表格自己填，忘了设权限保护——几天内陌生人开始往里加数据 [5]。这张表格后来变成 Nomad List。
- 他的选题方法从来不是市场调研，而是"我自己需要什么"：数字游民选城市（Nomad List）、找远程工作（RemoteOK，2015 年从 Nomad List 用户需求里长出来）、给自己拍 AI 照片（PhotoAI）[2][10]。
- 更底层的缝隙是方法论本身：2014 年 3 月他公开承诺 "12 startups in 12 months"——每月上线一个带支付功能的完整产品，不是原型。动机是治自己的病："创作者是完美主义者，永远在开新坑、从不发布"，他的原话："By doing nothing, you figure out exactly nothing" [1]。
- 12 个月挑战的实际战绩：上线约 8 个项目，没做满 12 个 [1]。第一个 Play My Inbox（邮件音乐播放列表）零收入；GIF 翻页书毛利只有 2–3%，交完税亏钱；Go Fucking Do It 做到 $500/月 [2]。但其中跑出了 Nomad List 和 RemoteOK 两个百万美元级业务。
- 他 2021 年 11 月的著名复盘推文："Only 4 out of 70+ projects I ever did made money and grew. >95% of everything I ever did failed. My hit rate is only about ~5%. So...ship more" [3]。赚钱的四个：Nomad List、RemoteOK、Interior AI、Photo AI。

## 时机

- 三次踩点都极准。2014 年：远程办公第二波兴起，Nomad List 的众包表格发出后 24 小时内约 100 人填入城市数据，一个月后正式产品上线 [5]，随即"意外地"同时冲上 Product Hunt 和 Hacker News 双第一 [6]。
- 2022 年 9 月 Stable Diffusion 开源发布，他几周内就开始把玩；10 月上线 Interior AI（第一周 $10K）；11 月上线 AvatarAI，头 10 天收入超过 $100,000 [11]。从新模型发布到收费产品上线，以周计。
- 2025 年 2 月："vibe coding" 风口起点。他用 Cursor + Claude + Grok 3 花 3 小时写出浏览器多人飞行游戏 fly.pieter.com，第 3 天被马斯克转发（"Wow, this is cool. AI gaming will be massive"），17 天做到 $1M ARR（$87K MRR，32 万玩家），靠卖游戏内广告位（$5,000/月/个）变现 [13]。他自己说这是他所有项目里涨得最快的一次 [13]。

## 差异化

- 技术栈是反差异化的差异化：不用任何框架，"It's PHP and jQuery, yes, and SQLite... It's a really simple stack and you get stuff done really fast with that"；他嫌 JS 框架每次升级都要重写，"PHP just stays the same and works" [4]。
- 全部产品跑在一台 Hetzner VPS（Ubuntu + Nginx）上，共享成本 $500/月 [12][9]。Interior AI 的 GPU 账单 $200/月，出 21,000 张图，单张约 1 美分，利润率 >99% [12]。
- 一人全栈："I'm a designer, I'm the developer, I make everything, I make the logo" [4]。没有法务、没有审批、没有会议，所以能以天为单位转向。
- 验证标准只有一个——付款："They need to take out their credit cards, pay me money, and then I can see if the idea is validated" [4]。

## 第一批用户/冷启动

- Nomad List 冷启动就是那条 2014 年 6 月 24 日的推文 + 公开表格：24 小时约 100 人众包填数据，等于用户先把产品内容做出来了，他再用这些数据搭网站 [5]。
- 上线后同登 Product Hunt 和 Hacker News 第一，他专门写过一篇《How I got my startup to #1 on both Product Hunt and Hacker News by accident》[6]。
- 之后的每个新产品都不再需要冷启动——他的 X 账号本身就是渠道。他 2025 年 3 月自陈："150,000 tweets. 37 tweets per day every single day for 10+ years. Distribution that I spent 1/3rd of my life to get!" [17]。fly.pieter 的 17 天 $1M ARR 完全建立在这个既有分发上 [13]。

## 收入与定价

- 结构（时间点各异）：PhotoAI 2025 年 9 月创纪录 $150,000/月，2,573 个活跃订阅者，87% 利润率，"100% bootstrapped + $0 funding"，"Employees: 1 = just me on my laptop"，他特意标注这花了"2 年 7 个月 14 天" [9]。PhotoAI 2023 年 2 月 10 日上线，第一周约 $5.4K MRR，第 18 个月破 $100K MRR [10]。
- Nomad List 会员制：终身会员一次性付费，价格多年在 $99–$300 区间反复调整实验 [22]；2016–17 年前后会员费收入 $15,000–25,000/月，RemoteOK 约 $10,000/月、月访问近百万，是当时世界最大的远程工作站 [2]。
- 《MAKE》书：$29.99 起，累计卖出 31,975+ 册、约 $942,548 收入（销售页上挂着实时计数器，本身就是 open startup 式营销），Product Hunt 年度书 [16]。
- 媒体普遍口径是"$3M/年、零员工" [23]。注意各产品公开面板数字波动很大（AvatarAI 从 $100K/10 天到归零；fly.pieter 峰值 $87K MRR 后回落），"~$3M/年"应理解为高位年份的合计。

## 内容与增长

- 他是 "Open Startup" 概念的发明者和招牌：2018 年 2 月宣布 "Nomad List is now an Open Startup™ sharing all its revenue and stats openly" [7]，收入、流量、用户数全部公开在 /open 页面。他自己承认这就是营销手段（"There's no denying it's a marketing tactic"），效果是不投一分钱广告、靠真实数字和过程本身获得信任与传播 [8]。这套玩法直接催生了后来整个 "build in public" 运动 [8]。
- 增长引擎 = 高频公开叙事：每天 30+ 条推文，发布、涨跌、故障、争议全部直播 [17]。每次收入里程碑推文本身就是获客事件（PhotoAI $150K/月那条自带完整技术栈和利润率，等于产品广告）[9]。
- 反面：openstartup 面板也给了模仿者完整的商业情报，行业观察者认为"open startup 的黄金时代已经结束"，多数跟风者已关闭面板，他是少数坚持者 [8]。

## 社区

- Nomad List 本质是"数据 + 付费社区"：付费会员才能进它的聊天社区（Slack 起家，#nomads 超过 1 万名数字游民），并解锁线下 meetup——官方页面列过 543 场早午餐、咖啡、coworking 聚会 [22]。
- 社区就是护城河：城市数据可以被抄，但"世界各地的游民都在这个群里"抄不走。2025 年他把域名升级为 Nomads.com 完成品牌化 [21]。

## 留存

- 终身会员制是他对留存问题的非典型解法：一次性把 LTV 收进来，不跟月度流失率搏斗，同时用社区和持续更新的城市数据把人留在产品里 [22]。
- 压力测试：2020 年 3 月疫情爆发，旅行停摆，Nomad List 收入跌掉 50% 以上；同一个人的 RemoteOK 却因远程工作普及反而受益——同一组合内天然对冲 [18]。

## 转型

- 他的转型速度建立在"沉没成本极低"上：AvatarAI 上线 10 天赚 $100K，随后 Lensa（融资公司）入场碾压，他不硬拼，观察到用户真正想要的是逼真头像而非艺术化头像，直接推倒重做成 PhotoAI（2023 年 2 月）[11][10]。死一个产品的成本是几周时间和一台服务器的分摊费用。
- 更早的转型：2013 年他的 YouTube 频道（电子乐 mix）收入崩掉，人陷入抑郁，"12 startups in 12 months" 本身就是那次转型的自救方案 [2]。
- 2025 年又一次：AI 写代码成熟后，他 3 小时做出飞行游戏，转向"AI 游戏 + 广告位"这种全新变现形态 [13]。模式识别：每次底层技术变化（远程办公、Stable Diffusion、LLM coding），他都用最小可收费产品在几周内进场。

## 如何保持小

- 员工数：0（他把自己算作唯一"员工"）[9]。替代方案是机器人：一台服务器上 187 个 cron 脚本跑天气抓取、职位处理、退款等所有运营，"you can run entire businesses now with robots, with scripts doing stuff for you" [2]。RemoteOK 实现 100% 自动化，Nomad List 约 90% [2]。
- 自动化的代价他也公开写过：《How Automation Left Us Feeling Empty》——机器人接管后"没事可做"反而带来身份认同的空虚 [14]。
- 拒绝融资："I don't really raise money, I don't use VC funding, I do everything myself"；他说很多拿了 VC 的创始人朋友私下告诉他"next time, if I'm going to do it, I'm going to do it like you, because it's more fun, it's more indie, it's more chill" [4]。他不想做 $100M 公司——那只会稀释他 100% 的持股，最后到手可能更少 [20]。（注：他自己反而开了 levels.vc 对外投资，只出不进 [24]。）
- 拒绝收购：99% 的收购意向不严肃；唯一一次走完 6 个月尽调，发现对方只是想套他的客户名单，从此不再谈 [20]。他把一次收购接洽直接发成段子："Big company messages me to acquire Nomad List, I ask how much? 'we usually discuss price last' 😂" [19]。
- 拒绝会议和一切私信：邮箱不看、全平台 DM 关闭多年、播客和媒体采访基本拒绝，只回公开推文。理由是算术题："If I'd reply to the ~50 messages I get per day, and spend 5 minutes per message on them, it'd take me 4 hours"——那就没时间做产品了 [15]。

## 开放问题（值得当面问本人的）

1. PhotoAI 一度占你收入的大头，而 Google/OpenAI 随时可能把逼真人像做成原生免费功能——你给单一产品设过"撤退线"吗？信号是什么？
2. 你在《automation void》里写过自动化之后的空虚 [14]。十年过去，现在每天推着你发 37 条推文、继续 ship 的到底是什么——无聊、身份认同，还是维护那份"花了 1/3 人生换来的分发资产"？
3. 有没有一个数字能让你卖掉 Nomads.com？那次 6 个月尽调被骗客户名单之后 [20]，你对"认真买家"的判断标准变成了什么？
4. Open startup 面板挂了快十年，同行大多关掉了 [8]——2026 年它带来的抄袭、税务和安全麻烦 vs 营销收益，净值还是正的吗？你为什么还留着？
5. 在 AI 三小时能写出一个游戏的时代 [13]，"12 startups in 12 months" 这套方法论哪些部分失效了？如果 2026 年重来，你会把约束改成什么——12 天 12 个，还是别的？

## 来源

1. https://levels.io/12-startups-12-months （2014-03）
2. https://levels.io/startups （演讲整理，约 2016–17）
3. https://x.com/levelsio/status/1457315274466594817 （2021-11）
4. https://lexfridman.com/pieter-levels-transcript/ （Lex Fridman Podcast #440，2024-08）
5. https://www.marketergems.com/p/how-google-spreadsheet-became-digital-nomad-platform
6. https://levels.io/product-hunt-hacker-news-number-one/
7. https://x.com/levelsio/status/968219339588493312 （2018-02）
8. https://testimonial.to/resources/the-golden-era-of-being-an-open-startup-is-gone
9. https://x.com/levelsio/status/1970858876212756506 （2025-09）
10. https://www.indiehackers.com/post/photo-ai-by-pieter-levels-complete-deep-dive-case-study-0-to-132k-mrr-in-18-months-3a9a2b1579
11. https://thecreatorsai.com/p/how-solopreneuer-is-making-12m-arr
12. https://x.com/levelsio/status/1773443837320380759 （2024-03）
13. https://x.com/levelsio/status/1899596115210891751 （2025-03）
14. https://levels.io/automation-void/
15. https://levels.io/contact-levelsio
16. https://readmake.com/ （2026-07 查看）
17. https://x.com/levelsio/status/1902664111445454911 （2025-03）
18. https://blog.openstartuplist.com/pieter-levels-corona-virus-nomadlist-remoteok/ （2020）
19. https://x.com/levelsio/status/1419683547112087554 （2021-07）
20. https://cheekypint.substack.com/p/a-cheeky-pint-with-serial-entrepreneur
21. https://smartbranding.com/nomad-list-rebrands-to-nomads-com-representing-millions-of-digital-nomads-worldwide/ （2025）
22. https://nomads.com/faq
23. https://www.fast-saas.com/blog/pieter-levels-success-story/
24. https://levels.io/vc
