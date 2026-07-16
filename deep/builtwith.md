# BuiltWith（Gary Brewer）

> 把"右键查看网页源代码猜技术栈"这个程序员的手工习惯，做成覆盖近 5 亿域名的自动化数据库，再把数据库卖给销售团队当线索清单 ｜ builtwith.com ｜ Gary Brewer（悉尼）｜ 2007-07（点子诞生于 2007-07-22 周日下午，当天注册域名）[1] ｜ 约 1 人全职（Gary 一人写码 + 运营；Andrew Rogers 以纯股权身份任顾问；一名英国兼职博客写手）[2][3][4] ｜ 数据 / 销售情报 / SaaS / pure-bootstrap ｜ 【传闻】~$14M/年（见"收入与定价"的溯源分析，从未被本人确认）[4][12][13]

**档案说明**：Gary Brewer 是全网"闷声赚钱"叙事的头号样本，但他本人 19 年来几乎不接受采访、从不公布财务数字。本档案将【实据】（本人访谈、BuiltWith 官方博客、共同创始人文章、TechCrunch 报道、官网抓取）与【传闻】（第三方推算、社交媒体疯传）分开标注。最核心的发现：疯传的 "$14M/年、零员工" 没有任何第一手来源，且共同创始人 2015 年就公开提醒媒体数字失真 [2]。

## 缝隙切入点

- 2007 年，Gary 在悉尼科技圈的早期创业者聚会（Mick Liubinskas 组织的活动）上看到一批 startup，回去挨个访问它们的网站、右键看源代码，猜它们用什么技术搭的 [5][6]。他发现这件事没人做成自动化工具："I realized no one was doing this in an automated friendly to use way and thought I'd create it and that day the idea was born!" [6]
- 域名即定位："because builtwith.com was still available and it answers the question, 'what is this site built with?'" [6]——产品名字本身就是那个问题。
- 但真正的生意藏在好奇心背后：免费查询满足好奇，付费产品是"把数据当销售线索清单卖"——比如 Mailchimp 的竞争对手可以拉出所有用 Mailchimp 的网站列表去挖客户；对冲基金拿技术采用率数据做市场分析；记者拿它做调查 [4]。缝隙的本质：**技术栈探测是入口，销售情报（sales intelligence）才是付费理由**——而这个理由 Gary 自己花了六年才想明白（见"转型"）。

## 时机

- 2007 年正是 Web 2.0 技术栈大爆炸的年代：CMS、分析工具、JS 库、托管商开始多到"看源代码猜"成为普遍需求，而当时没有任何自动化探测工具 [5][6]。第一个动手的人独占了这个品类的域名、SEO 和心智。
- 更重要的时机红利是**复利型的**：BuiltWith 每周爬全网并保留历史快照，19 年下来积累了任何后来者都无法回填的时间序列数据——2012 年 TechCrunch 报道时是 1.3 亿网站、约 2,000 种技术 [7]；2026 年官网标称 491.9M 域名、122,201+ 种技术、18 年以上技术趋势史 [8][9]。数据护城河随时间自动变宽，这是"长跑 19 年"本身构成竞争力的罕见生意。
- 变现的时机则踩在 2011-2013 年 SaaS 销售情报市场成形期：TechCrunch 2012 年报道 Trends Pro 时，"按技术找客户"刚刚成为增长团队的标准动作 [7]。

## 差异化

- 对比最直接的竞品 Wappalyzer（众包模式，靠 250 万+ 浏览器插件用户上报数据）：BuiltWith 坚持自建定时爬虫，覆盖面碾压——同查 Stripe 用户，Wappalyzer 显示 30 万+ 网站，BuiltWith 显示 130 万+ [14]。【第三方评测，注意利益相关】代价是新鲜度和前端识别准确率略逊（一项 500 个电商站的测试中 Next.js 识别率 82% vs Wappalyzer 94%）[14]。
- 历史数据是独家资产：官网标称技术趋势数据可回溯 18 年以上（部分域名数据回溯到 1985 年）[8][9]——"某公司哪年从 Magento 迁到 Shopify"这类问题只有 BuiltWith 能答，服务于竞争情报和投资研究场景 [14]。
- 技术选型的差异化是"反差异化"：Gary 用最早学会的 ASP.NET 一路写到底，"Sticking with what you know has been useful and not getting carried away with cutting edge tools" [6]；"If you keep changing things to the latest and greatest product, you never really fully understand how it works" [11]。一个人维护如此大的爬虫系统，靠的是无聊的技术栈。

