# Kagi（Vladimir Prelovac）

> 在 Google 免费帝国的正中心卖付费搜索——用户付钱、搜索无广告无追踪 ｜ kagi.com ｜ 创始人：Vladimir Prelovac ｜ 2018 年成立，2022 年 6 月公测收费 ｜ 团队约 50 人（2026）｜ 付费订阅搜索引擎 + WebKit 浏览器 ｜ 2023 年破 $1M ARR，2024 年中起盈亏平衡，2026 年估算 $9M+ ARR（第三方估计）

## 缝隙切入点

全世界最"不可能"的缝隙：搜索。Google 把它做成了免费+广告的万亿帝国，所有人默认"没人会为搜索付钱"。Kagi 的判断是：正因为免费，搜索才坏掉了——广告模式让搜索引擎为广告主打工，而不是为搜索者打工。

起点是一个具体的恼怒瞬间。2018 年 Prelovac 在 Google 搜 GitLab："I was using Google, as everybody else does in the world, and I was searching for GitLab. I saw a sponsored ad for GitLab at the top and then noticed the organic search result was also for GitLab."——广告位和第一条自然结果一模一样，他意识到自己的智商被广告商业模式侮辱了 [10][11]。

Kagi 的核心论证写在官方文档里：Google 2023 年仅美国广告收入就有 $760 亿，摊到每个用户约 $277/年（$23/月）——这是广告主为"影响你的搜索结果"付的钱。所谓免费，其实你在用注意力和数据付费，而且付得比 Kagi 的订阅费还贵 [12]。Prelovac 的说法更直接："The fact that we as citizens are getting information from the world's largest advertising company is my definition of dystopia." [10]

有意思的是，这个批评最早来自 Google 创始人自己：Brin 和 Page 1998 年的斯坦福论文就警告"advertising-funded search engines will be inherently biased towards advertisers and away from consumer needs" [12]。Kagi 等于是把 Google 创始人的原始警告做成了生意。

## 时机

- **创始人有底气**：Prelovac 是连续创业者，2010 年在贝尔格莱德创办 WordPress 管理工具 ManageWP（自筹资金，2015 年营收 $1M，30 人），2016 年卖给 GoDaddy，之后任 GoDaddy VP of Product 到 2018 年 [17]。退出所得让他能自掏约 $300 万，把 Kagi 白手养了四年（2018–2022）[1][11]。
- **VC 全部拒绝反而验证了缝隙**：他找硅谷 VC 融资，对方说他疯了，"没人会为搜索付钱，Google 是免费的" [11]。VC 不投的地方，恰好是巨头不会跟进的地方——Google 无法在不炸掉自己广告收入的前提下转向用户付费。
- **搜索质量肉眼可见地变差**：2020 年代初"Google 搜索变烂了"成为技术圈共识（SEO 垃圾、AI 生成内容、广告越来越多），付费换干净结果第一次有了真实需求。
- **订阅习惯已被养成**：Netflix/Spotify 教育了一代人为"无广告版"付费，搜索只是最后一个没人敢做的品类。

## 差异化

- **商业模式即产品**："You pay us, we work for YOU."（付费 = 激励对齐，无广告、无追踪、不留搜索记录）[12]。Prelovac："You can pay for Kagi with your wallet, not with your data."；"For Kagi, user data is a liability. We don't want it." [10]
- **反停留时间**：与所有广告产品追求 engagement 相反——"I want you to spend the least amount of time possible using Kagi."（越快搜到越快走，才是付费用户要的）[10]
- **用户可编程的结果**：用户可以对任何域名升权/降权/屏蔽（比如永久屏蔽 Pinterest），这在广告模式下不可能——广告模式不能允许用户屏蔽金主。
- **技术上是"混合搜索"**：聚合 Google、Brave、Mojeek、Yandex 等上游结果，加上自建索引 Teclis（非商业化小网站）、Tinygem（新闻）、Small Web（个人博客）——爬虫主动降权广告过多的网站，给个人网站曝光 [13][14]。
- **极简工程文化**：后端用 Crystal 语言 + PostgreSQL 裸 SQL，前端 Jinja 模板 + 尽量少的 JavaScript，服务端渲染，零客户端埋点 [13]。

## 第一批用户/冷启动

教科书级的 HN 冷启动：

- 2019 年先做了个失败的付费搜索尝试 Donna.gg，没人买账 [1]。
- 2021–2022 年封闭 beta 积累种子用户，2022 年 6 月 1 日在 Hacker News 公开发布（"Kagi search and Orion browser enter public beta"），热帖顶评："I've been evaluating Kagi for a couple weeks, I'm liking it, but today I'm completely sold." [19]
- **发布首日 210 个付费客户**——三年后其中 121 人仍在付费 [2]。
- 头三个月：约 2,600 名付费客户，每天约 7 万次查询，每天 30–50 个新注册全部来自口碑，免费转付费率 20%，月流失率低于 3% [6]。
- 目标人群极其清晰：为搜索结果质量痛苦的专业开发者/技术人。官方口径："our core focus remains on professionals." [8]

