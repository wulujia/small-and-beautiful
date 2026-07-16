# Mike Perham — Sidekiq

> L2 创始人资料库 · 聚焦本人公开表达
> 调研日期：2026-07-16 · 调研人：Nix
> 一句话画像：商业开源的教科书样本。2012 年写出 Ruby 后台任务框架 Sidekiq，用"开核（open core）"模式一个人做到年营收接近千万美元、零员工、零融资；他把"能一个人跑"写进每一条商业政策，把"公平定价 + 拒绝捐赠式生存"讲成方法论，晚年开始公开思考项目身后事。

## 账号全集

- 个人博客：https://www.mikeperham.com/ （2007 年写到现在，500+ 篇；每年的 Sidekiq 生日帖 + 大版本发布帖是这家公司最完整的编年史）
- Mastodon（主账号，Ruby/工作）：**@getajobmike@ruby.social** https://ruby.social/@getajobmike
- Mastodon（生活/城市规划侧账号）：**@getalifemike@urbanists.social** https://urbanists.social/@getalifemike （博客页脚自列，见 https://www.mikeperham.com/）
- Bluesky：**@mike.perham.net** https://bsky.app/profile/mike.perham.net （2024-08-31 注册；bio："Software engineer, biking + housing advocate in Portland, OR"，来源：Bluesky 公开 API）
- X/Twitter：@getajobmike https://twitter.com/getajobmike （已基本弃用，表达阵地转 Mastodon/Bluesky）
- GitHub 个人：https://github.com/mperham ；项目组织：https://github.com/sidekiq 、https://github.com/contribsys （Faktory）
- Hacker News：**mperham** https://news.ycombinator.com/user?id=mperham （580+ 条评论，2026 年仍活跃；多条谈营收/不雇人的高含金量发言，见"语录"）
- 产品站：https://sidekiq.org/ ；公司站（Contributed Systems / Contribsys，Faktory 所在）：https://contribsys.com/
- Email：mike@perham.net（博客页脚公开）
- 演讲档案：https://www.rubyevents.org/profiles/mperham

## 访谈清单

1. **2013-06-07 · The Changelog Interviews #92：Sidekiq and Ruby** · https://changelog.com/podcast/92
   - 早期访谈：Sidekiq、Dalli、girl_friday 等项目与"可持续开源"话题
   - 当时 Sidekiq Pro 商业化刚满一年（首年约 $70k 销售额）
   - 自述编程偶像是 Celluloid 作者 Tony Arcieri

2. **2017-05-31 · Indie Hackers Podcast #016：Building a $1 Million Business Solo** · https://www.indiehackers.com/podcast/016-mike-perham-of-sidekiq
   - 当时约 $80k/月营收、约 800 客户、零员工；Pro $1,000/年、Enterprise $2,000/年
   - 自称 "accidental entrepreneur"：只是想解决"为爱发电几千小时分文不赚"的问题
   - 成功的秘密是时间：辞职前用 18 个月、每周约 20 小时打磨，不给自己"6 个月内必须成"的死线
   - "There's plenty of money for one person if you can make a difference as one person."
   - 不做销售：90% 的订单成交前他没跟客户说过一句话；要折扣的人注定是最差客户

3. **2020-02-03 · Maintainable Podcast：How Developers Underestimate Long-Term Costs of External Dependencies** · https://maintainable.fm/episodes/mike-perham-how-developers-underestimate-long-term-costs-of-external-dependencies
   - 外部依赖的长期成本被系统性低估（与其名文 Kill Your Dependencies 一脉相承）
   - 如何在开源项目上长出一门生意；维护 Ruby 项目 vs Go 项目的差异

4. **2020-02-19 · The EmberMap Podcast Ep.88：Sustaining Open Source with Sidekiq and Faktory** · https://embermap.com/podcast/mike-perham-on-sustaining-open-source-with-sidekiq-and-faktory （视频：https://www.youtube.com/watch?v=VruWGJ27rUo）
   - Sidekiq 的商业模式如何供养他 10+ 年的全职开源开发
   - Faktory：把同样的能力带给任意语言（含 JS）的新赌注

