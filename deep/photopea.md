# Photopea（Ivan Kutskir）

> 在浏览器里复刻 Photoshop：打开 photopea.com 就是完整图像编辑器，无需安装、文件不出本机 ｜ photopea.com ｜ Ivan Kutskir（生于乌克兰西部，2002 年随家人移居捷克，布拉格）｜ 2012 年动念、2013-09-14 发布 0.1 ｜ 1 人，至今 13 年 ｜ 免费 + 广告（约 90%）+ Premium/自托管授权 ｜ 2019 约 $25 万 → 2021 约 $100 万 → 2024 $300 万+/年

## 缝隙切入点

起点小得惊人：大学期间（布拉格查理大学计算机科学，2009-2016 [3][11]）他想试试能不能在浏览器里解析 PSD 文件，先做了个"打开 PSD、把图层分别下载下来"的小工具 [4]。没有商业计划——"我从没打算开公司，我只是想做有用的软件"[5]。产品几乎立刻就发布了："我发布 Photopea 时，它只有今天功能的 1%"[5]，然后"很自然地，做完一个功能再做下一个，帮完一个用户再帮下一个，不知道接下来会怎样，也没有目标"[4]。

定位是他自己说得最准："它免费，这点不像其他高级软件；它高级，这点不像其他免费软件"[11]。浏览器天然解决了另一个缝隙："图像编辑器都是原生应用，小众操作系统上很难找到好用的编辑器"[11]——Linux、Chromebook、公司里没有安装权限的电脑，都是 Photoshop 触不到的地方。

## 时机

2013 年 5 月，Adobe 宣布 Photoshop 停售买断版、全面转向 Creative Cloud 订阅制 [17]；四个月后 Photopea 0.1 上线 [7]。这不是有意为之的狙击，但结构性机会从此持续变大：全世界"不想订阅 Adobe 却需要开 PSD"的人，成了一个逐年膨胀、且 Adobe 主动放弃的池子。浏览器和 JavaScript 引擎的性能在同一时期成熟到足以跑重型图像运算，让"网页版 Photoshop"从笑话变成可行工程。

## 差异化：工程本身是护城河

- **一个人手写整个 Photoshop 级编辑器**。纯 JavaScript/HTML/CSS，不用任何框架："我自己写我的 JavaScript、HTML 和 CSS"[1][2]。代码量并非坊间传说的"百万行"——他每次发版都在博客公布精确行数：v5.0（2021-01）98,893 行，v5.6（2024-04）138,541 行 [6]。约 14 万行代码扛住了 Photoshop 约 90% 的功能 [1]，密度是护城河本身。
- **投入是可计算的**：2020 年他估算已写了"大概 15,000 到 20,000 小时"[1]——按 7 年折算，相当于每天 6-8 小时、全年无休。
- **纯客户端架构**：所有运算在用户设备上完成，服务器只跑账号和 PeaDrive 网盘的少量 PHP [5]。文件不上传，隐私是卖点，更是成本结构——年运营成本约 $620（域名 ~$20 + 托管 ~$600）[5]，早年只要 $66 [4]。一个千万级用户的产品，服务器开销约等于一部手机。
- **格式转换是钩子**：能把 PDF、SVG、Sketch、XD、Figma 转成带图层的 PSD [1]，"打不开的文件扔给 Photopea"成为设计圈口口相传的场景。
- 底层图像能力（PNG/TIFF 解码、字体解析等）他以独立开源库形式发布，编辑器本体闭源 [3]，GitHub 仓库不放源码、只当 issue 跟踪器用 [19]。

## 第一批用户/冷启动：AMA 是增长引擎

- 最早把网站提交到 Google 的实验目录，每天只有 10-20 个访客 [5]。早期他到处"刷屏"："我曾经在整个互联网上'骚扰式'宣传 Photopea……我 90% 的帖子和评论都被当成自我推销删掉了"[4]。
- 真正的放大器是 Reddit AMA。2018 年 10 月，网站月访问量创下 150 万新高，他做了第一次 AMA，拿到 5 万+ 赞、2200 条评论，冲上 r/IAmA 头部 [9][10]。九个月后流量翻倍到 300 万，第二次 AMA（2019-07）再次爆掉 [9][18]。2020-08 第三次 AMA 时标题已是"被 700 万人使用"[1]。2021-04 又在 Hacker News 做了一场 AMA [2]。此后 AMA 成为固定动作，最近一次在 2026-03-18 [12]。
- AMA 之外全靠自来水：YouTuber 和博主的主动测评带来持续流量 [4]。广告预算始终为零，增长成本就是他本人反复出现在评论区。
- 流量轨迹：2017 年开始变现时日访客 5,000 [5] → 2018-10 月访问 150 万 [9] → 2019-07 月访问 300 万 [9] → 2020-08 月用户 700 万 [1] → 2024 年月访客 1200 万、日活约 100 万 [5][9]。

