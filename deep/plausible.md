# Plausible Analytics

> 在 Google Analytics 免费垄断的市场里，把"隐私 + 轻量 + 开源"做成用户付费订阅 ｜ plausible.io ｜ Uku Täht & Marko Saric ｜ 2018-12 写下第一行代码，2019-04 上线收费 [1][9] ｜ 10 人（2026-07 官网自述）[11] ｜ 开源 SaaS / 隐私分析 / 反巨头 / pure-bootstrap ｜ 公开口径：$1M ARR（2022-06）[1]，$188k MRR ≈ $2.26M ARR（2023 访谈）[13]；第三方估 2024 约 $3.1M ARR（仅供参考）[18]

## 缝隙切入点

- 对手是"免费且垄断"：GA 装在互联网大部分网站上，价格是零。Plausible 的赌注是——有一群人愿意为"不做监控资本主义的分析工具"付钱。Marko 的原话："We want to grow without supporting surveillance capitalism... We don't want to sacrifice our principles or happiness to become the next unicorn."[13]
- 产品层面的缝隙是"GA 太重"：Uku 2019 年 4 月的发布帖把卖点写成一页纸——"Get all the important stats on one single page. No training necessary."[9] 今天官网的量化版本：脚本比 GA 小 54 倍，无 cookie、无需 cookie 弹窗 [11]。
- 商业层面的缝隙是"信任"：不融资、不卖数据、代码开源可审计——"The code is public and auditable. Verify exactly what we collect, and run it yourself if you want to."[11] 开源在这里不是开发模式，是信任装置："Being open source adds a new level of transparency and trustworthiness that proprietary products don't have."[3]
- 一句话总结其模式：既然不收广告钱、不卖数据，那唯一的收入必须来自用户——"Subscription revenue is the only revenue we have."[12]

## 时机

- GDPR 2018 年 5 月生效，Uku 2018 年 12 月开始写代码，2019 年 4 月上线 [1][9]——正好卡在欧洲隐私监管收紧、大众反追踪意识抬头的起点。
- 增长的几次大浪都是"别人犯错/搞事"送来的：Google FLoC 争议、AMP 争议、欧洲数据保护机构裁定使用 GA 违反 GDPR——蹭准这些新闻节点的博文一次次带来流量高峰 [1]。
- 时机也解释了为什么同样的产品 2019 年只能挣 $64 MRR、2022 年却能过 $1M ARR：产品没有本质变化，是市场对"隐私"的付费意愿在这三年里被监管和大厂自己教育出来了 [1]。
- 2020 年 10 月，TechCrunch 报道称其为"增长最快的开源创业公司"[16]。

## 差异化

- 三个词能说完：隐私（无 cookie、不收集个人数据、GDPR/CCPA 合规 [12][16]）、轻量（脚本比 GA 小 54 倍 [11]）、开源（AGPLv3，可自托管 [16]）。
- 地缘也是差异化：“Made and hosted in the EU”——"Built and hosted in the EU. Your data never leaves European-owned infrastructure."[11] 在 GA 数据出境屡被欧洲监管判违规的背景下，这句话本身就是销售文案。
- 反向差异化同样重要——他们公开列出**不做**的事："We've never done any type of paid advertising, we don't have an affiliate program, we don't pay anyone to recommend us, we don't have a mailing list that we use to broadcast marketing messages, we don't do any sales calls."[13] 不做 A/B 测试、不装 Facebook/Google 像素、不弹窗 [2]。
- 客户名单是差异化的背书：Basecamp、Ghost、Hugging Face、MongoDB、Python 软件基金会、哈佛大学 [12]，以及苏格兰政府、Steve Jobs Archive [16]。

## 第一批用户/冷启动

- 冷启动极其难看：2019 年 5 月 14 日第一个付费用户，之后花了 **324 天**才做到 $400 MRR [3]。逐月数字：2019-05 $64 → 2019-07 $118 → 2019-09 $178 → 2020-02 $403 [1]。
- 第一批用户来自 Indie Hackers：Uku 从开发期就在 IH 发帖记录，"早期营销全靠 Indie Hackers，第一批访客和客户直接来自那里" [3]。
- 上线时的定价就拒绝免费档：$6/$12/$36 按页面浏览量分档，"There will be no premium features, accounts will be billed purely for the amount of traffic they get"；不设免费层的理由是单人创始者撑不起免费用户的支持成本 [9]。
- 转折点是找营销合伙人：卡在约 100 个订户、$400 MRR、创业 14 个月时，Uku 决定找一个 marketing co-founder；他通过 Marko 写"隐私友好的科技替代品"的博客找到了他，2020 年 3 月 Marko 以联合创始人身份加入 [1][15]。Marko 的说法："Uku decided to look for a marketing co-founder and that's how we found me."[15]
- Marko 加入后 135 天（2020-04-02 至 07-30）：$415 → $2,750 MRR，订户 100 → 427，试用注册翻 10 倍，网站流量 18 万访客（+2,200%），全程零广告费 [2]。

## 收入与定价