5. **2020-09-07 · Computer Science: Just the Useful Bits：Sidekiq and Whitepapers and What Success is For** · https://justtheusefulbits.com/jtub/mike-perham-sidekiq-and-whitepapers-and-what-success-is-for/
   - "The whole point of becoming a success is not having to work very hard and getting to enjoy your life therein."——成功的意义是不必再拼命
   - 职业转折：从资深 Java 工程师归零改学 Ruby（"a tough career shift"）
   - 现状的双刃剑：他写的每行代码几乎立刻跑在几千家公司的生产环境里

6. **2021-03-05 · Remote Ruby：Building a Business on Rails with Mike Perham** · https://remoteruby.com/119 （视频：https://www.youtube.com/watch?v=5g3cOtYF6oQ）
   - 在 Rails 生态上建立一人公司的完整叙事（41 分钟）

7. **2022-04-14 · alphalist.CTO Podcast #49：Creator of Sidekiq** · https://alphalist.com/podcast/49-mike-perham-creator-of-sidekiq-faktory
   - 当时数据：约 **$4M ARR，年增 20%**，一人运营
   - 独立开发者要警惕依赖 VC 支持的或无商业模式的开源项目（它们会死）
   - Bootstrap vs 融资：他选择不拿一分钱外部资本

8. **2023-04（文字访谈）· Code Code Ship：From Employment to Independence** · https://codecodeship.com/blog （HN 讨论 201 分：https://news.ycombinator.com/item?id=35566768）
   - 谈 Sidekiq 为何经久不衰；配套 HN 跟帖中他自曝"营收更接近 $10M 而非 $1M"、约 2000 客户
   - 关键细节：在 The Clymb 任职时提前在雇佣合同里谈好 IP 豁免条款（IP carve-out），保证 Sidekiq 归自己所有

9. **2023-05-16 · Startups For the Rest of Us #661：Millions in Revenue As a One-Person Software Company**（Rob Walling） · https://www.startupsfortherestofus.com/episodes/episode-661-millions-in-revenue-as-a-one-person-software-company
   - 不雇人的原话最全的一期："I didn't want to hire people, period. I don't want to be a manager."
   - 所有商业政策围绕一个问题设计：怎么把 Mike 的时间当稀缺资源保护起来
   - 定价心法：$1,000/年是刻意卡在多数公司"超过一千美元要 VP 审批"的信用卡红线之下
   - "十年才成的一夜成名"：Sidekiq 之前他试过的东西全没成
   - 知足哲学："I don't need more… desire is a root of pain."（佛教心态）

10. **2023-11-20 · Software Sessions：Mike Perham on keeping it solo（RubyConf 2023 现场，有全文 transcript）** · https://www.softwaresessions.com/episodes/keeping-it-solo/
    - "I explicitly create business policies so that I can run solo."——solo 不是结果，是被设计出来的
    - 不雇人的技术理由：Sidekiq 与他本人的 Ruby/线程知识深度绑定，雇人也接不住
    - "Sometimes the best thing in business that you can do is just say no."（挑客户）
    - 对开源资助的立场：钱让项目更可持续，但"我们需要在纯资本主义之外寻找其他融资形式"；警惕依赖 VC 背景的商业基础设施

11. **2023-11-22 · saas.unbound（saas.group）：Bootstrapping a SaaS to $7M solo**（主持 Anna Nadeina） · https://saas.group/podcasts/saas-unbound-interview-mike-perham-sidekiq/
    - 标题即数据点：一人做到 $7M
    - 开核模式、可持续定价、社区驱动的产品开发

12. **日期不详（约 2014，文字访谈）· Starting & Sustaining（Garrett Dimon）** · https://startingandsustaining.com/interviews/mike-perham/
    - 围绕"如何启动并持续经营一个 SaaS/产品"的书配套访谈

