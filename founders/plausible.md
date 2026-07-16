# Uku Täht ＆ Marko Saric — Plausible

> Plausible Analytics：开源、隐私友好的 Google Analytics 替代品。爱沙尼亚公司，全程 bootstrap，零广告投放，零投资人。Uku 负责产品与工程（爱沙尼亚，Elixir + ClickHouse），Marko 负责内容营销与传播（丹麦背景，前内容营销人）。截至 2026 年：19,000+ 付费订阅者，团队 10 人。
>
> 建库日期：2026-07-16。所有语录为英文逐字原文（经网页抓取提取，正式引用前建议对原文页面复核一遍）。

## 账号全集

### Marko Saric（营销/内容，联合创始人）

- 个人网站 + 博客：https://markosaric.com/ （邮箱 hi@markosaric.com，官网自述页确认）
- X / Twitter：https://x.com/markosaric
- Mastodon：https://fosstodon.org/@markosaric （官网标注的现用账号；https://mastodon.social/@markosaric 亦存在，疑为旧号，未确认）
- LinkedIn：https://www.linkedin.com/in/markosaric/
- Medium（旧）：https://medium.com/@MarkoSaric
- Crunchbase：https://www.crunchbase.com/person/marko-saric-7f8d
- 背景（据 markosaric.com 自述）：生于"一个已不存在的国家"（前南斯拉夫），少年时移居丹麦；英国 Staffordshire 大学市场营销学士；伦敦某上市游戏公司做内容营销/社媒 7 年；某风投 B2B SaaS 分析公司增长负责人 3 年；2020-03 加入 Plausible。

### Uku Täht（产品/工程，创始人）

- X / Twitter：https://x.com/ukutaht
- GitHub：https://github.com/ukutaht （2016 年写过 elixir-koans 教学项目）
- dev.to：https://dev.to/ukutaht
- LinkedIn：https://www.linkedin.com/in/uku-taht/
- YouTube：https://www.youtube.com/c/UkuT%C3%A4ht
- Changelog 个人页（播客出场索引）：https://changelog.com/person/ukutaht
- Crunchbase：https://www.crunchbase.com/person/uku-t%C3%A4ht （曾任 Gigride CTO，Miina Härma 中学，坐标爱沙尼亚塔尔图/塔林）
- 背景（据 Flagsmith 访谈）：曾在伦敦与朋友做过一个失败的创业项目；因同事要求装 Google Analytics 而对"数据中间商"感到不适，萌生做替代品的念头。

### 公司官方

- 博客（增长复盘主阵地）：https://plausible.io/blog
- X / Twitter：https://twitter.com/plausiblehq
- GitHub：https://github.com/plausible
- About / 数据页：https://plausible.io/about

## 访谈清单

1. **2020-05-27 · The Changelog Interviews #396「De-Google-ing your website analytics」（Uku + Marko）**
   https://changelog.com/podcast/396 （官方复盘：https://plausible.io/blog/changelog-podcast）
   - Uku 先写博客立 flag 再写代码，用公开承诺换早期关注与自我问责
   - GA 脚本臃肿（45.7KB）、收集 300+ 指标但大多数人根本不看——做减法就是产品定位
   - 无 cookie、匿名化处理，从根上绕开 GDPR 弹窗问题
   - 选 MIT 开源是为了防"公司变质"：用户不信任你时可以带着代码走
   - Marko 的 4 月爆文带来流量 +2,500%、272 个试用注册（3 月的 6 倍）、MRR 数周内 +80%

2. **2021-04-11 · It's FOSS 文字访谈（Marko）**
   https://itsfoss.com/news/marko-saric-plausible/
   - Plausible 是"对 Google 变成什么样、对今日互联网现状的直接回应"
   - 经常有 VC 主动找上门，一律礼貌拒绝
   - MIT → AGPL 是防大公司白嫖："这些想占开源便宜的公司并不真的热爱开源"
   - 捐赠模式养不活开源项目，付费订阅才可持续；他们把营收 5% 捐回开源生态
   - 截至当时：2,700 订阅者、$18,500 MRR

3. **2021-04-29 · Indie Hackers AMA「From $400 to $22k MRR in one year」（Uku + Marko）**
   https://www.indiehackers.com/post/from-400-to-22k-mrr-in-one-year-with-plausible-a-google-analytics-alternative-ama-776a4803b7
   - 一年从 $400 到 $22,010 MRR，3,085 订阅者，追踪 16,657 个网站
   - Marko："2020 年 4 月初发的第一篇博文冲上 Hacker News 头条……戏剧性地提升了知名度"
   - Marko 80% 时间在回复用户来信，每天清空收件箱——支持即营销
   - Uku：没有 ClickHouse 撑不起这个规模（峰值 278 请求/秒）

