# PocketBase（Gani Georgiev）

> 单文件开源后端（Go + 内嵌 SQLite，Firebase/Supabase 替代）：一个人、零收入、零营销做到近 6 万 star、大量生产环境使用 ｜ pocketbase.io ｜ Gani Georgiev ｜ 保加利亚 ｜ 2022 ｜ 1 人 ｜ oss-nonprofit / 开发者工具 ｜ 收入 $0——非商业项目，2024 年起主动拒收个人捐赠 [2][3][6]

全库唯一的"反收入"样本：别人研究怎么收钱，他研究怎么把钱挡在门外。价值在于给"小而美"划出光谱的另一端——小到连商业都不要，靠什么维持？

## 缝隙切入点

PocketBase 最初不是产品，是自用件："initially created to be the backend for the next version of my other open source project - Presentator v3"——他想要一个"可以自托管、几乎零配置、不依赖任何第三方服务"的后端，市面上没有，就自己写了一个 [1]。业余时间做了 3-4 个月，最后 4 周向日常工作请了长假来收尾，2022 年 7 月 21 日发 Show HN [1][2]。

缝隙的形状：当时 BaaS（Firebase、Supabase、Nhost）全在往"更大"做——托管服务、多容器、水平扩展、融资扩张；他反向压缩，把数据库（SQLite）、实时订阅、用户认证、文件存储、管理后台全部塞进**一个可执行文件**，下载即运行 [1][2][3]。HN 用户后来的总结最传神："Unlike Firebase, you can run it anywhere. Unlike Supabase, you don't need 10+ containers" [11]。

发布第一天他就公告了"不做什么"：PocketBase 只设计为单服务器运行，不支持水平扩展——"要 scale 请去用 Supabase 或 Nhost" [1]。把天花板写进定位，是这个项目一切"保持小"决策的起点。

## 时机

- 2022-07-05 建仓库，07-21 Show HN 拿下 563 分，评论区集中反应是"终于有不绑云服务、不用装一堆依赖的 Firebase 替代"——自托管需求在 BaaS 融资热的另一面积压已久 [1][2]。
- 对照组恰好同场：Supabase（2020 年创立）走的是标准 VC 路线，此后累计融资约 $10.4 亿 [15][16]。同一个缝隙（"开源 Firebase 替代"），两条路线同时开跑，四年后一边是 $105 亿估值 350 人，一边是 1 个人 0 收入——本案例的对照价值就在这里 [16]。

## 差异化

- 产品差异化 = 减法：单文件、单服务器、SQLite，官方 FAQ 称普通硬件可支撑 10,000+ 持久实时连接——对绝大多数应用，"不能水平扩展"根本不构成约束 [3]。
- 对竞品不攻击反而引流：作者自己推荐需要水平扩展的用户去用 Supabase/Nhost [1]。诚实的边界声明本身成了信任资产，HN 用户评价这个项目"so well thought out… there's a bit of soul" [11]。
- 商业结构上的差异化最极端：Supabase 融资 $10.4 亿、350 名员工、$105 亿估值 [15][16]；PocketBase 1 个人、$0 收入、MIT 协议 [2][3]。生产用户的真实账单是这样的：有用户用一台 $10/月的 Hetzner 服务器跑 5 个 PocketBase 实例，每天服务几千用户 [11]。

## 第一批用户/冷启动

- 冷启动就是一次 Show HN：563 分，此后增长全靠 GitHub 和口碑，2026 年 7 月达 59,761 stars、3,521 forks [1][2]。
- 无官网博客运营、无 Twitter/X 账号、无广告、无 Product Hunt 式打榜——本次调研检索不到他任何一次采访、播客或会议演讲记录；个人网站 gani.bg 只有一句话简介和一个 GitHub 链接；连 HN 用户名都不用实名，叫 "randomwebdev" [1][14]。增长引擎只有两个：产品本身 + 发布日志。
- 生产采用是真实的：HN 2025 年的讨论串里，用户报告跑着带 Stripe 支付的商业目录站、30 张表 1 万条记录 3GB 备份的应用，评价"never had it go down unexpectedly" [11]。

## 收入与定价（一部"拒绝史"）

他的收入时间线，方向和所有案例相反——每一行都是把钱推出去：

| 时间 | 事件 | 数字 |
|---|---|---|
| 2022.10 | 接受 Chrome Advanced Web Apps Fund 赠款（机构、无交付义务）："starting from November I'll be able to work full-time on PocketBase for at least 5 months" | $20,000 [4] |
| 2023.12 | 自述已靠个人积蓄全职开发约一年；当时月捐赠额 | ~285 BGN（约 $160）/月 [5] |
| 2024.01 | **停收个人捐赠**（关闭 sponsor 渠道） | 停收前最后一个月 ~320 BGN（约 $170）[6] |
| 2025.10 | 宣布接受 FLOSS/fund（印度 Zerodha 出资的开源基金）一次性赞助，计划全职一年发布稳定版 v1 | €30,000 [8][9] |
| 2026.02 | **主动撤回申请、放弃已到手的赞助**：基金与 GitHub 的合作因监管问题告吹，改为从印度直接电汇、需通过邮件传输大量跨境个人材料——"I don't feel comfortable doing that because I don't trust them, nor the India government, with processing and storing personal sensitive data" | −€30,000 [8][10] |
| 现状（2026.07） | FAQ：个人开源项目、无公司无团队；只接受"no strings attached"的机构赞助，邮件洽谈 | 经常性收入 $0 [3] |

