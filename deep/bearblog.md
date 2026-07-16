# Bear Blog（Herman Martinus）

> 把博客做回 3KB 纯文本——无 JS、无追踪、无广告，把"这个软件 50 年后还在"当成核心卖点 ｜ bearblog.dev ｜ Herman Martinus ｜ 2020 年，南非开普敦 ｜ 1 人 ｜ newsletter·内容工具 / pure-bootstrap / solo-creator ｜ ~$5K/月、月增 10%（约 2023 自述）[17]；2025 年口径改为"覆盖开销 + 让我过上体面生活"[12][15]

## 缝隙切入点

2020 年疫情期间，Herman 经历了一场他自称的"存在主义危机"，想重新开始写作，把 WordPress、Ghost、Jekyll、Hugo、静态 HTML 全试了一遍，结论是全都"无限可定制、无限臃肿"（infinite customizability and bloat）——他要的只是"把文字放上互联网的最快方式"[18][22][23]。于是用 Django 花一个周末搭了个能在手机上发文的极简原型，这就是 Bear [1][17]。

缝隙的本质是**反潮流**：在网页平均体积以 MB 计、到处是 cookie 弹窗和订阅弹层的年代，Bear 的页面约 2.7KB，"No trackers, no javascript, no stylesheets. Just your words."，口号是"Shun the bloat of the current web, embrace the bear necessities"[19]。他后来在 HN 上说，GDPR 弹窗和强推 newsletter 的套路"正是我做 Bear 想逃离的东西"[10]。

方法论来源很特别：不是精益创业，而是游戏设计——他把《ICO》《旺达与巨像》的"Design by Subtraction"（减法设计）当作 Bear 的底层哲学，"Something is perfect when nothing else can be removed"；每收到功能请求，第一个问题是"这件事能不能在现有系统的约束内完成？"[18]

## 差异化

一句话：**别的平台卖功能，Bear 卖克制和寿命**。

- 技术姿态即产品姿态：服务端渲染、无 JS 框架、页面 2.5-5KB；刻意选"无聊的老技术"（Django/Python + Heroku），理由是久经考验、社区大、可迁移到几乎任何基础设施——与之对照的是依赖 Firebase 这类随时可能被 Google 改动或砍掉的方案 [5][6]。
- 把"永续"写成首页卖点："Built to last forever"[19]。2022 年他专门写了 Building Software to Last Forever：Bear 盈利且开销很小，拒绝融资以免"搅浑产品方向"，重心是"把现有功能打磨到完美，而不是堆新功能或推变现"[5]。
- 他对融资的态度（播客原话）："I'm not really beholden to anyone else to push out features."[6]
- 早在 2020 年 11 月他就写过 MVP 批判文：产品应该"slick"（顺滑）而不只是"viable"（能用）[23 附档：herman.bearblog.dev/mvp-vs-slc/]。

## 第一批用户/冷启动

教科书级的 HN 冷启动，而且是无心插柳：原型上线 4-5 天后，他把它发上 Hacker News 求反馈，20 分钟内冲上首页，挂了约 24 小时——峰值 24 小时约 5 万独立访客、约 1,200 个新账号 [1][18]。基础设施连环爆炸：邮件服务超额、DNS 记录 130 条手动更新到才发现有上限、数据库赶上计划维护弹出上百个无法复现的报错，"我被同时发生的一切淹没，几乎没睡"[1]。但他最得意的结论是：一台 **$7/月的 Heroku 服务器**扛住了 HN Hug——"优化良好的老技术就够了"[1]。

此后没有再做过任何传统营销。最大的获客渠道是他自己的博客（herman.bearblog.dev，本身就跑在 Bear 上，也是平台的示例站）：写运营平台的真实故事 → 上 HN → 带来新用户 → 新用户产生内容 → 更多人知道 Bear，自我强化 [17]。

## 收入与定价