4. **2021-10-18 · Sustain 播客 #95（Marko）**
   https://podcast.sustainoss.org/95
   - 做隐私产品不开源就没有可信度："If you're not open source and you're talking about privacy first you will probably be excluded from the conversation."
   - AGPL 是在"开发者友好"与"商业存活"之间的取舍
   - 不追 VC 增长，"just do our own thing and try to do our own little sustainable business"

5. **约 2021 · The Craft of Open Source #2（Flagsmith 出品，Uku + Marko）**
   https://www.flagsmith.com/podcast/plausible （文字版：https://flagsmith.medium.com/interview-with-uku-taht-and-marko-saric-founders-plausible-1c9643e510f2）
   - Uku 讲创业动机三条：做分析赛道的替代品、学习海量数据处理、受 Indie Hackers 运动启发做商业产品
   - Uku：开源带来的是安全报告而不是抄袭——"社区不在，增长不在"
   - Marko：GitHub 星标增长没有任何 growth hack，全靠产品与立场

6. **2022-06-28 · Thinking Elixir 播客 #105（Uku 单独）**
   https://podcast.thinkingelixir.com/105
   - 刚过 $1M ARR 的技术复盘：Elixir + ClickHouse，自写 ClickHouse Ecto 适配器
   - 谈规模化的 growing pains、创始工程师"永远是那个要修东西的人"的心理重量
   - 谈 burnout 与健康：离问题太近，会看不见自己已经取得的成绩
   - 公司文化"transparent by default"

7. **2023-08-09 · Indie Hackers 文字访谈「From $400/mo to $188,000/mo in 3 years」（Marko）**
   https://www.indiehackers.com/post/from-400-mo-to-188-000-mo-in-3-years-marko-saric-of-plausible-tells-us-how-he-did-it-7a4e821834
   - $188k MRR、11,000+ 付费用户、客单价不到 $20/月、团队仍以两位创始人为核心
   - 第一年连续数月每周发两篇纯教育性（非推销）博文
   - "从未做过任何付费广告，没有联盟计划，不付钱让任何人推荐我们"
   - 付费用户主要来自口碑，自然流量的用户留存更好

8. **2025-02-27 · OpenSaaS.sh 文字访谈「Meet Marko Saric」（Marko）**
   https://docs.opensaas.sh/blog/2025-02-27-meet-marko-saric-co-founder-of-privacy-friendly-plausible-analytics/
   - 当时数据：14,000+ 活跃订阅者，累计追踪 136B+ 页面浏览
   - "我们的营销策略很无聊，对所有 growth hack 和'最佳实践'说不"
   - 给创始人的建议：无论以后融不融资，先 bootstrap；推荐《Rework》和《This Is Marketing》

9. **2025-05-06 · Indie Hackers 专题「They Made $1 Million+ Going Against Google」（Uku + Marko）**
   https://www.indiehackers.com/post/they-made-1-million-going-against-google-1fe07df370 （转载：https://www.jointhequarter.com/blog/plausible）
   - 完整叙事线：2018-12 写第一行代码 → 2019-05 首月收入 $64 → 2019-07 上 HN 但只到 $118 MRR → 2020 年 Marko 加入后起飞
   - 定位学案例："They're the Google Analytics alternative"——就叫板行业老大，反而好记

10. **2025-08-06 · Subscription Heroes #24「How Plausible Grew to $1M ARR Without Ads or Investors」（Marko）**
    https://churnkey.co/subscription-heroes/how-plausible-grew-to-1m-arr-without-ads-or-investors-marko-saric-co-founder-of-plausible/
    - 复述冷邮件起源：Uku 读到 Marko 的 de-Google 博文后主动发邮件，两人此前素不相识
    - 没有投资人 = 没有外部增长压力，目标是可持续的赚钱生意而非 hypergrowth
    - 团队多数人四天工作制；刻意不加速，因为加速会带来不可持续的压力

其他文字访谈（备查）：20i 访谈 https://www.20i.com/blog/plausible-analytics-interview-with-co-founder-marko-saric/ ；Paddle 谈挑战市场老大的定位 https://www.paddle.com/blog/how-position-your-saas-business-against-a-market-leader ；SEO Buddy「My SEO Journey」 https://seobuddy.com/blog/my-seo-journey-marko-saric/ ；Step by Step Business https://stepbystepbusiness.com/plausible-analytics-marko-saric-interview/ ；Build In Public Hub https://buildinpublichub.substack.com/p/how-i-built-this-in-public-marko ；SaaS Growth Podcast EP6 https://carlanderson.xyz/saas-growth/episode-6/