冷启动阶段的账很难看：单次搜索成本 1.25 美分，月基础设施开销约 $26,250，MRR 约 $26,500——收入刚够付服务器，工资和运营（约 $10 万/月）全靠创始人的钱 [6]。

## 收入与定价

**定价史是一部教材，包括一次公开的来回摇摆：**

- 2022-06 上线：$10/月不限量 [19]。
- 2023-03 涨价+限量：$5/月 300 次、$10/月 700–1,000 次、$25/月不限量。理由摊开讲："We are already losing money on most accounts."（Kagi 用户月均搜 700 次，而 Google 用户平均只搜 90–120 次、DuckDuckGo 用户约 30 次——重度用户自选择进来，成本模型被击穿）[8]。此举违背了半年前"老用户永久保价"的承诺，社区反弹。
- 2023-09 恢复：$10/月重新不限量（上游成本降了 + 规模效应），加年付 9 折 [9]。
- 2025-02 "Fair Pricing"：**哪个月完全没用，就自动免掉下个月的钱**。官方解释只有一句："We have implemented this for the simple reason of being kind to our users." [15]

**资金结构（"不接 VC"经核实，但不是纯自资）：**

- 2018–2022 完全由创始人自掏腰包（约 $300 万）[1][11]。
- 2023-06 第一次外部融资：SAFE 轮 $670K，42 名合格投资人，**大部分是 Kagi 用户**（"Friends, Family, and Users" 轮，最低 $5,000 起投）[7]。
- 2023–2024 两轮合计约 $2.4M，93 名天使全部来自社区；VC 融资额：$0 [3][13]。官方说法：用户股东"provides invaluable insights and feedback"，股权结构本身就是激励对齐 [3]。
- 2024 年注册为特拉华州 Public Benefit Corporation（公共利益公司），章程写明"aligns the incentives of everyone involved" [1][3]。

**里程碑：**2023 年破 $1M 年收入 [1] → 2024-05/06 宣布盈亏平衡（break-even profitable）[2][3] → 2024-01 两万付费会员 → 2025-06 五万会员（含 5,000+ 家庭、近 200 团队）[4] → 2026-07-16 实时数据：**73,132 名付费会员**、9,531 个家庭、399 个团队、日查询 107 万次 [5]。第三方估算 2025 年营收约 $9.1M [ZoomInfo，估计值]。收入 100% 来自订阅，无任何其他收入源 [3]。

## 内容与增长

- **透明报告即内容营销**：2022 年起定期发"status update"（First three months、What's next for Kagi 2024、First three years 2025、2025 Year in Review），公开成本、亏损、会员数、churn，每篇都上 HN 热榜。2023 年起干脆把会员数和查询量做成实时公开页 kagi.com/stats [5]。对一家反追踪公司来说，"自己被看光"是最好的信任广告。
- **增长几乎全靠口碑**：不投广告（投广告等于自我否定）。2024-01 到 2025-06 会员翻 2.5 倍 [4]。
- **Orion 浏览器是获客渠道**：官方承认 Orion 贡献了约 20% 的客户获取 [8]。
- **2025-06 转向漏斗模式**：上线免费搜索门户（不注册 50 次搜索、注册再送 100 次）+ Kagi for Libraries（全球公共图书馆读者免费一年）[4]——从"纯付费墙"转向"有限免费引流"。
- 媒体背书自然累积：Fast Company、The Verge、Ars Technica 等主流科技媒体报道 [18]。

## 社区

- 两个公开反馈站：kagifeedback.org（早期 1/4 付费用户注册过）、orionfeedback.org；官方论坛累计 3,500+ 搜索讨论帖、6,400+ 浏览器讨论帖 [3][6]；Discord 7,400+ 成员 [4]。
- **用户就是股东**：93 名投资人全部来自社区 [3]。
- 仪式感运营：五万会员时发 2 万双 Kagi 袜子；从 121 名"首日会员"里抽 3 人全费请到欧洲聚会一周；CEO 兑现上线时的承诺把头发染成蓝绿色 [4]。
- 2025 年在贝尔格莱德开了实体 Kagi Hub，加入日本涩谷创业计划 [18]。
- 发起 SlopStop 社区行动，靠用户众包标记 AI 垃圾内容 [18]。

## 留存

- 头三个月：月流失 <3%；试用转付费 20%，其中 77% 在第一周内转化、超过 1/3 当天转化——付费意愿在试用前就已形成，产品只需不辜负 [6]。
- **首日 210 名客户，三年后 121 名仍在付费（57.6% 三年留存）**——订阅产品里极罕见的数字 [2]。
- Fair Pricing 是留存哲学的极致：与其赚沉睡用户的钱，不如免单换信任 [15]。
- 结构性留存：升降权/屏蔽规则、Lens 等个性化设置是用户自己积累的资产，迁移成本随使用加深。

## 转型

