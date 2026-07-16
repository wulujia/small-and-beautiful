# Datasette / Simon Willison（simonwillison.net）

> 开源数据探索工具 + 全球最有影响力的 AI 独立博客之一，"一个人的研究实验室" ｜ datasette.io / datasette.cloud / simonwillison.net ｜ Simon Willison（英国人，居美国）｜ Datasette 2017 年至今，博客 2002 年至今 ｜ 1 人（+ 一位由 Fly.io 赞助的协作者）｜ solo / 开源优先 / 靠声誉而非产品变现 ｜ 收入结构：Eventbrite 卖公司的积蓄 + 咨询 + 681 个 GitHub Sponsors + 2026 年起博客横幅赞助，Datasette 本身 9 年未盈利 [5][7][1]

## 缝隙切入点

- Datasette 的缝隙是"数据新闻的贫富差距"：纽约时报、华盛顿邮报有全职数据工程师团队，小新闻编辑室没有。他 2019 年申请斯坦福 JSK 新闻学者项目时的提案就是这个——用开源工具把大报级的数据报道能力交给雇不起工程师的小编辑室 [4][19]。
- 技术切口极小而精确：把任何 SQLite 数据库一键变成可浏览、可任意 SQL 查询的网站和 JSON API。2017 年 11 月首发时的核心洞察是"只读"——去掉写操作后，SQLite 的并发短板消失，"It lets us use SQLite in production in high traffic scenarios"，数据不可变还能把 HTTP 缓存设成一年 [3]。
- 更深一层的缝隙是他本人的位置：AI 时代几乎所有有分量的评论者都隶属于大厂、实验室或学术机构，他是极少数完全独立、不拿任何一方工资的技术声音——这个"无立场位置"本身成了稀缺资产 [2]。
- 他对 Datasette 的承诺是以十年计的："I realized that Datasette is the first project of my entire career where if I was still working on it in 15 years time I wouldn't feel bored yet... I want to work on it for decades"（2023 年他在 HN 的自述）[20]。

## 时机

- 路径上的每一站都踩在浪头：2003–2004 年在堪萨斯州 Lawrence Journal-World 报社实习（本科 gap year），和 Adrian Holovaty 等人一起创造了 Django（2005 年开源）；2005 年入 Yahoo，2008 年任卫报软件架构师；2010 年底和妻子 Natalie Downe 创办会议日历网站 Lanyrd，2011 年初进 YC，2013 年 9 月被 Eventbrite 收购，随后在 Eventbrite 做了六年工程总监 [2]。
- 2017 年做 Datasette 踩中 serverless：数据只读 + SQLite 单文件，正好能塞进当时兴起的按需容器托管，发布成本趋近于零 [3]。
- 最大的一次时机是被动的：ChatGPT 时代来临时，他已经写了 20 年博客、有现成的读者和信任存量。2022 年 9 月（ChatGPT 发布前两个月）他给一类新漏洞命名"prompt injection"（类比 SQL injection），被全球安全界直接采纳为标准术语 [2][21]；2025 年 6 月又造了"lethal trifecta"（AI agent 三要素致命组合）[2]。一个独立博主成了 AI 安全领域的命名者。

## 差异化

- 无聊技术 + 20 年如一日的写作，是他全部的护城河。技术上死守 SQLite 和 Python（"boring technology"），连 AI 辅助编程他都建议选训练数据里多的老牌库 [11]。
- 独立性是产品级卖点：博客 About 页明确写着"写任何主题都不收钱"、赞助商对内容零影响力 [1]。结果是 GPT-5 发布前，OpenAI 给的预览权限没有给传统媒体，而是给了他这样的独立博主——他提前两周拿到模型，发布日当天的评测文章上了 Techmeme 头条 [16]。
- 他的"pelican riding a bicycle"基准测试（让每个新模型画"骑自行车的鹈鹕"SVG，2024 年底开始）从个人玩笑变成行业默认基准，2025 年 Google I/O 主题演讲里专门放了一只骑车的鹈鹕向他致意 [15]。
- 一人多线的工作方式本身是差异化：同时维护 Datasette、LLM CLI（GitHub 上分别约 11.3K 和 12.2K stars）、sqlite-utils 及几百个小项目 [7]，每天把实验过程原样写出来。别人发论文，他发当天可复现的博客。

## 第一批用户/冷启动

- Datasette 的发布渠道就是他的博客：2017 年首发文用 FiveThirtyEight 的公开数据集现场演示"任何人都能对数据跑任意 SQL" [3]。目标用户（数据记者）和他的读者高度重合，没有独立的冷启动动作。
- Datasette Cloud（2023 年 8 月上线的 SaaS）延续同一路径：先向新闻编辑室开放预览；2025 年 4 月推出"Datasette for Newsrooms"套件，非营利新闻编辑室免费用一年，其他人两个月试用 [8][9]。