## 演讲与公开课

**重要发现：两人几乎不做大会演讲。** 检索 MicroConf / FOSDEM / ElixirConf 等主流会议均无二人讲台记录。他们的公开表达集中在两个渠道：公司博客（Marko 的长文）+ 播客访谈。仅有的类演讲记录：

- Hasgeek PrivacyMode（印度隐私社区）线上对谈「Chat with Uku Taht — Plausible as a Privacy Preserving Alternative to Google Analytics」：https://hasgeek.com/PrivacyMode/plausible-io-a-privacy-preserving-alternative/schedule/chat-with-uku-taht-plausible-as-a-privacy-preserving-alternative-to-google-analytics-12k1QYBxe7nr3PkX6Pmb84
- YouTube 片段「Plausible creator Uku Täht on side project success」（Changelog 剪辑，2020-07）：https://www.youtube.com/watch?v=llZXFta_KnM

## 博客关键文章

Marko 的增长复盘全部公开发在 plausible.io/blog，是从 0 到 $1M ARR 最完整的逐段公开记录之一。

### 增长复盘系列（金矿）

1. **Why you should stop using Google Analytics on your website**（2020-04-08）https://plausible.io/blog/remove-google-analytics — Marko 入伙后第一篇文章，HN 当日第一，一周 48,000 访客（超过之前 15 个月总和），一篇文章改写公司命运的反 Google 檄文。
2. **How one blog post changed the traction for my startup**（2020-04-17）https://plausible.io/blog/blog-post-changed-my-startup — 对上一篇爆文的复盘："内容营销不像付费广告那样立竿见影""发布之后推广工作才刚开始"。
3. **Building Plausible: April 2020 recap**（2020-05）https://plausible.io/blog/april-2020-recap — 爆发月流水账：62.8k 访客（+2,500%），4 月 272 个注册超过之前 9 个月总和。
4. **$400 to $2,750 MRR in 135 days without ads**（2020-07-31）https://plausible.io/blog/startup-marketing — Marko 加入后头 135 天的打法明细。
5. **What we learned on our journey to $10,000 MRR**（2021-01-28）https://plausible.io/blog/growing-saas-mrr — 9 个月从 $400 到 $10k MRR 的完整教训清单。
6. **How we bootstrapped our Google Analytics alternative to $500k ARR**（2021-10-25）https://plausible.io/blog/bootstrapping-saas — 自曝低谷（数月无薪水、倒贴 $50k+）与"零广告预算、无联盟计划、无视一切最佳实践"的方法论。
7. **How we built a $1M ARR open source SaaS**（2022-06-22）https://plausible.io/blog/open-source-saas — 里程碑总结帖（2022-06-02 达成 $83,637 MRR / 7,000+ 订阅者），开源 SaaS 商业模式的教科书级复盘，全网转载最多。

### 立场文与开源治理

8. **Plausible is going open source**（2019-09-02，Uku）https://plausible.io/blog/plausible-is-going-open-source — 开源决定的原始公告。
9. **How to pay your rent with your open source project**（2020-06-18）https://plausible.io/blog/open-source-funding — "捐赠养不活开源，订阅可以"的核心论证。
10. **Open source licensing and why we're changing Plausible to the AGPL license**（2020-10-12）https://plausible.io/blog/open-source-licenses — MIT → AGPL 的防白嫖逻辑，开源商业化必读。
11. **Is Google Analytics GDPR compliant?**（2020-06-09）https://plausible.io/blog/google-analytics-gdpr 与 **Is Google Analytics illegal?**（2023-07 更新）https://plausible.io/blog/google-analytics-illegal — 借欧洲监管裁决持续输出的反 GA 法律弹药库。
12. **Introducing Plausible Community Edition**（2024-02-23）https://plausible.io/blog/community-edition — 自托管版更名 CE、部分企业功能云端独占："如果我们无法捕获自己工作的经济价值，项目就会不可持续而死掉。"
13. **Why we say no to investors and are 100% user-supported**（2026-01-15，官方博客）https://plausible.io/blog/customers-not-investors — 拒绝投资人立场的最新集大成："真正的成功是可持续的财务自由，而不是一次风光的退出。"

### markosaric.com 个人站关键文章