- 模式演进：先是 sponsorware（赞助者才能绑自定义域名，抵服务器成本）[3]，后固化为 freemium：免费版无限写作，付费解锁自定义域名、媒体上传、统计分析、邮件订阅收集、进入发现页等，$5/月或 $49/年，另有 $189 终身版；按购买力平价（PPP）做区域定价 [10][21][*]。
- 公开数字线：2023-03 播客称订阅收入"已超过我上班时的工资"[6]；BoringCashCow 访谈（约 2023）：约 $5,000/月，月增约 10%，"我能给自己开一份普通开发者的薪水"[17]；2025 年起不再公布具体数字，口径变为"项目覆盖自身开销，并给我足够的报酬过上体面的生活"[12][15]。
- 平台规模：2022-05 约 5,500 个博客 [3] → 2023-03 约 15,000 个活跃博客 [6] → 2025 年初一次"注册量陡增"逼他上了自动扩容 [23]。
- 他很清楚免费平台的残酷比例："99.9% 的用户不会为免费服务付一分钱"[3]。
- **多产品组合分散风险**：Bear 之外他还经营 JustSketchMe（给插画师的人体姿势参考工具，与 Bear 并行多年）和一堆小工具（JustCORS、Bearlytics 自托管统计、PPP 定价 API、Rent v Buy 等）[3][20]。早在 2020 年 12 月（Bear 还没怎么赚钱时）他就写道，产品收入约 10 个月前已越过"覆盖本地生活成本"的门槛 [2]——先有饭吃，再谈理想，是 Bear 能"不着急变现"的底气。

## 内容与增长

增长引擎就是他的写作本身。他把每一次运营危机都写成长文：反垃圾之战、排序算法设计、许可证之争——这些文章反复登上 HN 首页，本身就是 Bear 的最佳广告 [17]。2025-09 那篇宣布改许可证的文章被阅读超过 12 万次 [14]。他的增长哲学在 2025-12 的 Grow slowly, stay small 里说透了：反对"招人、扩张、上杠杆"的默认剧本，"真正的难题是想清楚什么是'足够'"（figuring out what is "enough"），"bigger is not always better"[15]。

## 社区：反算法的发现页

Bear 的发现页（Discovery feed）是整个平台的"城市广场"，也是 Herman 花心思最多的反潮流设计——目标不是最大化停留时长，而是**故意让任何人都红不过一周**：

- 排序公式：Score = log(upvotes) + 时间项（14 天衰减因子）。对数压制热度："一篇两周前的帖子需要 10 倍于新帖的赞才能排在它前面"；即使一篇帖子有 1 万个赞，也在头部呆不满一周 [4]。约 30 个赞之后，更多的赞几乎不再起作用——专治把站外粉丝导进来刷榜的大 V [16][18]。
- 移除了信息流里的点赞按钮，"防止人们只看标题就投票"——必须点进去读完才能赞 [4]。
- 24 小时发 3 篇以上，直接踢出发现页——刷屏无效 [18]。
- 2024 年改为 opt-in（发帖需显式声明 make_discoverable），理由一句话："Defaults matter a lot"；同时警告社区规模与质量负相关，"太大就会变成 Reddit"[11]。
- 治理哲学："Curation instead of exclusion"（策展而非排斥）：给读者"隐藏某博客"的自助过滤，而他本人手动审核每一个想进发现页的博客，自称是"园丁而非守门人"[16][18]。
- 对 AI 的边界划得很清楚：AI 生成的博客会被清除（Bear 要保持"human-centric"），但**不按话题过滤**——写 AI 话题没问题，"按话题审查会破坏平台的平等性"[16][18]。

## 留存：信任本身是产品

Bear 的留存策略不是功能锁定（它甚至没什么可锁定的），而是一纸公开承诺。2025-01 的 The Bear Manifesto 立了三条 [12]：

1. "Bear won't shut down. Period."（按 10 年、20 年、50 年的尺度设计）
2. "Bear won't sell. I'm not building this to flip it to the highest bidder."（无 VC、无外部压力、无退出策略）
3. "Bear won't show ads. Your blog is your space."