## 收入与定价

- 真实的财务结构（他在访谈里坦白过）：Lanyrd 卖给 Eventbrite + 六年总监工资攒下"substantial runway"，但没到财务自由；靠临时咨询和培训补现金流，"等 Datasette 产生收入" [5]。
- 目标模式是 WordPress：代码全部开源，靠托管服务（Datasette Cloud）赚钱；Datasette Cloud 的公开目标不只是养活自己，而是"养一个团队全职做 Datasette" [5][8]。但截至 2026 年中，Datasette Cloud 仍处早期（官网连公开定价都没有，见客户约演示）[22]，Datasette 1.0 发了 34 个 alpha 还没正式版 [23]。
- 博客的直接收入被刻意压到很低：681 个 GitHub Sponsors（$10/月档可收他的月度 LLM 摘要通讯，档位一直到 $10,000/月的企业档）[7]；偶尔挂 EthicalAds；2026 年 2 月才第一次卖博客广告位——学 Troy Hunt 的模式，按周出售一条纯文本横幅，无 JS 无 cookie [1]。写了 24 年博客，第 24 年才开始直接变现。
- 所以对"博客爆发性影响力是否带来收入"的诚实回答是：直接收入很小且是近两年才有的；真正的变现是间接的——咨询单、演讲、模型预览权限、以及让 Datasette Cloud 未来有一个自带的分发渠道 [1][5]。
- 外部输血：Fly.io 赞助了 Datasette Cloud 的部分开发，直接出钱让工程师 Alex Garcia 和他一起做（两人公开直播如何在 Fly Machines 上搭多租户 SaaS）[18]。

## 内容与增长

- 产量方法论：受 Tom Scott 十年不断更的启发，尽量每天发；单篇只花 10–15 分钟，因为写了二十几年手熟；博客自动转成 Substack 通讯，每期分发成本约两分钟，订户约 6,000（2023 年数据）[5]。
- 爆发点：2023 年 2 月他汇总 Bing AI 失控对话的文章拿到 140 万浏览，被马斯克转推，带来他人生第一次电视采访 [5]。2024 年底的年度综述《Things we learned about LLMs in 2024》让 Latent Space 直接称他"the world's top AI blogger"，为此专门做了跨台联播节目 [13]。
- 命名即增长：除了 prompt injection 和 lethal trifecta，他 2024 年 5 月起在主流圈带火"slop"（未经请求、未经审核的 AI 生成内容），纽约时报为此发了专文《First Came 'Spam.' Now, With A.I., We've Got 'Slop'》，该词 2025 年被 Merriam-Webster 和美国方言学会同时选为年度词汇 [14]。
- 他公开的 AI 辅助编程方法论本身成了高传播内容：LLM 是"你那个怪异、过度自信的实习生"[5]；核心技能是管理上下文；对生产代码要当"独裁者"，给出精确的函数签名和规格；以及铁律——"the one thing you absolutely cannot outsource to the machine is testing that the code actually works" [11]。
- 他对 AI 提效的表述比"更快"更深一层："This doesn't just make me more productive: it lowers my bar for when a project is worth investing time in at all"——以前不值得做的项目现在值得做了，这是他几百个小工具井喷的原因 [12]。

## 社区

- Datasette 走插件生态：他的原话是"The great thing about a plugin ecosystem is that it removes the need for a gatekeeper"——别人扩展功能不需要经过他，核心保持小 [6]。LLM CLI 同样靠插件接入各家模型。
- 他 2022 年起任 Python 软件基金会董事，在 Python 社区的公信力反哺项目 [2]。

## 转型

- 他的路径不是连续创业，而是"换赛道不换方法"：Django（框架）→ Yahoo/卫报（平台与媒体）→ Lanyrd（创业公司）→ Eventbrite（管理者）→ JSK（学者）→ 独立开源人。促成最后一跳的是 JSK 那一年的自由："once you've done that, it's very difficult to go back" [5][4]。
- 2022 年底的转向没有换产品，而是换了"报道口"：博客重心从数据新闻工具转向 LLM 实测，2023 年 4 月发布 LLM 命令行工具，把 AI 变成 Datasette 生态的一部分而不是另起炉灶 [2]。代价是 Datasette 主线明显变慢（1.0 拖了九年），收益是影响力上了一个数量级——这笔账他自己似乎认为划算。

## 如何保持小

