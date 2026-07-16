# Obsidian

> 在 Notion/Roam 云端数据库笔记统治的赛道里，用"本地 Markdown 文件 + 永不锁定"切开信任缝隙 ｜ obsidian.md ｜ Shida Li & Erica Xu（滑铁卢大学同学，华裔加拿大）｜ 2020 ｜ 约 7 名全职（官网列 8 人 + 一只猫）[1][9] ｜ PKM / 笔记工具 / 本地优先 ｜ 营收未公开，官方仅确认持续盈利、无外部融资 [9][19]

## 缝隙切入点

- 2020 年前后主流笔记应用（Notion、Evernote、Roam）都把数据放进云端数据库；Obsidian 反着来：给用户一个本地文件夹，全部是 Markdown 明文，用户自己管 [4]。Fast Company 的概括："While apps like Notion put all your notes in the cloud... Obsidian gives users a folder full of files and puts them in charge of managing it." [4]
- 起点是联合创始人 Erica Xu 的个人痛点。她自述是"会为自己一个人搭私有 MediaWiki"的人（"I'm the kind of person who sets up a private MediaWiki instance just for myself"），试遍 TiddlyWiki 等工具后列了一张"圣杯笔记应用必须打勾的清单"（"I made a list of boxes that must be checked by my holy grail note-taking app"），这张清单长成了产品 [2]。
- 这个缝隙后来被现任 CEO Steph Ango 提炼成传播力极强的哲学"File over app"（2023-07-01 成文）："If you want to create digital artifacts that last, they must be files you can control"；"Apps are ephemeral, but your files have a chance to last"；"If you want your writing to still be readable on a computer from the 2060s or 2160s, it's important that your notes can be read on a computer from the 1960s." [5]
- 配套承诺：核心应用免费、无限制、不用注册账号（官网原文 "Free without limits. No sign-up required. No strings attached."），且不收集任何用户数据 [11][6]。

## 时机

- 两人此前已合作做了大纲工具 Dynalist（2015 年起），在笔记工具上有五年积累 [3][16]。
- 2020 年初 COVID 隔离期间动手开发，2020 年 3 月底发布公测——正好撞上 Roam Research 在 2019-2020 年引爆的双链笔记 /"tools for thought" 浪潮 [3][16]。Roam 走 VC + 高价订阅路线，Obsidian 以"免费 + 本地 + 可扩展"接住了这波被教育起来但不愿付月费、不愿把第二大脑放在别人服务器上的人群 [16][4]。
- 到 2020 年 9 月，Discord 社区已破 1 万人 [16]。

## 差异化

- 本地明文文件 vs 云端数据库：不做账号体系、不做遥测，甚至刻意不做 Web 版 [3][11]。
- 像代码编辑器一样可扩展。Erica："if I don't like how Visual Studio Code looks or works, I can customize almost every aspect of it. Why can't we do this to notes?"——插件化从第一天就是设计目标，而非后补 [2]。
- Kepano 在 Decoder 访谈中的说法："If Obsidian is not working the way you want, you can pretty much change it very fast." [9]
- 差异化的另一半是公司形态本身：2023-02-06（Ango 出任 CEO 当天）他公开写道，Obsidian "Free for personal use / Built on durable open file formats, no lock-in / Private, offline-first, and E2E encrypted / Endlessly customizable via API... Above all, Obsidian is 100% user-supported. There are no investors pushing us to compromise on these values." [8]

## 第一批用户/冷启动

- 需求验证来自 Hacker News 上关于笔记工具的讨论——他们从中确认"市面上没有满足这些条件的工具，但想要的人很多" [2]。
- 私测阶段用 Discord 发放测试资格，社区是"意外"长出来的；后来补建 Discourse 论坛解决信息沉淀问题（Erica 总结：Discord 提供实时氛围和管理工具，论坛解决内容组织） [2]。
- 第一笔收入是 beta 期的 Catalyst 许可：25 美元一次性付款，本质是"打赏 + 提前用 beta 版 + Discord VIP 身份"，把最热心的早期用户变成了资助者 [17]。
- 中文社区是冷启动期的意外强区：2021 年 9 月，Discord 破 4 万人时，官方把第一个官方非英语论坛给了中文社区（forum-zh.obsidian.md），当时中文社区已有 330 个插件的开发者和 13 位社区管理员 [14]。

## 收入与定价