配套的不是空话而是机制：完整的系统文档、多名可信开发者持有代码库权限、维护指引——"如果我以任何方式失能，平台会继续活下去"[12]。他研究过什么组织活得最久，答案是家族小生意、修道院、教育机构，而"不惜一切代价的增长最终必然导致公司解体"；他的结论是信任"不只是法律结构，而是一种社会契约"——Bear 以 PTY LTD 形式运营，用附加功能换钱、用钱养基础设施，仅此而已 [12]。早在 2022 年他就写过最坏情况下把项目移交给可信方的流程，并考虑过 Django 基金会式的非营利结构 [5]。

## 转型：从开源理想到现实防御

2025-09-01，Bear 把代码许可从 MIT 改为 Elastic 风格的 source-available（禁止把它作为托管服务提供）。直接原因：反复有人把仓库 fork 一下、改个名字就上线竞品，AI 时代做这件事"只需要输入一句'Create a fork of this repo and change its name'"。他写得很诚实："看到自己辛苦做了这么多年的东西被复制，是很疼的"——这威胁到他的生计，也让他对开源原教旨有所幻灭；但他的核心判断是：代码不是护城河，"让平台特别的是使用它的人"[13]。这篇文章读者超 12 万，HN 上约一成骂声，但他收到的邮件绝大多数是支持 [14]。顺带一提：Bear 从来不接受外部代码贡献，所有代码都是他一个人写的 [14]。

## 如何保持小：一个人跑一个平台的运维哲学

- **对抗 spam 是免费博客平台的核心运维**，他打出了两场漂亮的非对称战争：
  - **Frustration Loop（2023-09）**：检测到 spam 后不封号，而是"用最令人沮丧的方式伪造系统故障"——表单随机清空、报错"Our servers are bearly managing"、禁用粘贴、每 5-10 秒乱跳输入焦点，让 spammer 自己放弃。三个月内 spam 从新博客的约 30% 降到 5% 以下，唯一的误伤投诉来自一个推广非法赌场的用户 [8]。
  - **ChatGPT spam 战争（2023-04）**：ChatGPT 让垃圾内容变得"高质量"且无法机器识别（有职业学校开了 20 个假"个人博客"自吹，连反链都不放）。试过 AI 检测（误报太多）、试过逼付费（"会毁掉平台"），最终方案：新免费博客默认一周不可见、不进搜索索引，之后可申请人工审核或升级付费 [7]。文中留下一句名言："On the flip side, fuck spammers."[7]
- 运维负荷的真实刻度：2022 年每周花 15-20 分钟审 spam [3]；到后期每天屏蔽 100-200 个垃圾博客、花 1-2 小时做审核与支持——度假时也不停 [18]。2024 年起把 spam 审核部分外包给 Bonsai Digital 的两位帮手——这是这个"一人公司"唯一的外援 [11]。
- 个人节律是基础设施的一部分：晨间散步 + 健身房 + 日记，两个 3 小时工作块（上午块不开邮箱），下午 5 点准时收工；判断接不接一个项目的标准是"如果它成了，我愿意在它上面花掉未来几年吗？"；2019 年删光了社交媒体账号，靠一个存满用户感谢信的"Nice Emails"文件夹维持士气 [9][18]。
- 终局观早在 2020 年就写下了（My product is my garden）："My product is my garden"、"I want to make things that don't scale"、"我想在园子里踱步，与过程保持连接，并乐在其中"——达到覆盖生活成本的盈利线之后，优化的对象是质量而不是用户数 [2]。2025 年初他宣布 Bear"基本功能完备"，之后的重心从写代码转向写文章 [23]。

## 开放问题（值得当面问创始人的）

