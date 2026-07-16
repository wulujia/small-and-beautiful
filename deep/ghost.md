# Ghost（John O'Nolan）

> 在 WordPress 的臃肿和 Substack 的抽成之间，做"只为独立出版者服务、且永远不能被卖掉"的开源出版平台 ｜ ghost.org ｜ John O'Nolan + Hannah Wolfe ｜ 2013（概念 2012-11）｜ 34-35 人全远程 ｜ 非营利基金会 + 开源 + SaaS 托管 ｜ ARR 约 $10.9M（2026-07 公开面板）[1][4]

## 缝隙切入点

- John O'Nolan 原是 WordPress 核心 UI 团队的活跃贡献者，眼看 WordPress 从"简单的博客工具"膨胀成复杂 CMS，且对生态内的"office politics, drama, and conflicts of interest"（办公室政治、内斗和利益冲突）感到失望 [2][3]。
- 2012 年 11 月他发了一篇概念博文，问题只有一个：如果把 WordPress 推倒重来、只为写作和新闻出版服务，会是什么样？项目名和口号直接把缝隙写在脸上——"Ghost: Just a blogging platform"（就是个博客平台，别的不干）[2][9]。
- 缝隙的另一半是制度层面的：他在概念博文里写下当时被批评最多的一句话——"No corporate arm of the law. Ghost would be free as in Mozilla, not as in Automattic ... Every decision made would be about improving the software, not the bottom line."（Ghost 的自由是 Mozilla 式的，不是 Automattic 式的；每个决策都为改进软件，而不是为利润表）[12]。产品缝隙 + 结构缝隙，从第一天就是一体的。

## 时机

- 2012-2013：WordPress 越做越重、Medium 等封闭平台崛起，"简单的开源博客工具"出现真空——概念博文一周 25 万浏览、上 Hacker News 首页，验证了饥渴程度 [6]。
- 2019：广告模式的问题被广泛讨论，Stratechery、De Correspondent、Patreon 证明订阅制出版可行，Ghost 3.0 赶在 newsletter 浪潮起飞前内置了会员订阅功能 [16][18]。
- 2024 年 1 月：Substack 的纳粹内容审核危机爆发，Casey Newton 的 Platformer（17 万订阅者）公开宣布迁往 Ghost，成为标志性事件——Ghost 十年"反平台"定位在一夜之间变成行业头条 [11]。
- 2024-2025：中心化社交平台信任崩塌、fediverse 兴起，Ghost 宣布并落地 ActivityPub 联邦化，再次踩中周期 [10]。

## 差异化

- **制度上的"自我锁死"**：Ghost 是非营利基金会（注册于新加坡），没有股份资本——John 和 Hannah 不持有任何股份、资产、域名或商标，一切归基金会所有。公司**不能被收购、不能分红**，100% 收入再投入产品和社区 [1][2][3]。John 的原话："The primary purpose of the non-profit structure is to protect against this and ensure that any decisions made benefit the organisation."（非营利结构的首要目的就是防止利润被抽走，确保决策只为组织本身）[3]。这不是姿态：它同时也锁死了创始人自己的退出通道。
- **0% 抽成对抗 Substack 10%**：Ghost 官方对比页的核心算术——1,000 个 $5/月的付费订阅者，年收入 $60,000，用 Ghost 托管年付约 $348，用 Substack 一年被抽走 $6,000 [7]。Jack Dorsey 公开替 Ghost 站过台："why not use Ghost instead? Is the payment you get from Substack greater than the freedom Ghost would provide?" [7]
- **开源兜底**：MIT 协议，出版者的 Stripe 账户直连、订阅者名单归自己。Ghost 的说法是"if Ghost the company disappears, you can continue to run your membership business in perpetuity"（就算 Ghost 公司消失，你的会员业务照跑不误）[7]。
- **公开 metrics 传统**：ghost.org/about 挂着实时财务面板（ChartMogul API 驱动），ARR、客户数、流失率全公开，从 2010 年代中期延续至今 [1][17]。

## 第一批用户/冷启动

- 2012-11 概念博文上 Hacker News 首页，一周约 25 万浏览，临时加了个表单，直接收了约 3 万邮件订阅 [6]。
- 2013-04-29 上 Kickstarter：目标 £25,000，**11 小时达标**，29 天最终 5,236 人支持、共 £196,362（约 78.5 倍超募）[2][9]。知名 backer 包括 Seth Godin、Leo Babauta、Darren Rowse，以及 WooThemes、Envato、微软等公司 [2]。
- Kickstarter 期间邮件列表从 3 万涨到 8 万；2013 年 9-10 月正式发布（首版代号 Kerouac，先发给 backers），发布日注册超 10 万 [2][6]。
- John 对冷启动的复盘：Kickstarter 的价值不在钱，而在**验证付费意愿**——邮件列表只能证明兴趣，掏钱才算数 [6]。

## 收入与定价