## 第一批用户/冷启动

- 2007 年 8 月（上线约一个月后）：Gary 主动给 ReadWriteWeb 提供"独家报道"，同时冲上当时最大的社交分享站 Digg 第一名 [1][5]。他给"网站同时在线 500 人"的统计截图拍了张照留念 [4]。
- 决定性的一击是运气+产品可传播性：AboutUs.org（域名目录 wiki，创始人 Raymond King）的人发现 BuiltWith 后，在其被 Google 收录的数千万个域名页面上都加了指向 builtwith.com 的链接——流量 10 倍增长，更关键的是给了 BuiltWith 至今受益的搜索引擎权重 [5][12]。
- 传播机制自带病毒性："It's a cool thing to be able to show someone, so that has helped spread the word."（Starter Story 转述）[5]——查任何网站的技术栈，结果页天然是可分享的谈资。
- 但流量≠收入：上线后近四年只是业余项目，Gary 白天上班、每晚写代码，持续了 4 年 [4][11]。第一封"我想付费"的客户邮件，他因为不敢相信，**晾了一个星期才回** [1]。

## 收入与定价

- 【实据】收入轨迹的可靠锚点只有两个：
  - 2011 年（Andrew Rogers 初见 Gary 时）：$40k/月，约 $480k/年，当时还是业余项目 [2][4]。
  - 2015 年（StartupDaily 报道）：付费客户"2,000-3,000 之间"，三档定价 $299/$495/$995 每月，客户分布约 40% Basic / 40% Pro / 20% Enterprise；月活用户 50 万+，月 PV 约 200 万；客户包括 Google、New Relic、Twitter [3]。
- 【传闻溯源】"$14M/年"的疯传路径：按 2015 年公开数字推算（2,500 客户 × 加权均价约 $470/月 ≈ $14M/年），最早成型于 Colin Keeley 的博客文章（无日期标注，约 2020 年，未给出处）[4]，经 Nathan Barry（2022-12）[12]、Deedy（2025-12，称"ONE employee and brings in $14M+"）[13] 等推文放大成"事实"。**Gary 本人从未确认过任何营收数字**。更要命的是：Andrew Rogers 2015 年就发文提醒，StartupDaily 的数字因为"累计客户数 vs 当前订阅数"的口径混淆而偏高 [2]——也就是说，$14M 推算的地基本身被共同创始人打过折。Starter Story 目前标注的 "$22.6M/年" 是其模型估算值，可信度更低 [5]。
- 【实据】定价 19 年近乎冻结：2015 年 $299/$495/$995 [3]，2026 年官网 Basic $295 / Pro $495 / Team $995（另有 Team Ultra），个人单站查询"free to use for individual site lookups forever" [8]。**没有低价档**——直接从 $0 跳到 $295/月，天然过滤掉高支持成本的小客户，这是"零客服"得以成立的定价前提。
- 【实据】成本侧的第一手线索极少：起步时是 $8/月的共享 ASP.NET 主机 [1]；如今官网提到基础设施分布在 OVH、AWS、Google Cloud [10]。"几乎零成本"是传闻，爬近 5 亿域名的爬虫+存储成本不可能为零，但一人公司无人力成本是实据。

## 内容与增长