（另有 The Ruby on Rails Podcast #144 "Mike Perham - Sidekiq & Sidekiq Pro" https://www.therubyonrailspodcast.com/144 ，页面无法抓取、日期未核实，约 2015；Indiedotes Podcast Ep.7 https://player.fm/series/indiedotes-podcast/episode-7-mike-perham 日期未核实。）

## 演讲与公开课

他不是活跃讲者——2012 年后基本不上台，改以赞助商身份出现在 Ruby 大会上，把大会当发布节点和获客场：

- **RubyConf 2012：Asynchronous Processing for Fun and Profit**（38 分钟，唯一广为流传的大会演讲，讲后台任务处理与 Sidekiq 的多线程思路） · https://www.rubyevents.org/profiles/mperham
- **RubyConf 2015**：现场发布 Sidekiq 4.0（赞助商身份） · 出处：他的博客 https://www.mikeperham.com/2017/04/24/sidekiq-at-railsconf-2017/
- **RailsConf 2017**：现场发布 Sidekiq 5.0 + 展位 · https://www.mikeperham.com/2017/04/24/sidekiq-at-railsconf-2017/
- **RailsConf 2020（线上）**：组织 "Virtual Hallway" 云走廊活动 · https://www.mikeperham.com/2020/04/29/railsconf-2020-virtual-hallway/
- **RubyConf 2023（圣迭戈）**：赞助并组织 5k 晨跑、桌游夜、Coffee Swap 等周边活动（见其 events 页 https://www.mikeperham.com/events/ ），并在现场接受 Software Sessions 访谈

## 博客关键文章

### 商业开源方法论
- **The Path to Full-time Open Source**（2014-10-01）：他的完整 playbook——选自己每天在用的关键工具、拆分开源/商业功能、先把开源版做好，卖的是"打包 + 保障"；公布 2012 Q4 $7.5k → 2013 $85k → 2014 预计 $175k 的营收曲线 · https://www.mikeperham.com/2014/10/01/the-path-to-full-time-open-source/
- **How to make $100k in OSS by working hard**（2013-10-01）：Pro 首年卖出约 140 份、$70k，年化约 $100k；结论是收费让维护从苦役变成乐事 · https://www.mikeperham.com/2013/10/01/how-to-make-100k-in-oss-by-working-hard/
- **How to Charge for your Open Source**（2015-11-23）：名句 "The easiest way to make someone value your time and software is to charge for it" 的出处；提出 AGPL 默认 + 付费换 MIT 的双许可机制 · https://www.mikeperham.com/2015/11/23/how-to-charge-for-your-open-source/
- **Indie Developers in Ruby, 2015 Ed.**（2015-02-04）：盘点 Ruby 圈独立开发者生态，他对"同行"的观察 · https://www.mikeperham.com/2015/02/04/indie-developers-in-ruby-2015-edition/

### 定价与产品史
- **Say Hello to Sidekiq Pro**（2012-10-01）：商业化起点；承诺首份销售收入 100% 捐给 Celluloid 作者 Tony Arcieri · https://www.mikeperham.com/2012/10/01/say-hello-to-sidekiq-pro/
- **Sidekiq Enterprise**（2015-08-06）：第二级付费产品线上线，客单价翻倍的关键一步 · https://www.mikeperham.com/2015/08/06/sidekiq-enterprise/
- **Introducing Faktory**（2017-10-24，配套雄文 The Future of Background Jobs，2017-10-23）：把 Sidekiq 模式复制到全语言的第二产品 · https://www.mikeperham.com/2017/10/24/introducing-faktory/ 、https://www.mikeperham.com/2017/10/23/the-future-of-background-jobs/
- **Faktory Enterprise**（2020-01-08）：第二产品也走完 开源→Pro→Enterprise 三级火箭 · https://www.mikeperham.com/2020/01/08/faktory-enterprise/