- 商业模式一句话：免费开源内核 + 收费托管服务 Ghost(Pro)，"a sustainable business around a free core application, funded by a premium managed-service to run it on" [1]。
- 非营利结构反而逼出了财务纪律：基金会**不能融资、不能贷款**，Ghost(Pro) 上线后 **11 个月内盈利**，此后 12 年持续自给自足，不靠捐赠和 grant [1][6]。
- 定价教训（2017 年复盘）："We've doubled our prices 3x since then, and each time we do, we get nicer people who value the product more and create fewer problems."（三次翻倍涨价，每次涨价换来更好的客户）以及 "I would never create a business ever again which charges less than $10/month."（再也不会做低于 $10/月的生意）[6]。
- 现行定价（2026）：Starter $18/月、Publisher $29/月、Business $199/月、Custom 面议（年付价，按会员数分级），付费订阅功能明确标注"没有任何来自 Ghost 的额外交易抽成" [8]。
- 营收轨迹：2017 年 $750K/年（10 人）[6] → 2019 年累计客户收入 $5M [18] → 2025-05 ARR $8M（34 人）[4] → 2026-07 公开面板 ARR $10,884,111、30,441 个付费客户、净流失率 3.05% [1]。
- 累计账本（2025-08）：托管收入共 $36M；同期独立出版者通过 Ghost 赚到 **$100M+**（Ghost 一分不抽）[5]。

## 内容与增长

- 增长引擎是"透明本身"：公开财务面板、公开 changelog、公开复盘（如《Two Years In: How We Spent the Kickstarter Money》）——每个里程碑都是一篇可传播的内容 [1][17]。
- John 的个人博客持续输出高传播故事：《A decade after being rejected by YC》——当年想向 YC 要 $120K 换 7% 股份，被拒两次；十年后 Ghost 从客户手里赚了 $25M+、出让 0% 股权，而 YC 自己的博客跑在 Ghost 上 [13]。
- 对比页营销做得极其锋利：ghost.org/vs/substack 直接列出算术账和已迁移的出版物（The Browser、Tangle、Webworm 等），并内置 Substack 迁移向导（一键导入免费/付费订阅者）[7]。
- 大客户即案例：OpenAI 的博客最初就是一个 Ghost 站——ChatGPT 发布高峰期，Ghost 为 OpenAI 服务的流量超过其他所有出版者总和 [4]。其他用户包括 404 Media、Kyiv Independent、Sky News、Tinder 等 [2][4]。

## 社区

- 开源社区是护城河的一部分：GitHub 54,000+ stars，累计安装量 1 亿+ [1]。
- 初始社区就是那 5,236 个 Kickstarter backer——他们不是投资人（拿不到股份，因为根本没有股份），而是"想让这个东西存在"的捐赠者，这个基调塑造了此后的社区关系 [9][3]。
- 治理开放化：John 在 2024 年公开计划扩大基金会理事会、引入社区选举席位，防止任何个人（包括他自己）长期控制 Ghost 的方向 [3]。

## 留存

- 公开面板显示净 MRR 流失率 3.05%（2026-07）[1]。
- 留存逻辑是反直觉的"零锁定"：内容可整站导出、订阅者名单归出版者、Stripe 直连（钱不经过 Ghost 的手）、开源代码兜底。离开的成本被刻意做到最低，信任反而成了留下来的理由 [7]。官方的说法：出版者"switch for the better writing experience, stay for the ownership"（为写作体验而来，为所有权而留）。

## 转型

Ghost 有两次改变公司性质的转向，都是"在原缝隙里挖深"而不是换赛道：

1. **2019，Ghost 3.0：从 CMS 到出版业务操作系统**。内置会员与付费订阅（Stripe 直连、0 抽成），从"帮你发布内容"变成"帮你靠内容赚钱"[16][18]。这次转型让 Ghost 从与 WordPress 竞争的工具，变成了与 Substack 竞争的商业基础设施——后来的 $100M 出版者收入全部由此而来 [5]。
2. **2024-2025，ActivityPub 联邦化**。2024-04 宣布加入 fediverse [10]，2025-08-05 发布 Ghost 6.0：读者可以从 Mastodon、Threads、Bluesky、Flipboard 直接关注一个 Ghost 站点，内容分发不再依赖中心化算法 [10]。John 称这是"most requested feature over the past few years"，但也坦承最大的不确定是用户能不能"get"它——"terms like ActivityPub, Fediverse, bridge, protocol, server are alienating and confusing"（这些术语让普通人望而生畏）[10]。

创始人自己也有一次"转型"：John 成长期就在各国搬家（荷兰、菲律宾 7 年），成年后边环球旅行边远程运营 Ghost 十余年，是数字游民的标志性人物（2025 年初资料显示常驻迪拜）；2026-05-31 他发布视频《The End of My Digital Nomad Era: Why I'm Settling Down》，宣布结束 12 年游民生活、定居下来 [15]。公司从第一天全远程，创始人却从"永远在路上"走到了"停下来"。

## 如何保持小