14. **How to de-Google-ify your life for a less intrusive web**（2020-03-18）https://markosaric.com/surveillance-capitalism/ — 促成两人合伙的 de-Google 系列（Uku 正是读到 Marko 的 de-Google 文章后发出冷邮件）。
15. **How to de-Google your site to make it faster and visitor friendly**（2020-04-24）https://markosaric.com/degoogleify/
16. **Ethical marketing in the GDPR, CCPA and no third-party cookies world**（2020-04-23）https://markosaric.com/ethical-marketing/ — 他的"道德营销"方法论原型。
17. **Only 9% of visitors give GDPR consent to be tracked**（2020-07-06）https://markosaric.com/gdpr-consent/ 与 **13% of my website visitors block Google Analytics**（2020-07-13）https://markosaric.com/google-analytics-blocking/ — 用自家数据做原创研究引流的典型打法。
18. **10 startup marketing lessons from 1,000 days at a SaaS**（2018-11-22）https://markosaric.com/startup-marketing/ — 加入 Plausible 之前的方法论存货，可看出其打法一以贯之。

## 创业时间线

- **2018-12** — Uku（时任/前 Gigride CTO，此前在伦敦有过失败创业）写下 Plausible 第一行代码。（来源：https://plausible.io/blog/open-source-saas ；https://plausible.io/about）
- **2019 年初** — MVP 完成，经由 Indie Hackers 公开测试上线。（来源：https://plausible.io/blog/open-source-saas ；https://www.indiehackers.com/post/they-made-1-million-going-against-google-1fe07df370）
- **2019-05** — 上线付费订阅；2019-05-14 迎来第一个付费用户，首月收入 $64。（来源：https://plausible.io/blog/bootstrapping-saas）
- **2019-07** — Uku 的博文上了 Hacker News，日访客 2,500，但 MRR 仅到 $118——流量≠收入的第一课。（来源：https://www.indiehackers.com/post/they-made-1-million-going-against-google-1fe07df370）
- **2019-09-02** — 宣布开源（MIT）。（来源：https://plausible.io/blog/plausible-is-going-open-source）
- **2020 年初（低谷）** — 上线 324 天才做到 $400 MRR，随后数月停滞；Uku 独自撑了一年多，意识到需要营销合伙人。（来源：https://plausible.io/blog/bootstrapping-saas ；https://churnkey.co/subscription-heroes/how-plausible-grew-to-1m-arr-without-ads-or-investors-marko-saric-co-founder-of-plausible/）
- **2020-03** — Uku 读到 Marko 的 de-Google 博文后发冷邮件（两人素不相识）；3 月中旬 Marko 以联合创始人身份加入，当月 MRR $433。（来源：https://plausible.io/blog/open-source-saas ；https://www.indiehackers.com/post/from-400-to-22k-mrr-in-one-year-with-plausible-a-google-analytics-alternative-ama-776a4803b7）
- **2020-04-08（HN 爆发）** — Marko 第一篇博文《Why you should stop using Google Analytics on your website》登顶 Hacker News：一周 48,000 独立访客（超过此前 15 个月总和），4 月新增 272 个注册（超过此前 9 个月总和），GitHub 星标翻倍。（来源：https://plausible.io/blog/blog-post-changed-my-startup ；https://plausible.io/blog/april-2020-recap）
- **2020-10-12** — 开源许可证 MIT → AGPL，防大公司拿代码做闭源商业产品。（来源：https://plausible.io/blog/open-source-licenses）
- **2021-01** — 突破 $10,000 MRR（从 $400 到 $10k 用了 9 个月）。（来源：https://plausible.io/blog/growing-saas-mrr）
- **2021-10** — $500k ARR（$42,624 MRR，约 4,800 订阅者）；自曝曾数月不领薪水、靠积蓄倒贴 $50,000+。（来源：https://plausible.io/blog/bootstrapping-saas）
- **2022-01** — 奥地利等欧洲数据保护机构裁定使用 Google Analytics 违反 GDPR，外部监管事件放大自然增长势头。（来源：https://plausible.io/blog/google-analytics-illegal ；https://plausible.io/blog/open-source-saas）
- **2022-06-02（$1M ARR）** — $83,637 MRR、7,000+ 付费订阅者、50,000+ 网站在用；团队仅 4 人，全程零广告、零投资人。（来源：https://plausible.io/blog/open-source-saas）
- **2023-08** — $188,000 MRR（≈$2.25M ARR），11,000+ 付费用户，客单价 <$20/月。（来源：https://www.indiehackers.com/post/from-400-mo-to-188-000-mo-in-3-years-marko-saric-of-plausible-tells-us-how-he-did-it-7a4e821834）
- **2024-02-23** — 推出 Plausible Community Edition：自托管版更名、保持 AGPL 免费，但漏斗、电商收入等企业功能云端独占。（来源：https://plausible.io/blog/community-edition）
- **2024 年** — 五周年，团队约 8 人，累计追踪 73B+ 页面浏览；第三方估算年末约 $3.1M ARR（非官方口径）。（来源：https://founderventures.io/companies/plausible ；https://tinyempires.substack.com/p/inside-a-tiny-empire-plausible-analytics）
- **2025-02** — 14,000+ 活跃订阅者，累计 136B+ 页面浏览。（来源：https://docs.opensaas.sh/blog/2025-02-27-meet-marko-saric-co-founder-of-privacy-friendly-plausible-analytics/）
- **2026 年（现状）** — 19,000+ 付费订阅者，团队 10 人，多数人四天工作制，继续"用户即股东"、明确永不融资不卖身；2026-04 创下史上最佳单月。（来源：https://plausible.io/about ；https://plausible.io/blog/customers-not-investors ；https://plausible.io/blog/homepage-edits-conversion-lift）