### 编年史（生日帖系列）
- **Happy Birthday Sidekiq!**（2013-02-05，一周年）：25 个 Pro 客户起步 · https://www.mikeperham.com/2013/02/05/happy-birthday-sidekiq/
- **Happy 2nd Birthday Sidekiq!**（2014-01-31）：下载量 21 万→119 万，Pro 客户 25→200+；"我已达成目标：做出最好的后台任务框架，没有之一" · https://www.mikeperham.com/2014/01/31/happy-2nd-birthday-sidekiq/
- **Happy 6th Birthday, Sidekiq**（2018-02-05）：2017 年营收同比 +40%，"利润可观、有机增长"，明确拒绝投资人式增长目标 · https://www.mikeperham.com/2018/02/05/happy-6th-birthday-sidekiq/
- **Happy 10th Birthday, Sidekiq**（2022-01-17）：十年账本——累计销售 **$13.5M**、1,850 客户、1.15 亿次下载、1 名员工（他自己）；首次公开身后事：2030 年后大概率不再维护，考虑把 Sidekiq 移交 Ruby Central · https://www.mikeperham.com/2022/01/17/happy-10th-birthday-sidekiq/

### 开源可持续性批判 / 生态立场
- **Sustainable Open Source**（2013-06-13）：早期檄文——用户拿走巨大价值，维护者却在免费支持中烧尽 · https://www.mikeperham.com/2013/06/13/sustainable-open-source/
- **Kill Your Dependencies**（2016-02-09）：广为流传的依赖极简主义宣言，"the scourge of dependencies spares no one"；这也是他能一个人维护整个商业产品的工程前提 · https://www.mikeperham.com/2016/02/09/kill-your-dependencies/
- **Sponsoring Hanami**（2025-01-17）：个人出资 $12,000 赞助 Hanami 框架，反对 Rails 单一文化："A diverse ecosystem is a healthy ecosystem." · https://www.mikeperham.com/2025/01/17/sponsoring-hanami/

### 近期动态
- **Introducing Sidekiq 8.0**（2025-03-05）：14 年后仍在发大版本（profiling、job iteration 等） · https://www.mikeperham.com/2025/03/05/introducing-sidekiq-8.0/
- **Sidekiq in the terminal**（2026-03-10）：2026 年仍在活跃开发的证据 · https://www.mikeperham.com/2026/03/10/sidekiq-in-the-terminal/

## 创业时间线

