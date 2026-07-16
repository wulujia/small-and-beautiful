# Heptabase（詹雨安）

> 在拥挤的笔记赛道只做"深度理解"：视觉白板 + 概念卡片，服务学生/研究者/终身学习者 ｜ heptabase.com ｜ 詹雨安 Alan Chan（1997 年生，台南）+ 林昱帆（CTO）+ 吴雨川（设计）｜ 2021 ｜ 团队 10 人（2024-08）[7]｜ 订阅制笔记工具（YC W22，注：常被误记为 S21，官方为 Winter 2022 [1]）｜ 约 $2.4M ARR（2025-01，第三方估算）[8]，盈利 [6][7]

## 缝隙切入点

- 表面上是"又一个笔记软件"，实际定位是"学习与研究"：优化"吸收信息 → 深度理解 → 产出"的完整流程，而不是收集和存储笔记 [13]。官方愿景一句话："创造一个任何人都能对任何事物建立深度理解的世界" [10]。
- 方法论内核是"视觉原子化"：把学到的概念拆成原子卡片，再在无限白板上摆放、连线、重组——"要通过视觉思考对一个主题建立深度理解，你需要先把学到的概念原子化" [5]。
- 缝隙的来源是个人痛点 + 思想史：詹雨安从台大休学后自学多学科，用 Evernote/Notion 管理读书笔记时发现工具断层；研读 Engelbart 1960 年代《Augmenting Human Intellect》后发现 Notion 本质上在实现上世纪的 OHS 规格，于是自问"为什么要实现一个 20 世纪末的旧规格？"——他要做 21 世纪版的思考工具 [5]。
- 辍学路径：台南一中科学班，物理奥赛备取国手保送台大物理系、双主修数学，19 岁（大二上）休学，理由是"大学把一切都决定好了，很多课程最终沦为'需要学它'的范畴"；退伍后入读实验性大学 Minerva，读约一年再次休学创业 [2][3][4]。他自述并非反传统，而是"目标导向"：15-20 岁间评估传统教育是否有助于达成目标，结论是阻碍，于是走自学路线 [13]。

## 时机

- 2021 年 5 月开始开发（当时叫 Project Meta）[8][6]，正值 tools-for-thought 热潮：Roam/Obsidian 带火双链笔记、Notion 高速增长——赛道拥挤但全部在"记录/组织"层竞争，"帮个人在白板上思考"是空位 [5][10]。
- 2021 年 10 月发表长文《My Vision: Heptabase》，指出当时工具的共同缺陷："我在不停切换工具，一个想法的上下文散落在不同工具里……一个想法如果记不起背后的上下文，就失去了大部分意义" [10]。
- 2022 年 1 月进 YC W22，是"目前唯一以台湾（公司主体）名义进入 YC 的团队"，种子轮共募 $1.7M（YC、Kleiner Perkins、HOF Capital、Moving Capital 等）[1][3][4]。

## 差异化

- 与 Notion/Obsidian 的分野：Heptabase 强调"简单性"和"流畅性"，打开软件即进入思考状态；白板给出接近实体白板的自由度 [13]。詹雨安 2023 年专门写过《Heptabase vs Notion vs Obsidian》从工作流角度划界 [11]。
- 架构差异化："meta-app"架构——不做插件系统也不做 all-in-one，而是让白板、日志、标签等多个"元应用"共享同一套卡片原语，解决跨场景互操作而不增加复杂度 [5]。
- 路线图差异化：按"知识生命周期"五阶段（探索→收集→思考→创造→分享）逐年推进：2021-2022 只做"思考"，2023 做"收集/创造"，之后才做"分享/探索"——先让个人学会独立思考，再做协作 [5][12]。
- 奖项佐证定位成立：Product Hunt 2023 Golden Kitty 个人生产力类奖 [17]；詹雨安以 26 岁入选 Forbes 亚洲 30 Under 30（2024）[3]。

## 第一批用户/冷启动

- 冷启动靠公开写长愿景文：2020 年 6 月还在读书时就发表《My Vision: The Context》，定下三个时间尺度的目标（短期把人类智识进步加速到理论极限）[14]；2021 年 Project Meta 阶段即有 waitlist，早期用户看了愿景文排队进来 [6][10]。
- 节奏：8 个月封闭 Alpha（Discord 内测）→ 18 个月公开 Beta、迭代 300+ 版本，前后 26 个月才到 1.0（2023-08）[8][11]。
- 执行风格（詹雨安原话）："我们不害怕推出很破的产品、也不害怕被用户讨厌。我们就是直接发布了再说，用户抱怨了，我们就继续迭代。" [4]
- 到 2023 年 10 月：1.2 万+ 用户、遍布 100+ 国家，其中 1 万+ 付费，营销费用为零，全靠口碑 [6]。

## 收入与定价

- 无免费版，只有 7 天试用；上线时定价 $11.99/月（月付）或 $8.99/月（年付）[6][8]。2026 年起分层加入 AI credits：Pro $8.99、Premium $17.99、Premium+ $53.99（年付价，年付省 25%）[15]。
- 营收轨迹：2022 年初对外说的目标是"近程 ARR 10 万美元，一年半后 ARR 100 万美元" [4]；两年内达到 7 位数 ARR [8]；2023 年自述年增长 3 倍以上 [13]；第三方估算 2024 年营收 $1.2M [9]、2025 年 1 月约 $200K/月（$2.4M/年）[8]、2026 年约 $7M ARR（估算，未经官方确认）[16]。
- 关键事实：$1.7M 种子轮资金一直没花，靠产品收入维持运营、持续盈利 [6][13]。

## 内容与增长