- 增长引擎就是免费工具本身："The free tool is what gets most paid users signing up." [4] 免费查询页 + 每种技术的公开趋势页构成了海量 SEO 落地页，AboutUs 事件又给了域名权重 [5][12]。
- 【传闻】流量结构：约 57% 直接访问、36% 搜索、0% 付费投放（第三方文章引用流量工具数据）[12]。方向上与"零营销预算"的叙事一致。
- 内容投入的全部：一名英国兼职 contractor 每周写博客 [3][4]。没有销售团队、没有投放、没有增长团队 [3][4]。
- Gary 对增长的态度并非"佛系"，而是清醒的工程师自省："Growth is only going to happen if more people know about your product"；对技术型创始人，"the hurdle is doing the things that aren't as much fun as the programming/engineering side of things... These boring bits always get put at the bottom of the TODO list but have the greatest effect on growth." [6]

## 留存

- 反直觉设计：Gary 刻意**把退订做得尽可能容易**——"make unsubscribing as easy as possible so he has less to do"，省下的时间拿去做新功能 [4]。用产品留人，不用流程留人。
- 结构性留存来自数据的保鲜属性：技术栈数据每周都在变，销售线索用完即旧，订阅续费买的是持续更新——数据业务天然是订阅制的形状 [7][8]。
- CRM 集成（Salesforce、HubSpot、Zoho、Dynamics 365）把 BuiltWith 数据焊进客户的销售工作流 [8]，切换成本随使用加深。

## 转型

BuiltWith 是"六年找不到商业模式，但免费工具一直有人用"的教科书案例，官方博客 10 周年文章罕见地披露了完整弯路 [1]：

1. **2007-2008**：首页挂自制广告系统卖广告位——收入寥寥 [1]。
2. **2008**：做 Website Optimizer（SEO 优化建议工具）尝试收费——失败 [1]。
3. **2008-2009**：不务正业做了 TwitLinks、TwitTruth、TwitTrading 三个 Twitter 周边项目——全部无疾而终；官方博客自称这段是 "Trough of Sorrow"（绝望低谷）[1]。
4. **低谷谷底**：把 BuiltWith 挂上 Flippa 出售——没卖成 [1]。**今天疯传"$14M 印钞机"当年差点几千美元卖掉。**
5. **转折**：收到第一封付费意向邮件（晾了一周）；在 Tjoos 兼职时，其创始人点醒他"专注做客户愿意付钱的东西"[1]。
6. **2011-2012**：推出 BuiltWith Trends 和 Pro 按次付费报告；TechCrunch 报道后听编辑建议改为订阅制 [1][7]。
7. **2013**：产品市场契合，Gary 全职投入（此时距创立已六年）[1]。官方原话："It took roughly six years to get to a point where it actually found a business purpose beyond free technology lookups." [1]

## 如何保持小

- 明确的意愿而非阶段："Gary didn't want employees... The business wasn't just about money. It was about creating a business that matched the founder."（Colin Keeley 转述）[4]
- Andrew Rogers（2011/2012 年相识，两处来源年份不一 [1][2]）以纯股权、不领薪的方式加入，主要贡献是劝 Gary 辞职全职 + 做客户调研，后来退到每月开一次会的顾问角色；他自己写道："BuiltWith remains Gary's baby not mine." [2]
- 两人当年设的招人门槛："$100k per month revenue" 才考虑招第一个程序员 [2]——按传闻收入早已越过，但至今没招。2012 年 Gary 曾对 TechCrunch 说在筹建销售团队 [7]，此事再无下文——这是档案里最值得当面追问的"未走之路"。
- 客服自动化到极致：每天只花几小时回复；常见问题甩知识库链接；新问题录一段 20 秒视频，之后同类问题复用 [4][12]。指标也极简：只看试用注册、付费注册、报告生成数、客户数 [4]。
- 性格底色：报道者形容他 "very softly spoken"（说话轻声细语）；他把公司几乎完全握在自己手里，理由朴素——"it's just easier and faster this way"（大意：这样更简单更快）[11]。【注：此引语转自搜索摘要，原文页面无法直接验证，措辞可能有出入】
- 低调本身可能就是策略的一部分：不融资（2012 年他说 "hasn't ruled out taking funding but for the time being wants to see how far he can get by bootstrapping" [7]，此后 14 年再未提过）、不公布数字、不接受播客采访——没有对外承诺，就没有增长的义务。

## 开放问题（值得当面问创始人的）