- 关键里程碑（全部自己公开）：2020-09 $5,035 MRR 首次给自己发工资；2021-01 $11,303 MRR 达到可持续；2021-10 $42,624 MRR（$500k ARR）；2022-06-02 $83,637 MRR，$1M ARR，7,000+ 付费订户 [1]。在此之前两位创始人无薪工作、各自消耗了 $50k 以上个人积蓄 [3]。
- 2023 年公开口径 $188,000 MRR（约 $2.26M ARR），11,000+ 付费用户，ARPU 不到 $20 [13]。2026 年 7 月官网：19,000 付费订户，累计追踪 2,600 亿页面浏览 [11]。
- 定价哲学是"必须便宜"：要替代一个免费产品，"We cannot achieve that by always charging more"——2021 年入门价 $6/月，当时竞品 Matomo 约 $30/月起 [4]。2026 年现价：Starter $9 / Growth $14 / Business $19 / Enterprise 定制，30 天免费试用、不要信用卡 [11]。
- 转化与留存数据：2020 年试用转付费 33.5% [2]；主动流失率（voluntary churn）每月略低于 2%，比行业均值低 52% [13]。
- 自愿承诺：2021 年 2 月起把毛收入的 5% 捐给环保事业和开源项目 [1]。

## 内容与增长

- Marko 的方法论一句话：**"Marketing is communication"**——不要把营销等同于"花钱投广告、刷屏、打扰、烦人" [15]。写教育性、信息性的文章，只在结尾提一句产品 [14]。
- 成名作：2020 年 4 月《Why you should stop using Google Analytics on your website》。发布后一周 48,000 独立访客——而此前 15 个月总共只有 27,300；一周新增 166 个试用，超过之前四个月总和；GitHub star 翻倍 [5]。
- 他最重要的一条经验："**The promotional work only starts after the blog post has been published**"——写完只是开始，要主动发到 Indie Hackers、Lobsters、Hacker News、Reddit（/r/degoogle、/r/opensource、/r/webdev）等相关社区 [5][2]。
- 执行强度：135 天里发了 15 篇博客（约每周一篇）+ 8 个千字以上的产品落地页；每天用 TweetDeck 监控关于 web analytics、GDPR、隐私的讨论并参与 [2]。
- 渠道结构（2020-04 至 07 实测）：Hacker News 43.6k 访客、Twitter 10k、Facebook 6.4k、Google 搜索 6.3k（质量最高、转化最好）、Indie Hackers 4.8k [2]。SEO 从零起步："My first goal was to get 10+ visitors from Google every day consistently"，九个月后 Google 每天带来 10+ 个试用注册（不是访客）[4]。
- 原创研究也是内容武器：一篇关于广告拦截器拦截率的研究 24 小时内 3 万人阅读 [1]。
- Build in public 本身就是营销：MRR 里程碑全部发在 IH、Twitter 和自家博客上 [1]，本档案引用的增长数据几乎全部来自他们自己的公开复盘——公开 metrics 让媒体、播客、案例作者（包括本书）免费替他们传播。
- 这套打法 2026 年仍在迭代：2026 年 1 月底重写首页（把功能区提前、按钮改成 "Start free trial"、砍掉一半文案），流量只涨 2% 的情况下试用注册涨 84%，2-4 月连续三个月刷新纪录，4 月单月新增 1,156 个付费订户 [10]。心得："Be obvious, be clear and don't make people work to understand what you're about."[10] 新变化：ChatGPT 引荐已成为流量来源之一 [14]。

## 社区

- 开源社区的真实经济学，他们算得很直白：自托管用户的捐赠每月约 $300——"We make $300 per month from donations from our self-hosted users. It would take us more than ten years of donations to pay one month of salary."[8] 养活团队的是云订阅用户，不是开源社区。
- 但社区的价值在别处：GitHub 是持续的获客与信任渠道（爆文当周 1,400+ 开发者访问 repo、star 翻倍 [5]）；Indie Hackers 社区是第一批用户和长期口碑放大器 [3]。
- 回馈机制：毛收入 5% 捐给开源和环保 [1]。

## 留存

- 主动流失率每月不到 2%，比行业均值低 52%；ARPU 不到 $20——低价 + 低流失 + 高试用转化（33.5%）构成复利结构 [13][2]。
- 支持策略是"文档代替客服"：完善的文档把支持量压到两位创始人兼职能处理的程度，直到 $500k ARR 才雇第一个兼职客服 [4][3]。

## 转型

- 许可证两连跳，都是被"白嫖"逼的：2019-09 以 MIT 完全开源；2020-10-12 改为 AGPL——起因是"There's been at least one case where a corporation has taken parts of our code, made it closed source and started selling it as a direct competitor"[7][1]。AGPL 堵住云漏洞：改了代码提供网络服务就必须开源修改 [7]。
- 2023 年第二跳：把 self-hosted 版更名为 **Plausible Community Edition（CE）**，每年只发两个版本，不含 Funnels、电商收入指标等商业功能，仅社区支持——目的仍是"prevent corporations from taking our code and using it as part of their closed-source proprietary products"，同时反制那些冒充官方、用非欧盟服务器转售 Plausible 的经销商 [8]。
- 这条线的本质：开源用来建立信任和分发，AGPL + CE 用来保护云业务这唯一的收入来源——开源与商业的边界是打出来的，不是设计出来的 [7][8]。