## 收入与定价：用广告对抗订阅制

Adobe 靠订阅收钱，Photopea 反着来：软件全功能免费，靠用户停留时间卖广告。

- **收入轨迹（全部来自他本人公开）**：2013-2017 年约 4 年零收入，2017 年挂上广告 [5]；2019 年全年约 $25 万 [1]（这就是"AMA 说年入数十万美元"的原始出处，2020-08 AMA 原话"around $250,000"，并称希望当年翻 2-4 倍 [1]）；2021-04 在 HN 亲口确认"过去 12 个月我赚了差不多 100 万美元，90% 来自广告"[2]；2021-22 年前后月广告收入约 $10 万、月访问 1000 万次、月使用时长 150 万小时 [4]；2024 年到 $300 万+/年、约 $25 万/月 [5]。
- **单位经济学他算得很细**："用户每在 Photopea 里待一小时，我赚大约 5 美分"[1]（后来说 6 美分 [4]）。收入 = 使用时长 x 单价，所以他优化的从来是"值得停留的工具"，不是转化漏斗。
- **Premium 一直是配角**：2020 年是"付 $10 免广告三个月"，付费者仅数百人、约占用户 0.01% [1]；后来约 1500 人、$3/月 [8]；现在 Premium 含 5GB PeaDrive 网盘和每月 3000 点 AI 额度 [7]。另有自托管授权 $500-2000/月 [7]——但他 2022 年公开困惑："我有数百万用户，却没有企业客户用它（付费授权）"[16]。
- **广告模式的代价**：他估算广告拦截器让他损失 10-40% 的潜在收入 [1]。2023-10 他曾强硬反击——检测到拦截器就不让新建/打开文件，在 HN 引发争议，uBlock Origin 社区数小时内就更新滤镜绕过了封锁 [14]。免费产品的用户不欠你广告曝光，这场小战争他没打赢。

## 拒绝出售与融资

- 2020 年他确认："Photopea 至今没有被任何人收购，尽管我收到过好几份投资报价"[1]——全部拒绝。
- 他把这条写成了给独立开发者的公开建议："不要卖掉你的作品，哪怕有人出的钱是你这辈子赚过的钱的 10 倍、100 倍甚至 1000 倍"[4]。
- 对"去大厂"的经典回答（2021 HN AMA）："当你做自己的项目，你永远不知道它能不能做到年入 25 万美元。但当你被雇佣，你可以非常确定，你永远不会赚到超过 25 万美元一年。"[2]

## 社区

- r/photopea 建于 2016 年，约 2.5 万成员，他本人每天在里面回答问题 [9]。
- GitHub 仓库（photopea/photopea）没有一行源码，纯粹是公开 bug tracker，issue 数以千计 [19]。
- 反馈闭环极短：AMA 里用户提的功能（如 Color to Alpha）会直接出现在后续版本里 [2]。社区不是营销渠道，是他的需求管理系统和 QA 团队。

## AI 时代：追赶与被追赶

- **追赶**：2023-24 年加入 AI 功能——一键抠背景（Remove BG）、生成式替换（Magic Replace）、文生图，底层不是自研模型，而是与 Dezgo API 合作 [7][13]。免费用户每天 1 次，Premium 每月 3000 点，用完可以填自己的 Dezgo API key 继续用 [7][13]。单人产品接 AI 的务实姿势：买运力，不烧钱训练。有趣的反向信号：有用户在 GitHub 上要求"给个开关，把所有生成式 AI 功能关掉"[20]。
- **被追赶**：2025-10-30，Canva 宣布 Affinity（Designer/Photo/Publisher 合并版）"永久免费"，只靠 Canva AI 订阅变现 [15]。Photopea 立身之本——"免费而专业"——从稀缺品变成巨头的补贴品。Adobe 有订阅制的包袱，Canva 没有。
- **信号混杂**：官方博客自 2024-04 的 v5.6 之后停更 [6]，但 2026-03 他仍在办新一轮 AMA [12]，产品持续在线。一人公司的"沉默"与"死亡"从外部难以区分，这本身就是单人模式的观察成本。

## 如何保持小

- **13 年，1 个人，0 员工，0 办公室** [5][9]。没有融资、没有收购、没有团队——上面每一个"没有"都是他拒绝出来的 [1][4]。
- **架构决定组织**：纯客户端运行让他没有运维、没有 SRE、没有服务器账单焦虑 [5]，广告变现让他没有销售、没有客服 KPI——"用户没付钱，不爽可以直接走，投诉都很少"[8]。技术选型和商业模式共同把"必须招人的理由"逐个消灭。
- **节奏**：常年保持约每月一次发版 [5]，每个大版本在博客公布功能清单和代码行数 [6]，像跑马拉松一样匀速。
- **想大过，没大成**：2020-21 年他多次说想招人、想做视频编辑器和矢量编辑器 [1][4]，到 2026 年这些都没发生——Photopea 还是一个人 [5][12]。