1. 全网传了快十年的 "$14M/年、近乎零成本"，你从未确认或否认。愿意给一个量级或区间吗？更有价值的是成本结构：每周爬近 5 亿域名的基础设施，占营收百分之几？
2. 2012 年你对 TechCrunch 说在筹建销售团队，后来为什么没建？你和 Andrew 定过"月入 $100k 才招工程师"的门槛，早已越过却始终没招——是哪一刻让你确定"一个人"不是阶段而是终点？
3. 19 年里 ZoomInfo、SimilarWeb、Semrush 这类买家一定找过你。除了早年挂 Flippa 那次，最接近卖掉是什么时候？为什么留下？
4. Wappalyzer 用 250 万浏览器插件做众包，你坚持自建爬虫。19 年后回看，真正的护城河是历史数据、指纹库、还是别的？LLM 时代爬虫成本骤降，这条护城河在变宽还是变窄？
5. 极端低调是深思熟虑的策略，还是纯粹性格？"从不接受采访、从不公布数字"对这门生意是保护、加分，还是无所谓？

## 来源

1. BuiltWith Blog, "10 Years of BuiltWith"（2017-07-17，第一手官方回顾）：https://blog.builtwith.com/2017/07/17/10-years-of-builtwith
2. Andrew Rogers（共同创始人）, "The Story of BuiltWith", Medium（2015-10-03）：https://medium.com/@andrewjrogers/the-story-of-builtwith-e3bbc17c239f
3. Startup Daily, "BuiltWith is perhaps one of Australia's most profitable online companies and has zero staff"（2015-09-30）：https://www.startupdaily.net/advice/builtwith-is-perhaps-one-of-australias-most-profitable-online-companies-and-has-zero-staff/
4. Colin Keeley, "The Story of BuiltWith: 1 Employee, $14m+ ARR"（无日期，约 2020；$14M 说法的主要源头，未注明出处）：https://www.colinkeeley.com/blog/the-story-of-builtwith-1-employee-14m-arr
5. Starter Story, "How Gary Brewer Stumbled Into A $14M Idea Profiling Websites"（营收数字为其模型估算）：https://www.starterstory.com/stories/builtwith-technology-lookup-breakdown
6. CrazyEngineers, Gary Brewer 书面访谈（少数本人直接受访记录之一）：https://www.crazyengineers.com/founders-circuit/gary-brewer-builtwith
7. TechCrunch, "BuiltWith Reveals The Tech Used By The 130 Million Web Sites That Matter Most"（2012-02-16）：https://techcrunch.com/2012/02/16/builtwith-reveals-the-tech-used-by-the-130-million-web-sites-that-matter-most/
8. BuiltWith 官网定价页（2026-07 抓取）：https://builtwith.com/plans
9. BuiltWith 官网首页（2026-07 抓取）：https://builtwith.com/
10. BuiltWith 官网 About 页（2026-07 抓取）：https://builtwith.com/about
11. HostingAdvice, "The Man Behind BuiltWith: How a Hobby Became a Global Business"（原页面反爬 403，引语转自搜索摘要，措辞待核）：https://www.hostingadvice.com/blog/builtwith-more-than-how-websites-are-made/
12. Louie Chen, "How BuiltWith generates $14 million a year with zero employees", Medium（二手汇编，AboutUs 细节较全）：https://medium.com/@gmitslouie/how-builtwith-generates-14-million-a-year-with-zero-employees-f53a87e40f0a
13. Deedy Das 推文（$14M 叙事的近期放大节点）：https://x.com/deedydas/status/2040806740040831379 ；Nathan Barry 推文（2022-12）：https://x.com/nathanbarry/status/1605948720063090688
14. 竞品对比（第三方评测，各有利益相关，交叉参考）：ZoomInfo "BuiltWith vs. Wappalyzer" https://pipeline.zoominfo.com/sales/builtwith-vs-wappalyzer ；bloomberry "5 BuiltWith alternatives" https://bloomberry.com/blog/5-builtwith-alternatives-for-technology-intelligence/ ；technologychecker.io "BuiltWith Alternatives" https://technologychecker.io/blog/builtwith-alternatives