- 增长引擎是创始人长文：《My Vision》系列（The Context 2020-06、A New City、Heptabase 2021-10、The Roadmap 2023-05）既是产品哲学也是获客内容 [10][12][14]；方法论文章（《The Best Way to Acquire Knowledge from Readings》2023、《The Best Way to Use AI for Learning》2025-09）每篇都兼作内容营销 [11][18]。
- 早期（2021-2023）在 Discord/Telegram 的笔记爱好者社群做有机渗透；产品打磨后口碑成为第一增长来源；2023 年底上线联盟计划（affiliate），贡献约 10% 收入 [8]。
- 到 1 万+ 付费用户时营销支出为零 [6]。

## 社区

- Discord 是产品社区中枢：早期内测、支持、反馈都在里面 [6][8]；另维护 Public Wiki（公开路线图、changelog、愿景文档）和定期 AMA（2023 Reddit、2024-08 Wiki）[7][12]。
- 最硬核的社区动作：全部员工都从用户里招——"所有员工均来自现有用户群" [6]。

## 留存

- 2022 年 1 月订阅的用户 cohort，20 个月后仍有 70%+ 留存（2023-10 AMA 披露）[6]——对订阅制个人工具属顶级水平，是"深度理解"定位成立的最强证据。

## 转型

- 不是转型而是按十年路线图推进 + AI 叠加：2023-08 发布 1.0 并公布 2.0 计划 [11]；2025 年起把 AI 深度融入学习/研究工作流（官网标语已改为"Master anything you learn. Do your best research with AI"），2026 年定价直接按 AI credits 分层 [15][18]。詹雨安的判断：AI 时代人类更需要建立深度理解的知识库，而非被动接受答案 [18]。

## 如何保持小

- 团队从 3 位共同创办人 + 3 名员工（2023-10）[6]，到 2024-08 扩到 10 人 [7]，全程 fully remote [6]。
- 扩张的两条硬标准：① 支撑当前用户量和下一阶段开发的真实业务需要；② 经常性收入足以在扩张后仍保持盈利 [7]。
- 詹雨安原话："创业公司最大的错误之一就是过早扩张团队，这会迫使创始人把精力放在管理和内部沟通上，而不是产品创新上。"以及面对竞争对手："我根本不在乎竞争对手有多少人。" [7]
- 不烧 VC 的钱：追求"盈利性增长率"而非"不惜代价的增长"，$1.7M 融资至今未动，以此保住"对公司方向的完全控制权"，并称希望尽可能长地维持这个状态 [6][7][13]。

## 开放问题（值得当面问创始人的）

1. 2021 年入场时 Notion/Roam/Obsidian 已经很热，你当时内部最怕的死法是什么？如果 Notion 第二年就做白板，你的应对预案是什么？
2. 20 个月 70% 留存的代价是什么——为了守住"深度理解"定位，你拒绝过哪些明显能带来短期增长的功能或用户群？
3. $1.7M 一直没花：AI 浪潮起来、对手大规模融资时，有没有哪个时刻你差点决定花掉它？那笔账当时是怎么算的？
4. "只从用户里招人"这条规则有没有失败或差点失败的案例？团队从 6 到 10 人之后，哪个环节最先感觉到"小"的极限？
5. 《My Vision》写在产品之前，五年过去，愿景里哪一部分你现在认为是错的、已经放弃了？

## 来源

1. YC 公司页（批次 W22、团队 10 人、投资方）：https://www.ycombinator.com/companies/heptabase
2. 维基百科·詹雨安（生平、两次休学）：https://zh.wikipedia.org/zh-tw/%E8%A9%B9%E9%9B%A8%E5%AE%89
3. 远见杂志《他26岁高中学历，如何靠Heptabase笔记软体登青年富比世？》：https://www.gvm.com.tw/article/109682
4. Sunrise 旭时报《台湾团队 Heptabase 如何获得矽谷第一加速器的青睐？》：https://sunrisemedium.com/p/120/heptabase-joins-y-combinator
5. Ness Labs 专访 Alan Chan：https://nesslabs.com/heptabase-featured-tool
6. Reddit AMA（2023-10，BestofAMA 存档）：https://bestofama.com/amas/17colc2
7. Heptabase Public Wiki AMA 2024-08：https://wiki.heptabase.com/ama-2024-08
8. Starter Story：How This Founder Bootstrapped a Visual Note-Taking Tool to $200K/Month：https://www.starterstory.com/heptabase-breakdown
9. GetLatka（2024 营收/人数估算）：https://getlatka.com/companies/heptabase.com
10. 詹雨安《My Vision: Heptabase》（2021-10）：https://medium.com/sheracaolity/my-vision-project-meta-e0bedd1467b2
11. 詹雨安 Medium 主页（Heptabase 1.0、对比文、方法论文章列表）：https://alanchan1209.medium.com/
12. 詹雨安《My Vision: The Roadmap》（2023-05）：https://medium.com/heptabase/my-vision-the-roadmap-d2fbf92fdf97
13. 阅读前哨站专访詹雨安：https://readingoutpost.com/heptabase-alan/
14. 詹雨安《My Vision: The Context》（2020-06）：https://medium.com/heptabase/my-vision-the-context-c73e29981685
15. Heptabase 定价页（2026-07 抓取）：https://heptabase.com/pricing
16. Fueler 估算（2026，约 $7M ARR，未经官方确认）：https://fueler.io/blog/heptabase-usage-revenue-valuation-growth-statistics
17. Product Hunt Golden Kitty 2023 获奖名单：https://www.producthunt.com/golden-kitty-awards/hall-of-fame?year=2023
18. 詹雨安《The Best Way to Use AI for Learning》（2025-09）：https://medium.com/heptabase/the-best-way-to-use-ai-for-learning-762c3467bdf1