- 失败起点：2019 年 Donna.gg（初版付费搜索）无人问津，推倒重来 [1]。
- 定价三连跳（不限量→限量→不限量）是一次公开试错，代价是违背承诺的信任损耗，收获是找到了可持续的 $10 不限量模型 [8][9]。
- 2025 年从"纯付费"转向"免费门户+图书馆计划"的漏斗获客 [4]。
- 从单品到生态：搜索 → Orion 浏览器（2025-11 出 1.0，百万下载，iOS/macOS/Linux，$5/月或 $150 终身的 Orion+ 已有 3,202 人付费）→ Assistant（2024）→ Translate（2024）→ Kagi News（2025）→ Kagi Mail（开发中）[1][2][5][16]。Prelovac 的判断：全球只有 4 家公司同时拥有"搜索+浏览器+邮箱"完整生态，Kagi 想做第五家 [2]。

## 如何保持小

- 团队规模：2018 年 3 人 → 2022 年 15 人 → 2024 年 40 人（其中 30 名工程师）→ 2026 年约 50 人；全远程，分布美加 45%/欧洲 40%/亚洲 15% [1][13]。
- **明确的"小"目标**：Prelovac 公开表示要做到 **$10 亿年收入但员工少于 Dunbar 数（150 人）**，5–9 年内做到 500 万客户，靠"selective hiring"维持组织凝聚力 [2]。
- 不接 VC = 不接增长指标枷锁；PBC 章程把"用户利益优先"写进公司结构，堵死"先圈用户再变现"的路 [3]。
- 技术选型服务于小团队：Crystal + 裸 SQL + 服务端渲染 + 几乎零 JS，30 个工程师维护整个生态 [13]。
- 收入结构简单到极致：只有订阅费，没有广告、没有数据生意、没有企业定制包袱 [3]。

## 开放问题（值得当面问创始人的）

1. 2023 年定价来回摇摆、违背"老用户保价"承诺那半年，实际流失了多少会员？如果重来，会先涨价还是先公开单位成本？
2. Kagi 的结果依赖 Google/Yandex 等上游 API。如果 Google 切断 API 供应怎么办？自建索引扩到 1 亿高质量页面 [3] 的进度和成本曲线如何？（Yandex 来源在 2022 年后的争议是否影响过续费？）
3. "$1B 收入 + <150 人"意味着人均年产出近 $700 万。哪些职能是你永远不打算招的？客服和内容审核在 500 万用户时怎么办？
4. 93 名用户股东拿的是 SAFE——他们的退出预期是什么？PBC 结构下有没有"永不出售"或 credible exit 的正式承诺？
5. Fair Pricing 上线一年多，实际触发免单的比例是多少？它对 churn 的可测量影响有多大——这是善意还是精算过的留存工具？

## 来源

- [1] Kagi Docs – Company History: https://help.kagi.com/kagi/company/history.html
- [2] Kagi Blog – Kagi status update: First three years（2025-06）: https://blog.kagi.com/first-three-years
- [3] Kagi Blog – What's next for Kagi?（2024-05，首份年度透明信）: https://blog.kagi.com/what-is-next-for-kagi
- [4] Kagi Blog – Celebrating 50K users（2025-06）: https://blog.kagi.com/50k
- [5] Kagi 实时统计页（2026-07-16 抓取）: https://kagi.com/stats
- [6] Kagi Blog – Status update: First three months（2022-09-01）: https://blog.kagi.com/status-update-first-three-months
- [7] Kagi Blog – Kagi raises $670K（2023-06-28）: https://blog.kagi.com/safe-round
- [8] Kagi Blog – Update to Kagi Search pricing（2023-03）: https://blog.kagi.com/update-kagi-search-pricing
- [9] Kagi Blog – Unlimited Kagi searches for $10 per month（2023-09-21）: https://blog.kagi.com/unlimited-searches-for-10
- [10] 1Password 访谈 Vladimir Prelovac – The real cost of "free" search: https://1password.com/blog/real-cost-search-engines-interview
- [11] TWiT – Breaking Free from Google: How Kagi's Paid Search Model is Revolutionizing the Web: https://twit.tv/posts/tech/breaking-free-google-how-kagis-paid-search-model-revolutionizing-web-experience
- [12] Kagi Docs – Why pay for search?: https://help.kagi.com/kagi/why-kagi/why-pay-for-search.html
- [13] The Pragmatic Engineer – Taking on Google search: Perplexity and Kagi: https://newsletter.pragmaticengineer.com/p/perplexity-and-kagi
- [14] Wikipedia – Kagi (search engine): https://en.wikipedia.org/wiki/Kagi_(search_engine)
- [15] Kagi Fair Pricing（2025-02，The Verge 等报道 + @KagiHQ）: https://x.com/KagiHQ/status/1886935292223086902
- [16] Orion Browser（1.0 发布 2025-11；Linux beta 2026-03）: https://blog.kagi.com/orion / https://www.omgubuntu.co.uk/2026/01/orion-browser-for-linux-alpha
- [17] ManageWP 被 GoDaddy 收购（2016）: https://wptavern.com/godaddy-acquires-wordpress-site-management-service-managewp / https://tech.eu/brief/managewp-godaddy/
- [18] Kagi – 2025 Year in Review: https://kagi.com/2025
- [19] Hacker News 发布帖（2022-06-01）: https://news.ycombinator.com/item?id=31584791
- [ZoomInfo 营收估计，仅供参考]: https://www.zoominfo.com/c/kagi-inc/21087075