1. 收入数字在 2023 年（约 $5K/月）之后就不再公布，Manifesto 也刻意不写用户数和营收——是"数字会招来错误的期待"，还是增长放缓了？现在免费/付费比例多少？
2. $189 的终身版本质上是"预收 50 年服务费"：终身用户越多，"last forever"承诺的长期负债越重。他算过这笔账吗？终身版占收入多少？
3. 继任计划里"多名持有代码权限的可信开发者"是谁、什么关系、有没有报酬？真到那一天，PTY LTD 的股权和 Stripe 账户怎么交接——社会契约如何落成法律文件？
4. 有没有人实际出价收购过 Bear？最高出到多少？"不卖"的承诺在真金白银面前被测试过吗？
5. JustSketchMe 和 Bear 的收入比例如何演变？多产品组合是刻意的风险对冲策略，还是兴趣驱动的自然结果——他会建议别的独立开发者"先有一个养家的产品，再做梦想产品"吗？

## 来源

1. Herman's blog: The Hacker News Hug（2020-05-29）— https://herman.bearblog.dev/the-hacker-news-hug/
2. Herman's blog: My product is my garden（2020-12-01）— https://herman.bearblog.dev/my-product-is-my-garden/
3. Herman's blog: On running a blogging platform（2022-05-18）— https://herman.bearblog.dev/running-a-blogging-platform/
4. Herman's blog: A better ranking algorithm（2022-07-07）— https://herman.bearblog.dev/a-better-ranking-algorithm/
5. Herman's blog: Building software to last forever（2022-10-25）— https://herman.bearblog.dev/building-software-to-last-forever/
6. Day Two Cloud #187 播客: The Back End of Bear Blog（2023-03-22）— https://packetpushers.net/podcasts/day-two-devops/d2c187-the-back-end-of-bear-blog-with-herman-martinus/
7. Herman's blog: The ChatGPT vs Bear Blog spam war（2023-04-16）— https://herman.bearblog.dev/the-chatgpt-vs-bear-blog-spam-war/
8. Herman's blog: The Frustration Loop（2023-09-20）— https://herman.bearblog.dev/the-frustration-loop/
9. Herman's blog: How I stay motivated as a solo-creator（2023-10-05）— https://herman.bearblog.dev/how-i-stay-motivated-as-a-solo-creator/
10. Herman 在 HN "side projects making $500/mo+" 帖下的评论（2024-01）— https://news.ycombinator.com/item?id=38937143
11. Herman's blog: Upcoming changes to the discovery feed（2024-07-19）— https://herman.bearblog.dev/discovery-feed-changes/
12. Herman's blog: The Bear Manifesto（2025-01-27）— https://herman.bearblog.dev/manifesto/
13. Herman's blog: Bear is now source-available（2025-09-01）— https://herman.bearblog.dev/license/
14. Herman's blog: Miscellaneous updates（2025-09-19）— https://herman.bearblog.dev/misc-updates/
15. Herman's blog: Grow slowly, stay small（2025-12-03）— https://herman.bearblog.dev/grow-slowly-stay-small/
16. Herman's blog: Discovery and AI（2025-12-30）— https://herman.bearblog.dev/discovery-and-ai/
17. BoringCashCow: Interview with the founder of Bearblog（约 2023）— https://boringcashcow.com/interview/interview-with-the-founder-of-bearblog
18. Wonders of Web Weaving #3: Herman（James G 访谈）— https://web-weaving.jamesg.blog/3
19. Bear Blog 官网首页（2026-07 查看）— https://bearblog.dev/
20. Herman 项目页 — https://herman.bearblog.dev/projects/
21. Bear docs: Contributions（付费功能清单）— https://docs.bearblog.dev/contributions/
22. People & Blogs 系列访谈: Herman Martinus（镜像）— https://zacharykai.net/notes/pb/herman
23. Herman's blog: Bear Blog question challenge（2025-01-13）— https://herman.bearblog.dev/bear-blog-question-challenge/

[*] 定价备注：$5/月、$49/年、$189 终身为多个第三方评测与 HN 讨论交叉印证的口径（2024-2025 间有 $6/月、$59/年的记录，疑似调过价）；官方 upgrade 页需登录，未能直接核验。任务简报中"$4/月"未找到任何来源支持，以 $5/月为准。