## 如何保持小

- 官网首页的自我定位（2026-07）："We're a completely independent, self-funded, bootstrapped and profitable team of 10, running since 2018. **No outside investors, no acquisition targets.**"[11]
- 团队扩张刻意缓慢：1 人（2018）→ 2 人（2020-03）→ 3 人（2021-06）→ 4 人（2022-02，$1M ARR 时）[1] → 8 人（2023，靠 12,000+ 云订户养活）[8] → 10-11 人（2025-2026，远程分布，含兼职贡献者）[11][14]。
- **每周四天工作制**："Most of the team works four days a week, with flexible hours and locations."[14] 增速与压力的取舍说得很明白："Doubling growth speed would require trade-offs—more pressure, faster feature delivery, more stress."[14]
- 拒绝投资人的完整论证（专门写了一篇博客）：从未拿过一分钱投资 [6]；自由——"Saying no to investors buys us freedom"[6]；隐私——投资人会逼你找"别的赚钱方式"，而分析工具最容易的"别的方式"就是卖用户数据 [6]；目标——"**Real success for us is sustainable financial freedom and not a glorified exit.**"[6]
- 不追增长的底气："We don't need to force any growth as we don't have to answer to any investors."[1]
- Bootstrap 保留选择权："Bootstrapping keeps our options open: sell later or never, stay niche, step back without collapsing the company."[6]

## 开放问题（值得当面问创始人的）

1. 对手免费是最硬的约束：试用流失里有多大比例最终还是回到了"GA 免费"？你们内部如何度量"隐私付费意愿"的天花板——19,000 订户离天花板还有多远？
2. 首页写着 "no acquisition targets"——收到过的最大收购要约是什么量级？拒绝时你和 Uku 之间有过分歧吗？有没有一个"什么价格都不卖"的明确约定？
3. Marko 在项目已运行 14 个月、$400 MRR 时以联合创始人身份加入——股权当时怎么谈的？现在回看，"给营销人真正的 co-founder 股权"是不是这家公司最重要的一个决定？
4. 把 self-hosted 改名 CE、降低发布频率、砍掉商业功能——开源社区的反弹有多大？有没有量化过 CE 用户转化为云付费的比例，还是它纯粹是信任装置？
5. 四天工作制 + 10 个人，对面是 Matomo、Fathom、Simple Analytics 和 GA4 本身——有没有哪个具体机会是因为"保持小"而明确放弃或错过的？AI 把内容生产成本打到零之后，你那套"写作 + 社区分发"的方法论还剩多少护城河？

## 来源

1. https://plausible.io/blog/open-source-saas — How we built a $1M ARR open source SaaS（2022-06）
2. https://plausible.io/blog/startup-marketing — From $400 to $2,750 MRR in 135 days（2020）
3. https://plausible.io/blog/bootstrapping-saas — How we bootstrapped to $500k ARR（2021）
4. https://plausible.io/blog/growing-saas-mrr — What we learned on our journey to $10,000 MRR（2021-01）
5. https://plausible.io/blog/blog-post-changed-my-startup — How one blog post changed the traction for my startup（2020）
6. https://plausible.io/blog/customers-not-investors — Why we say no to investors and are 100% user-supported
7. https://plausible.io/blog/open-source-licenses — Open source licensing: why we chose AGPL（2020-10-12）
8. https://plausible.io/blog/community-edition — Introducing Plausible Community Edition（2023）
9. https://plausible.io/blog/launching-plausible — I'm launching Plausible（Uku Täht，2019-04-29）
10. https://plausible.io/blog/homepage-edits-conversion-lift — How simplifying our homepage helped increase trial signups by 84%（2026-05）
11. https://plausible.io/ — 官网首页（2026-07 抓取）
12. https://plausible.io/about — 官网 About 页（2026-07 抓取）
13. https://www.indiehackers.com/post/from-400-mo-to-188-000-mo-in-3-years-marko-saric-of-plausible-tells-us-how-he-did-it-7a4e821834 — Indie Hackers 访谈（2023）
14. https://churnkey.co/subscription-heroes/how-plausible-grew-to-1m-arr-without-ads-or-investors-marko-saric-co-founder-of-plausible/ — Subscription Heroes 播客 #24（2025）
15. https://dev.to/wasp/meet-marko-saric-co-founder-of-privacy-friendly-plausible-analytics-3nm8 — Wasp 访谈 Marko Saric（2025-02）
16. https://en.wikipedia.org/wiki/Plausible_Analytics — Wikipedia 条目
17. https://carlanderson.xyz/saas-growth/episode-6/ — Carl Anderson 访谈 Marko Saric（2024-02，12,600+ 订户）
18. https://getlatka.com/companies/plausible-analytics — Latka 第三方营收估算（非官方，仅供参考）