停收捐赠的理由不是钱少，而是心理账务。2024 年 1 月他写道：捐赠附带"unspoken expectations"（隐性期待），"which only makes me feel guilty for not working on the demanded feature requests"——有用户因为他不给 v1 排期表达失望，他索性把捐赠通道关了 [6]。并立场声明："PocketBase is a non commercial project, developed entirely on volunteer basis, specifically for my own needs, and I don't plan to monetize it" [6]。

这条"什么钱能拿"的线其实清晰：**机构的、一次性的、无附加条件的可以（Chrome $20k）；个人的、持续性的、带隐性期待的不行（月捐 $170）；机构的但流程有风险的，宁可退掉（FLOSS/fund €30k）** [3][4][6][8]。他的区分标准是义务感而非金额——PocketBase"除了我的个人时间没有任何运营成本"，所以不需要钱；而他的另一个项目 Presentator 有真实托管开销，就正常接受捐赠 [6]。

值得注意的空缺：他自己一分不收，生态里别人在正常赚钱——第三方托管服务 PocketHost 按 $9.99/月/实例收费 [17]。他对此没有任何动作，MIT 协议下也无意分成。

## 社区（治理：一个人的秩序）

- **功能 PR 不经讨论不收**："PocketBase has a roadmap and I try to work on issues in specific order"，凭空而来的功能 PR 会"skew all initial planning"。最扎眼的一句写在贡献指南里："Don't get upset if I close your PR, even if it is well executed and tested"——但可能日后引用其实现并在发布日志致谢。Bug 修复、OAuth2 provider、文档 PR 欢迎 [12]。
- 2025-2026 年治理进一步收紧："Due to recent LLM spam, PRs are temporary disabled and only existing collaborators can open a PR"——AI 垃圾贡献潮之下，他干脆关闭了整个 PR 入口，贡献者需开 issue/discussion 附 fork 链接 [12]。
- 治理成效可量化：59,761 stars 的项目，**open issues 只有 18 个**（2026-07 查）——同量级开源项目通常积压数百上千。一个人反而做到了大团队做不到的收件箱清零 [2]。
- 对用户同样立规矩，FAQ 原文："If you don't have the time to at least skim through the documentation… and you plan to solely rely on some AI tool, then please do NOT use PocketBase!" ——公开劝退不读文档的用户 [3]。
- 沟通渠道单一化：他只在 GitHub discussions/issues 里说话，重大变化以 announcement discussion 发布，说完锁帖防刷 [8]。

## 转型

- 版本哲学：发布四年仍在 0.x（2026 年 7 月为 v0.39.7），拒绝给 v1 排期——"There are no ETAs. This is a hobby project and I don't want to make promises"（2023-12）[3][5]。0.x 不是烂尾信号，而是他保留破坏性重构自由的方式：他明确说想先用 PocketBase 做几个真实应用、验证内部设计，再锁定 API [7]。
- 走向 1.0 的路径（2026 年进行时）：全新重写的管理 UI 分两步发布，Stage 1（v0.37.0，2026-04-19 发布）无破坏性变更，含暗色模式、UI 扩展 API 雏形；Stage 2 将直接是 **v1.0.0-rc.1**，带破坏性 API 清理。他的说法："the main goal remains and I'll try to publish a stable PocketBase version this year"（2026-02）——但照例"NO ETAs" [8][13]。
- FLOSS/fund 的 €30,000 本来就是为这最后一程准备的（"fix long-lasting API warts… full-featured plugins support and finally publish a stable (v1) release"），钱退了，目标没退 [8][9]。

## 如何保持小

他把"一个人"从风险陈述成了选择，且论证得异常坦白：