## 开放问题（值得当面问创始人的）

1. 90% 收入靠广告，而广告拦截、AI 浏览器和"AI 代理替人干活"都在侵蚀"人眼看页面"这个前提。2023 年封锁拦截器用户那次失败的反击之后，你对广告模式的十年预期是什么？Premium 十年都没做起来（0.01% 付费率），是不想还是不能？
2. Affinity 2025 年被 Canva 变成"永久免费"，你的定位口号"免费得像业余软件、强大得像专业软件"第一次被巨头正面复制。你的下一道护城河是什么——格式兼容、加载速度，还是"用户就是懒得换"？
3. 你拒绝过的报价里最大的一笔是多少？有没有哪个深夜后悔过？"不要卖，哪怕 1000 倍"这句话，你现在还会原样送给别的独立开发者吗？
4. 2020 年起你反复说想招人、做视频编辑器，六年过去还是一个人。是发现了"一人公司"的最优性，还是被 14 万行只有你能维护的代码锁死了？如果明天你不能写代码，Photopea 的寿命还剩多久？
5. 你从 15,000-20,000 小时的手写 JS 里得到的最大工程教训是什么？如果 2013 年就有今天的 AI 编程工具，Photopea 会更快做成，还是根本轮不到你做——因为"单人复刻 Photoshop"的稀缺性消失了？

## 来源

1. Reddit AMA（2020-08-12）：I made a free alternative to Photoshop, that is used by 7 million people（BestofAMA 存档）— https://bestofama.com/amas/i8j5te
2. Hacker News AMA：Ivan Kutskir, creator of Photopea（2021-04-11）— https://news.ycombinator.com/item?id=26768550
3. Hacker News 讨论："…and created by 1 person"（2021-10）— https://news.ycombinator.com/item?id=29001723
4. Failory 访谈：Building a Photo Editor and Making $100k/mo as a Solo Founder — https://www.failory.com/interview/photopea
5. Indie Hackers：Making $3M+ per year with a free product（2025-05-09）— https://www.indiehackers.com/post/tech/making-3m-per-year-with-a-free-product-axW4u1vB6C8f91Z3Lxu5
6. Photopea Blog（版本发布与代码行数）— https://blog.photopea.com/
7. Wikipedia：Photopea — https://en.wikipedia.org/wiki/Photopea
8. Bootstrappers：This Founder's Legion of Reddit Fans… $1 Million a Year — https://bootstrappers.com/this-founders-legion-of-reddit-fans-helped-him-build-a-free-alternative-to-photoshop-that-brings-in-1-million-a-year/
9. Indie Hackers：How Reddit AMA Earned Photopea 12M Monthly Users — https://www.indiehackers.com/post/how-reddit-ama-earned-photopea-12m-monthly-users-7c66c1d9ad
10. Hacker News：Reddit AMA on Photopea, used by 1.5M people（2018-11-07）— https://news.ycombinator.com/item?id=18397380
11. New Rationalist 访谈：Ivan Kutskir - Creator of Photo Pea — https://newrationalist.com/ivan-kutskir-creator-of-photo-pea/
12. Photopea 官网：AMA 预告页（2026-03-18，r/IAmA）— https://www.photopea.com/reddit.html
13. Photopea 教程：Get Unlimited AI inside Photopea（2024-02-20）— https://www.photopea.com/tuts/get-unlimited-ai-inside-photopea/
14. Hacker News：Tell HN: Photopea refuses to create or open files if you have an ad blocker（2023-10-23）— https://news.ycombinator.com/item?id=37980680
15. Canva Newsroom：Why we made Affinity free, and how we'll keep it that way（2025-10-30）— https://www.canva.com/newsroom/news/affinity-free/
16. Hacker News：Reddit Photopea founder – I have millions of users, but no businesses use it（2022-02-16）— https://news.ycombinator.com/item?id=30357839
17. Wikipedia：Adobe Creative Cloud（2013-05 转订阅制）— https://en.wikipedia.org/wiki/Adobe_Creative_Cloud
18. X @photopeacom：第二次 Reddit AMA 预告（2019-07）— https://x.com/photopeacom/status/1146502965597003779
19. GitHub：photopea/photopea（无源码，仅 issue 跟踪）— https://github.com/photopea/photopea
20. GitHub issue #8291：Feature request: option to disable all generative ai features — https://github.com/photopea/photopea/issues/8291