- 结构：软件免费，钱全在"服务"上——Sync（端到端加密同步，年付 $4/月，月付 $5）、Publish（笔记建站，年付 $8/站/月）、Catalyst（$25 一次性）、商用许可（$50/人/年） [11][9]。
- Sync 曾从 $8/月降到 $4/月（年付），主动砍价一半 [20]。
- 2025-02-20 宣布"Obsidian is free for work"：商用许可从强制改为自愿购买，官方理由是"The Commercial license terms were confusing and added unnecessary complexity to our pricing"，并称此举更符合使命——"everyone should have the tools to think clearly and organize ideas effectively" [12]。
- 营收从未公开。Kepano 在 Decoder（2025-08-18）只确认盈利并解释逻辑："Because the team is small, we don't need mountains of cash to pay for that." [9] 第三方 ARR 估算从 $2M 到 $25M 不等，差异 10 倍以上，均非官方数字，不可采信 [19]。

## 内容与增长

- 不投广告、不做增长黑客、不收数据，增长引擎是两个：插件社区 + CEO 的公开写作。
- Kepano 的"三个永不"声明（2023-08-25）本身成了传播事件："The plan for Obsidian is to never grow beyond 10-12 people, never take VC funding, never collect personal data or analytics." [6]
- 他 2024 年 2 月再次系统阐述拒绝 VC 的理由："1. We want to stay small... 2. We follow strict principles that we do not want to compromise 3. Our users are happy to support us"，并给出金句"VCware is built with a five year horizon, it is not built to live on for decades" [7]。
- 里程碑数字：2023 年 10 月 Fast Company 报道时约 100 万用户（官方估算），Discord 超 11 万人，Reddit 9.46 万（全站 top 5%） [4]；2025 年 2 月 Kepano 在 Dialectic 播客称 "seven people full-time serving probably three or four million users" [10]。
- 生态型 KOL（Nicole van der Hoeven、Linking Your Thinking 的 Nick Milo 等）的教程和课程构成了官方之外的内容增长层 [16][9]。

## 社区

- 插件生态是真护城河：自 2020 年开放 API 以来，社区累计创建 4,000+ 插件和主题，总下载量超 1.2 亿次（官方博客，2026-05-12） [13]。Kepano："The community ecosystem is one of the most fun and powerful aspects of Obsidian." [13]
- 社区能内生领导层是最硬的证据：Kepano 本人就是社区出身——他做的 Minimal 是下载量最大的社区主题 [18]，先以外部贡献者身份受邀设计 1.0 版界面，再于 2023-02-06 出任 CEO [3][9]。
- 2026 年 5 月上线 "Obsidian Community" 目录：自动安全扫描、安全评分卡、开发者后台，把插件分发从 GitHub 列表升级成受管生态——7 人团队用自动化而非人力扩张来管理 4,000+ 插件的风险 [13]。

## 转型

- Obsidian 最独特的"转型"不是产品线，而是治理：创始人在公司第三年把 CEO 让给一个超级用户。Shida Li 转任 CTO、Erica Xu 转任 COO，回到最擅长的产品开发；Steph Ango 2023-02-06 接任 CEO [1][3]。他先以合同工身份参与 1.0 设计，角色逐步演化成 CEO [9]。
- Ango 的履历构成完美反差：他联合创办的 Lumi（包装供应链 SaaS，YC W15）2018 年拿了 Spark Capital 等 $9M A 轮 [15]，2021 年卖给 Narvar [21]——一个走完 VC 全流程的人，回头选择了用户供养模式。他接手时说："I can't overstate how life-changing Obsidian has been for me... I want to see what happens if more people gain that superpower."
- 产品节奏佐证"慢而稳"：公测两年半后才发 1.0（2022-10-13），随后 Canvas（2022-12）、Properties（2023）、Bases 数据库视图（2025）、Community 目录（2026-05） [3][16][13]。

## 如何保持小

- 公开自缚的"三个永不"：团队永不超过 10-12 人、永不拿 VC、永不收集用户数据 [6]。官网 Manifesto 落款是 "100% supported by our users, not investors" [1]。
- 全职 7 人（其中约 3 名工程师），服务三四百万用户 [9][10]。Kepano（Decoder，2025-08）："Obsidian, we have one meeting per year." [9]
- 主动放弃招聘杠杆。Kepano 对比 Lumi 时期"出问题就去雇最好的人"的打法，称在 Obsidian "hiring is off the table"，并直言 "I don't really enjoy being a manager"；他给这种模式起的名字："I just like the Ocean's Eleven model the best." [10]
- 保持小是定价的前提而非结果：因为不需要养大团队，才能把 Sync 砍半价、把商用许可改成自愿 [9][12][20]。