- 一个人维护 185 个 PyPI 包（2022 年 DjangoCon 演讲自述）的系统方法：每次提交必须四件套——实现 + 测试 + 文档 + 关联 issue（"the perfect commit"）；所有思考过程写进 GitHub issue（"commitment-free"的文档，不需要维护）；文档必须和代码同仓库，并用"documentation unit tests"强制代码功能在文档里出现 [10]。
- 对抗开源愧疚的规则："If your project is tested and documented, you have nothing to feel guilty about"；以及刻意不做带用户账号系统的项目——那会把副业变成无薪的运维工作 [10]。
- 用截止日期替代管理层：conference-driven development，公开报名演讲，用讲台日期倒逼项目发布 [5]。
- 值得注意的反面：他其实不想永远一个人——Datasette Cloud 的目标明确写着要养一个团队 [8]。九年过去团队仍是 1 人 + 一位赞助来的协作者 [18]，"保持小"对他一半是哲学，一半是商业化没跑通的结果。

## 开放问题（值得当面问本人的）

1. Datasette 1.0 发了 34 个 alpha、拖了九年 [23]，而你说要做几十年 [20]——"永远可以再等等"的开源完美主义，是不是恰好成了 Datasette Cloud 收不到钱的原因？什么条件下你会强制自己发 1.0？
2. 你是全球读者最多的 AI 独立博客之一，但直接变现只有一条按周卖的文本横幅和 $10/月的赞助者通讯 [1][7]。如果开付费订阅，几千订户大概率立刻到手——你在保护的到底是什么？这个"不变现溢价"你算过值多少吗？
3. Datasette Cloud 押注的新闻编辑室是全行业最没钱、且在持续萎缩的客户群 [9]。WordPress 模式需要一个庞大的付费宿主市场——如果两年内新闻室这条路走不通，你换哪个客群，还是接受 Datasette 永远靠赞助活着？
4. OpenAI 们现在给你模型预览权限 [16]——access 本身就是一种报酬。你写明了"写什么都不收钱" [1]，但拿了提前两周的独家权限还能对发布方零留情吗？你给自己划的线具体在哪里？
5. 你说 AI 降低了"值得做"的门槛 [12]——但同样的能力也让任何人用一句话就能生成数据查询界面。当 LLM 可以按需现写一个 Datasette 的时候，Datasette 作为产品还剩下什么？

## 来源

1. https://simonwillison.net/about/ （2026-07 查看）
2. https://en.wikipedia.org/wiki/Simon_Willison
3. https://simonwillison.net/2017/Nov/13/datasette/ （2017-11）
4. https://simonwillison.net/2019/Sep/10/jsk-fellowship/ （2019-09）
5. https://mtlynch.io/notes/simon-willison-software-misadventures/ （Software Misadventures 播客笔记，2023）
6. https://blog.southparkcommons.com/p/simon-willison-my-career-in-side-projects-and-open-source
7. https://github.com/sponsors/simonw （2026-07 查看：681 sponsors、档位与项目 stars）
8. https://www.datasette.cloud/blog/2023/welcome/ （2023-08）
9. https://simonwillison.net/2025/Apr/24/introducing-datasette-for-newsrooms/ （2025-04）
10. https://simonwillison.net/2022/Nov/26/productivity/ （DjangoCon 2022 演讲 "Coping strategies for the serial project hoarder"）
11. https://simonwillison.net/2025/Mar/11/using-llms-for-code/ （2025-03）
12. https://simonwillison.net/2023/Mar/27/ai-enhanced-development/ （2023-03）
13. https://www.latent.space/p/2024-simonw （2024-12，Latent Space × TechMeme Ride Home 联播）
14. https://en.wikipedia.org/wiki/AI_slop
15. https://fedi.simonwillison.net/@simon/114541794883433725 （2025-05，Google I/O 出现鹈鹕）
16. https://x.com/simonw/status/1953512493986591195 （2025-08，GPT-5 两周预览权限自述）
17. https://newsletter.pragmaticengineer.com/p/ai-tools-for-software-engineers-simon-willison （2024）
18. https://datasette.substack.com/p/datasette-cloud-and-the-datasette （Fly.io 赞助 Alex Garcia）
19. https://jsk.stanford.edu/news/jsk-journalism-fellowships-names-class-2019-2020 （2019）
20. https://news.ycombinator.com/item?id=37197073 （2023-08，本人 HN 留言）
21. https://simonwillison.net/series/prompt-injection/ （2022-09 起系列）
22. https://www.datasette.cloud/ （2026-07 查看，无公开定价）
23. https://letsdatascience.com/news/datasette-releases-alpha-build-10a33-for-data-publishing-d2f00432 （2026-06，1.0a33/a34）