- **2000s**：资深 Java 工程师转行 Ruby，在创业公司打工多年；后任 The Clymb（波特兰电商）工程总监，入职时在合同里谈好 IP 豁免条款，为日后保留 Sidekiq 所有权埋下伏笔（来源：JTUB 访谈；HN https://news.ycombinator.com/item?id=35566768 ）
- **2012-01-16**：Sidekiq 第一个 commit（来源：10 周年帖）
- **2012-02**：v0.5.0 公开发布，LGPL + $50 商业许可双轨；到 10 月共卖出 33 份、$1,650（来源：https://www.mikeperham.com/2013/10/01/how-to-make-100k-in-oss-by-working-hard/ ）
- **2012-10-01**：Sidekiq Pro 上线（约 $500/份），2012 年最后三个月卖了 $7,500（来源：Say Hello to Sidekiq Pro；The Path to Full-time Open Source）
- **2013**：全年销售 $85,000；Pro 首年约 140 份、$70k（来源：同上）
- **2014-01**：下载量 119 万，Pro 客户 200+（来源：2 周年帖）
- **~2014-07**：辞去工作，开源正式成为全职职业；成立公司主体 Contributed Systems（Contribsys）（来源：The Path to Full-time Open Source，"三个月前转全职"）
- **2015-08-06**：Sidekiq Enterprise 发布（来源：博客）
- **2015-11**：RubyConf 2015 现场发布 Sidekiq 4.0（来源：https://www.mikeperham.com/2017/04/24/sidekiq-at-railsconf-2017/ ）
- **2017-04**：RailsConf 2017 现场发布 Sidekiq 5.0（来源：同上）
- **2017-05**：营收约 $80k/月、约 800 客户（来源：Indie Hackers #016）
- **2017-10-24**：发布第二产品 Faktory（全语言后台任务）；2018-12 Faktory Pro、2020-01 Faktory Enterprise（来源：博客）
- **2019-12**：自曝 "Sidekiq makes ~1M/year in gross revenue"（来源：HN https://news.ycombinator.com/item?id=21909849 ）
- **2022-01-17**：十周年：累计销售 $13.5M、1,850 客户、1.15 亿下载；首次公开考虑 2030 年后移交 Ruby Central（来源：10 周年帖）
- **2022-04**：约 $4M ARR、年增 20%（来源：alphalist #49 页面 https://alphalist.com/podcast/49-mike-perham-creator-of-sidekiq-faktory ）
- **2022-10-27**：Sidekiq 7.0 发布（来源：https://www.mikeperham.com/2022/10/27/introducing-sidekiq-7.0/ ）
- **2023-04**："I'm closer to $10m than $1m in annual revenue now"，约 2,000 客户（来源：HN https://news.ycombinator.com/item?id=35566768 ）
- **2024**：以 Ruby Shield 赞助商身份向 Ruby Central 捐 **$250,000**（来源：他本人 HN 评论 https://news.ycombinator.com/item?id=47592885 ；Ruby Central 2024 年 newsletter https://rubycentral.org/news/june-2024-newsletter/ ）
- **2025-01-17**：个人出资 $12,000 赞助 Hanami（来源：博客）
- **2025-03-05**：Sidekiq 8.0 发布（来源：博客）
- **2025**：因 Ruby Central 邀请 DHH 在最后一届 RailsConf（2025-07）压轴演讲，**撤回原计划 2025 年的 $250,000 捐款**；此事后来被广泛认为是 Ruby Central 财务失衡、9 月 RubyGems 接管风波的导火索之一（来源：他本人 HN 评论 https://news.ycombinator.com/item?id=47592885 ；Joel Drapper 报道 https://joel.drapper.me/p/rubygems-takeover/ ；The Register https://www.theregister.com/2025/09/25/open_source_to_closed_doors/ ）
- **2025-10-02**：在 Bluesky 公开认领并解释撤款决定（原文见"语录"）（来源：https://bsky.app/profile/mike.perham.net/post/3m27umijz322k ）
- **2026-03**：仍在活跃开发（Sidekiq in the terminal；HN 上继续参与 RubyGems 风波讨论）（来源：博客；HN）

## 语录