- 直面 bus factor：2023 年有用户问"经理不敢用，PocketBase 会活下去吗"，他的回答以自贬开头："I'm just some random developer that burns through his savings. I can't and don't want to make any promises."——然后承认"having a bus factor of 1 is not great, but I don't want to maintain a team with random/spare contributors" [7]。
- 拒绝团队的理由：加人意味着精力从开发转向"people problems"；无偿贡献者凭什么要满足他的严苛标准？何况没人保证合并代码后还会留下来维护 [7]。
- 刻意收窄 scope 以匹配一个人的维护带宽，bug 出现即修 [7]。他不粉饰："managers' concerns are valid"，用不用 PocketBase 是团队自己要算的 tradeoff [7]。
- 拒绝一切制造义务感的东西：捐赠（隐性期待）、ETA（承诺压力）、路线图截止日期。他给自己保留的是"随时可以停"的权利——而这反而是他持续四年高强度维护的心理基础 [5][6]。
- 零公开露面是同一逻辑的延伸：不做个人品牌，不接受采访，让项目只以代码和文档的形态存在。个人网站一页纸，正文一句话 [14]。
- 财务上的"保持小"最硬核：不融资、不商业化、拒收捐赠，靠积蓄 + 偶发的无条件机构赠款全职开发 [4][5][6]。这也是全库最脆弱的可持续性模型——它成立的前提是保加利亚的生活成本、他的积蓄厚度和他的意愿三者同时在线。

## 开放问题（值得当面问本人的）

1. 靠积蓄全职做非商业项目四年，你给自己设过财务底线吗？积蓄到什么水位会触发什么动作——回去接活、放慢 PocketBase，还是重新考虑商业化？
2. "什么钱能拿"这条线：Chrome 的 $20k 接了，个人月捐 $170 停了，FLOSS/fund 的 €30k 先接后退。隐性期待（个人捐赠）和显性合同（机构赠款），哪种义务感对你更有杀伤力？如果 GitHub 明天出一个"真正零附加条件"的打款机制，你会重开吗？
3. Bus factor = 1 的身后事：除了 MIT 协议 +任何人可 fork，你有没有做过任何实际安排——继任者人选、转基金会托管、一份"我消失了怎么办"的交接文档？还是你认为对一个非商业项目来说，"死掉也是可接受结局"？
4. v1.0 锁定 API 之后呢？这个项目对你的乐趣有多少来自"还能随时推翻重来"的自由？稳定版发布那天，你是继续投入、转回 Presentator，还是开始下一个自用件？
5. 2022 年 Show HN 爆火后，有 VC 或 Supabase 类公司找过你吗（投资、收购、雇佣）？拒绝（如果有）的具体过程和理由是什么——是没谈拢，还是根本没进入谈的阶段？

## 来源

1. Show HN: PocketBase – Open Source realtime backend in one file（2022-07-21，563 分，含作者以 randomwebdev 身份的评论）— https://news.ycombinator.com/item?id=32013330
2. GitHub pocketbase/pocketbase 仓库（stars/forks/issues 数据经 GitHub API，2026-07-16 查）— https://github.com/pocketbase/pocketbase
3. pocketbase.io FAQ（资助立场、生产就绪声明、当前版本）— https://pocketbase.io/faq/
4. Discussion #730 "Chrome Advanced Web Apps Fund sponsorship"（2022-10-06）— https://github.com/pocketbase/pocketbase/discussions/730
5. Discussion #4036 "Date for version 1.0???"（2023-12-27）— https://github.com/pocketbase/pocketbase/discussions/4036
6. Discussion #4199 "No longer accepting donations"（2024-01-21）— https://github.com/pocketbase/pocketbase/discussions/4199
7. Discussion #3087 "Will PocketBase survive?"（2023-08-08）— https://github.com/pocketbase/pocketbase/discussions/3087
8. Discussion #7287 "(Cancelled) ~FLOSS/fund sponsorship~ and UI rewrite"（2025-10-29 宣布，2026-02-18 取消）— https://github.com/pocketbase/pocketbase/discussions/7287
9. FLOSS/fund PocketBase 资助计划页（€30,000 一次性，用途说明）— https://dir.floss.fund/view/funding/@pocketbase.io
10. HN "Pocketbase lost its funding from FLOSS fund"（2026-02-18，125 分）— https://news.ycombinator.com/item?id=47062561
11. HN "Pocketbase – open-source realtime back end in 1 file"（2025-11-28，生产使用报告与 bus factor 讨论）— https://news.ycombinator.com/item?id=46075320
12. CONTRIBUTING.md / README（PR 政策、LLM spam 关闭 PR）— https://github.com/pocketbase/pocketbase/blob/master/CONTRIBUTING.md
13. Discussion #7612 "Upcoming new UI release…"（2026-04-03，v0.37.0 与 v1.0.0-rc 计划）— https://github.com/pocketbase/pocketbase/discussions/7612
14. gani.bg 个人主页 — https://gani.bg/
15. TechCrunch: Supabase nabs $5B valuation（2025-10-03）— https://techcrunch.com/2025/10/03/supabase-nabs-5b-valuation-four-months-after-hitting-2b/
16. CNBC: Supabase raises $500M at $10.5B valuation, 350 员工（2026-06-04）— https://www.cnbc.com/2026/06/04/database-startup-supabase-raises-500-million-10point5-billion-valuation.html
17. PocketHost（第三方商业托管，$9.99/月/实例）— https://pockethost.io/