## 开放问题（值得当面问团队的）

1. 免费本地用户到 Sync/Publish 付费的转化漏斗大概什么量级？最大流失发生在哪一步？
2. 2023 年把 Sync 从 $8 降到 $4、2025 年把商用许可改自愿——这两次"主动少收钱"的决策内部怎么算账？实际营收影响如何？
3. CEO 交接是谁先开的口？让非创始人超级用户接任 CEO，股权和激励怎么安排，"永不卖、永不融资"在三个人之间有没有制度化约束（还是纯靠默契）？
4. 拒绝 VC 之后收购要约怎么处理？有没有报价高到内部认真讨论过的时刻？
5. 中文用户占比多少？2021 年为什么第一个官方非英语论坛给了中文社区，如今 7 人团队如何维护它？

## 来源

- [1] Obsidian About（Manifesto、团队名单）— https://obsidian.md/about
- [2] Ness Labs 访谈联合创始人 Erica Xu — https://nesslabs.com/obsidian-featured-tool
- [3] Wikipedia: Obsidian (software) — https://en.wikipedia.org/wiki/Obsidian_(software)
- [4] Jared Newman, "The cult of Obsidian", Fast Company, 2023-10-13 — https://www.fastcompany.com/90960653/why-people-are-obsessed-with-obsidian-the-indie-darling-of-notetaking-apps
- [5] Steph Ango, "File over app", 2023-07-01 — https://stephango.com/file-over-app
- [6] kepano 帖子（"三个永不"），2023-08-25 — https://mastodon.social/@kepano/110945642295048699
- [7] kepano（X），"Why @obsdmd is 100% user-supported"，2024-02 — https://x.com/kepano/status/1756468726743122140
- [8] kepano（X），出任 CEO 当日声明，2023-02-06 — https://x.com/kepano/status/1622648628379787264
- [9] Decoder with Nilay Patel（The Verge），"How the head of Obsidian went from superfan to CEO"，2025-08-18 — 笔记：https://www.podchemy.com/notes/how-the-head-of-obsidian-went-from-superfan-to-ceo-41358848188 ；另见 https://www.daniel.pizza/links/decoder-obsidian-kepano/
- [10] Dialectic Ep. 8: Steph Ango（Jackson Dahl 主持），2025-02 — https://jacksondahl.com/dialectic/steph-ango ；引文见 https://x.com/jacksondahl/status/1889022922401964512
- [11] Obsidian Pricing — https://obsidian.md/pricing
- [12] kepano, "Obsidian is free for work", Obsidian Blog, 2025-02-20 — https://obsidian.md/blog/free-for-work/
- [13] kepano, "The future of Obsidian plugins", Obsidian Blog, 2026-05-12 — https://obsidian.md/blog/future-of-plugins/
- [14] 《Obsidian 官方中文论坛成立啦》，知乎，2021-09 — https://zhuanlan.zhihu.com/p/409594116
- [15] TechCrunch：Lumi 获 $9M 融资，2018-02-14 — https://techcrunch.com/2018/02/14/meet-lumi-the-los-angeles-startup-that-just-raised-9-million-for-a-packaging-business/
- [16] Taskade, "History of Obsidian"（时间线；其营收/估值数字为第三方估算，未采用）— https://www.taskade.com/blog/obsidian-history
- [17] Obsidian Help: Catalyst license — https://help.obsidian.md/catalyst
- [18] Minimal 主题（kepano/obsidian-minimal，下载量第一的社区主题）— https://github.com/kepano/obsidian-minimal ；https://facedragons.com/foss/best-obsidian-themes/
- [19] Fueler：Obsidian statistics（明确标注营收/估值均为第三方估算、官方未披露）— https://fueler.io/blog/obsidian-usage-revenue-valuation-growth-statistics
- [20] eesel：Obsidian pricing（记录 Sync 由 $8 降至 $4）— https://www.eesel.ai/blog/obsidian-pricing
- [21] Wikipedia: Lumi (company)（2021 年被 Narvar 收购）— https://en.wikipedia.org/wiki/Lumi_(company)