1. 不雇人（管理动机）："**I didn't want to hire people, period. I don't want to be a manager. I don't want to deal with the administrative overhead.**" — Startups For the Rest of Us #661，2023-05-16 · https://www.startupsfortherestofus.com/episodes/episode-661-millions-in-revenue-as-a-one-person-software-company
2. 不雇人（制度设计）："**I still have 0 employees and don't plan to hire. I tune my business processes to run as lean as possible.**" — HN，2023-04 · https://news.ycombinator.com/item?id=35566768
3. solo 是设计出来的："**I explicitly create business policies so that I can run solo.**" — Software Sessions，2023-11-20 · https://www.softwaresessions.com/episodes/keeping-it-solo/
4. 时间即资产："**All of my business policies are based on the fact that how do we treat Mike's time as valuable and not allow the customer to take too much of my time.**" — Startups For the Rest of Us #661，2023 · 同上
5. 公平定价："**I charge what I think is a very fair price. It's only a thousand dollars a year.**" — Software Sessions，2023 · https://www.softwaresessions.com/episodes/keeping-it-solo/ ；定价依据："**I settled on a thousand dollars a year only because so many companies have the credit card policy where anything over a thousand dollars requires a VP sign off.**" — SFTROU #661
6. 反捐赠、要收费："**I don't take donations, I use an open core model and charge companies for access.**" — HN "Software Below the Poverty Line" 讨论，2019-06-13 · https://news.ycombinator.com/item?id=20179484 ；更早版本："**Donations are charity. If you want this to be a sustainable business, ask for people to pay for value.**" — HN，2013-06-21 · https://news.ycombinator.com/item?id=5918824
7. 收费即尊重："**The easiest way to make someone value your time and software is to charge for it.**" / "**But if you don't charge for it, I guarantee you will make no money.**" — 博客 How to Charge for your Open Source，2015-11-23 · https://www.mikeperham.com/2015/11/23/how-to-charge-for-your-open-source/
8. 一人公司的市场空间："**There's plenty of money for one person if you can make a difference as one person. Almost every niche has that potential.**" — Indie Hackers #016，2017-05-31 · https://www.indiehackers.com/podcast/016-mike-perham-of-sidekiq
9. 知足："**I don't need more. I'm happy to support my customers. I very much believe in sort of the Buddhist mindset where desire is a root of pain.**" — SFTROU #661，2023 · 同上
10. 成功的目的："**The whole point of becoming a success is not having to work very hard and getting to enjoy your life therein.**" — Just the Useful Bits，2020-09-07 · https://justtheusefulbits.com/jtub/mike-perham-sidekiq-and-whitepapers-and-what-success-is-for/
11. 营收自曝："**I'm closer to $10m than $1m in annual revenue now.**" — HN，2023-04 · https://news.ycombinator.com/item?id=35566768 ；"**Sidekiq makes ~1M/year in gross revenue.**" — HN，2019-12 · https://news.ycombinator.com/item?id=21909849
12. 价值观高于收入（撤款事件）："**That was me. I rescinded a six-figure grant because the org invited DHH, a white supremacist, to speak. We cannot tolerate hateful people as leaders in our communities.**" — Bluesky，2025-10-02 · https://bsky.app/profile/mike.perham.net/post/3m27umijz322k ；配套事实陈述："**I donated $250,000 in 2024 and withdrew a planned $250,000 donation in 2025, as has been widely publicized.**" — HN，2026-03-31 · https://news.ycombinator.com/item?id=47592885
13. 超越资本主义的开源资助观："**We need to look at other forms of financing beyond pure capitalism.**" — Software Sessions，2023 · https://www.softwaresessions.com/episodes/keeping-it-solo/

## 资料缺口

- **历年营收明细**：只有零散节点（2012 $7.5k → 2013 $85k → 2014 ~$175k → 2017 ~$80k/月 → 2019 ~$1M/年 → 2022-01 累计 $13.5M → 2022-04 $4M ARR → 2023 "closer to $10M than $1M" / saas.group 标题 $7M）；口径混杂（累计 vs 年度、gross vs ARR），无官方逐年数据
- **收购报价史**：从未系统披露是否收到过收购要约及金额；SFTROU #661 等长访谈均未触及"卖不卖"的具体报价——只有他反复表态不融资、不扩张。这是"不卖"叙事里最大的实证空洞
- **Ruby Central 交接进展**：10 周年帖（2022）说 2030 年后考虑移交 Ruby Central，但 2025 年撤款 + RubyGems 接管风波后双方关系破裂，接班/托管计划是否另有安排，无公开信息——这是追踪重点
- **Sidekiq Pro 首发定价与完整涨价轨迹**：2012 发布帖未写价格（可从首年 140 份/$70k 推得约 $500/份）；$500 → $950 → $1,000+ 各次调价的时间与公告不完整；2025-2026 年现行价目未核实
- **生日帖系列在 2022 年后疑似中断**：未检索到 11-14 周年帖，10 周年后的"编年史"要靠 HN 发言和版本发布帖拼接
- **Faktory 的营收占比**：第二产品线是否赚钱、占总盘子多少，无公开数字
- **个人背景**：出生年份、学历、The Clymb 之前的完整履历（据传 FiveRuns/Carbon Five 等，均未获一手来源核实）
- **IndieRails**：未找到他上过该节目的证据（尽管他是 indie Rails 商业化的头号标杆）
- **rubyevents.org 演讲档案页**（https://www.rubyevents.org/profiles/mperham ）反爬无法抓取，早年（2012 前）是否还有其他大会演讲未穷尽