## 语录

1. **Uku Täht**："I don't wanna use Google Analytics, but I didn't have a good alternative."
   —— The Changelog #396（2020-05-27），谈创业起点。https://changelog.com/podcast/396

2. **Uku Täht**："I wanted to learn that space because the handling of these massive amounts of data is interesting."
   —— Flagsmith《The Craft of Open Source》访谈，谈做分析产品的第二动机。https://flagsmith.medium.com/interview-with-uku-taht-and-marko-saric-founders-plausible-1c9643e510f2

3. **Marko Saric**："We have a $0 paid advertising budget and we don't have an affiliate program either. We pretty much ignore all the best marketing practices."
   ——《How we bootstrapped our Google Analytics alternative to $500k ARR》（2021-10-25）。https://plausible.io/blog/bootstrapping-saas

4. **Marko Saric**："Last year, we went several months without any salaries living from personal savings while growing Plausible. It was challenging and we were down more than $50,000."
   —— 同上（2021-10-25），自曝低谷。https://plausible.io/blog/bootstrapping-saas

5. **Marko Saric**："Free and open source software can be sustainable and can pay your rent."
   ——《How we built a $1M ARR open source SaaS》（2022-06-22）。https://plausible.io/blog/open-source-saas

6. **Marko Saric**："Plausible is pretty much a direct response to what Google has become and to the state of the web today."
   —— It's FOSS 访谈（2021-04-11）。https://itsfoss.com/news/marko-saric-plausible/

7. **Marko Saric**："We want to grow without supporting surveillance capitalism. Some may say we're leaving money on the table, and we're okay with that."
   —— Indie Hackers 访谈（2023-08-09）。https://www.indiehackers.com/post/from-400-mo-to-188-000-mo-in-3-years-marko-saric-of-plausible-tells-us-how-he-did-it-7a4e821834

8. **Marko Saric**："If we cannot capture the economic value of our work, the project will become unsustainable and die."
   ——《Introducing Plausible Community Edition》（2024-02-23），谈开源商业化的底线。https://plausible.io/blog/community-edition

9. **Plausible 官方博客**："We're sustainably profitable and solely funded by our subscribers. We have never raised a single dollar from any investor."
   ——《Why we say no to investors and are 100% user-supported》（2026-01-15）。https://plausible.io/blog/customers-not-investors

## 资料缺口

- **Uku 的深度个人访谈极少**：仅 Thinking Elixir #105 一次单独长访谈；其伦敦失败创业的公司名、Gigride 任职细节均无一手确认。
- **Marko 加入前的雇主未具名**：官网自述"伦敦某上市游戏公司 7 年 + 某风投 B2B SaaS 分析公司增长负责人 3 年"，具体公司名未查到；其出生国（前南斯拉夫的具体共和国）未确认。
- **冷邮件对应的具体文章有出入**：多数来源说 Uku 读的是 Marko 的 de-Google 文章，但现存《How to de-Google-ify your life》标注 2020-03-18，与"2 月/3 月中旬邮件往来"的时间线略有矛盾（可能是文章后来改版换址）。
- **2024 年 $3.1M ARR 为第三方估算**（tinyempires、onepc 等二手来源），官方最后一次正式公布收入里程碑是 2022 年 $1M ARR；五周年官方博文的准确 URL 未定位。
- **无大会演讲**：两人刻意低调，公开表达 95% 集中在自家博客与播客，视频素材稀缺。
- **Marko 早年博客**（据称运营十余年的 howtomakemyblog.com）未直接验证，仅有同名 SlideShare 账号旁证。
- **语录复核**：以上语录经抓取工具从原文提取，正式引用前建议对原文页面逐字校对（尤其播客口语引文）。