- **34-35 人做到 $8-11M ARR**，全远程、跨 5 大洲 16 个国籍，2013 年至今没有办公室 [1][4]。
- 结构性地拒绝了"必须变大"的压力源：没有投资人要回报、没有股东要退出、创始人没有股份可套现。John 的表述：作为非营利组织"we can just keep reinvesting 100% of what we make into improving the product"（我们可以永远把 100% 的收入投回产品）[4]。
- 组织刻意轻流程：多数人每周只有 1-2 个 Zoom 会议，日历留白给创造性工作；扁平、自由协作，招人时明确排斥"fixing media / changing the world"式的宏大叙事者 [14]。
- 增长节奏是"organic and steady"（自然而平稳）而非指数式——这是 John 自己的定性，从 2017 年说到现在 [6]。

## 开放问题（值得当面问创始人的）

1. 非营利结构锁死了退出，也锁死了用股权吸引人才的手段。34 人团队 13 年，靠什么留住最好的工程师和设计师？有没有因为"给不了期权"而错失关键人才的具体时刻？
2. Kickstarter 超募 78 倍验证的是"WordPress 难民"的需求，但 2019 年后 Ghost 实际服务的是"Substack 难民"。这次用户群体的置换是主动设计还是被市场推着走的？中间有没有差点做错的岔路？
3. ActivityPub 是 Ghost 第一次把赌注押在一个尚未被大众理解的协议上。如果三年后联邦化被证明是小众玩具，Ghost 6 投入的机会成本怎么算？止损线在哪里？
4. 公开 metrics 十年，有没有哪个时刻公开数据反过来伤害了 Ghost（竞争对手利用、低谷期的舆论压力）？为什么绝大多数公司学不了这一招？
5. 你个人结束游民生活定居的决定，和 Ghost 进入"稳态运营"之间有因果关系吗？一个"永远不能卖掉的公司"的创始人，如何规划自己的第二曲线（Vintas、RSS reader 等 side project 是解药吗）？

## 来源

- [1] Ghost 官方 About 页（含实时公开财务面板）：https://ghost.org/about/ （2026-07 抓取：ARR $10,884,111、客户 30,441、净流失 3.05%、35+ 人）
- [2] Wikipedia: Ghost (blogging platform)：https://en.wikipedia.org/wiki/Ghost_(blogging_platform)
- [3] John O'Nolan, "Democratising publishing"（2024-10-30）：https://john.onolan.org/democratising-publishing/
- [4] John O'Nolan, "12 years of Ghost"（2025-05）：https://john.onolan.org/12/
- [5] John O'Nolan, "$136M"（2025-08-18）：https://john.onolan.org/136m/
- [6] Indie Hackers 访谈 "How John O'Nolan Grew Ghost to $750,000/year"（2017-02）：https://www.indiehackers.com/interview/how-john-onolan-grew-his-publishing-platform-to-750-000-year-14e5bac2fa
- [7] Ghost 官方对比页 "Ghost vs Substack"：https://ghost.org/vs/substack/
- [8] Ghost(Pro) 定价页：https://ghost.org/pricing/
- [9] Kickstarter 项目页 "Ghost: Just a Blogging Platform"（5,236 backers / £196,362）：https://www.kickstarter.com/projects/johnonolan/ghost-just-a-blogging-platform
- [10] TechCrunch "Substack rival Ghost confirms it will join the fediverse in 2024"（2024-04-22）：https://techcrunch.com/2024/04/22/substack-rival-ghost-confirms-it-will-join-the-fediverse-in-2024/ ；Ghost 6.0 发布报道（2025-08）：https://www.webpronews.com/ghost-6-launches-fediverse-integration-via-activitypub/ ；Flipboard 访谈：https://about.flipboard.com/fediverse/john-onolan-ghost/
- [11] Casey Newton, "Why Platformer is leaving Substack"（2024-01）：https://platformer.substack.com/p/why-platformer-is-leaving-substack
- [12] John O'Nolan on X（2024-09，回顾 2012 年原文）：https://x.com/JohnONolan/status/1839672759384784910
- [13] John O'Nolan, "A decade after being rejected by YC"（2024-03-22）：https://john.onolan.org/（文章列表）
- [14] Ghost Careers（团队文化与工作方式）：https://careers.ghost.org/
- [15] John O'Nolan, YouTube "The End of My Digital Nomad Era: Why I'm Settling Down"（2026-05-31）：https://www.youtube.com/watch?v=pt4bwINCj24
- [16] TechCrunch "Ghost CMS adds open-source subscription and membership options"（2019-10-23）：https://techcrunch.com/2019/10/23/ghost-cms-adds-open-source-subscription-and-membership-options/
- [17] ChartMogul 访谈 "How we built the non-profit, distributed SaaS company of our dreams"（2017-03）：https://chartmogul.com/blog/ghost-founder-ceo-john-onolan/
- [18] Ghost 3.0 发布公告 "The story behind raising $5m"（2019-10）：https://ghost.org/changelog/3-0/
