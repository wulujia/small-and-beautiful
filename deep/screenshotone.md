# ScreenshotOne（Dmytro Krasun）

> 在一个"竞品成堆"的截图 API 市场里，赌"把最好的产品做出来"就够了——替开发者扛下 headless browser 的所有脏活 ｜ screenshotone.com ｜ Dmytro Krasun（乌克兰）｜ 2022（2022-01-05 买域名，2022-05-29 上线）[1][4] ｜ 1 人（solo，四年无雇员）[1][4] ｜ 开发者工具 / API / headless browser 基础设施 ｜ $25k+ MRR、800+ 付费客户（2026-03）[2]；$33k MRR、1,000+ 付费客户（2026-05）[4]

## 缝隙切入点

- 切入方式几乎是"反直觉教科书"：从 10 年服务端工程师经验里列了一张"自己遇到过的问题"清单，随手选中 "screenshot API"。Google 一搜发现竞品成堆，别人会吓退，他的结论是："I realized—it meant that the market was validated and I just needed to build the best product in the niche."[1]
- 缝隙的本质不是"截图"，而是 headless browser 的运维地狱：CPU/RAM 尖峰、字体包、超时重试、并发限制、反爬对抗、cookie 弹窗。他的定位是替开发者扛下这些："offload the tedious tasks from developers and empower them to focus on more creative work. Rather than having headaches from dealing with headless browsers."[10]
- 需求面极宽但每个客户需求极小：网站图库、侵权监测软件、cold email 个性化、营销工具、链接预览/OG 图生成，以及后来的 AI agents——任何"需要把网页变成图"的应用都是客户 [2][16]。单点小需求 × 横向无数场景，才撑得起订阅生意。
- 个人时机与产品选择绑定：2021 年孩子出生 + 一份新 offer 摆在面前，他没休育儿假也没跳槽，直接辞职创业；第一个项目 Twitter 分析工具因为"没热情"放弃，才回到自己最擅长的 API 领域 [1][3]。

## 时机

- 2022 年入场时市场已被 ApiFlash、Urlbox 等验证十年，他赌的不是新品类而是"老品类里没人把产品做到位"[1]。
- 真正的时代红利在四年后到来：AI agents 成为新客户群，官网单独开辟 "The screenshot API for AI agents" 页面；有客户是通过 AI agent 找到 ScreenshotOne 的，10 分钟跑通 [16]。截图 API 恰好是 agent 感知网页的基础设施——2022 年埋的种子接住了 2025-2026 的 AI 流量。
- 内容时机踩得极早：2022 年 1 月 5 日买下域名后，产品还没写一行核心代码就开始写 SEO 内容，"到上线时已经有被索引的流量可以变现"[1]。

## 差异化

- 明面上的技术壁垒是脏活的积累：50,000+ 条规则和启发式的 cookie 弹窗屏蔽数据库、广告屏蔽、聊天挂件隐藏、懒加载全页截图——每一条规则都是四年运营攒下来的 [15]。
- 计费设计当信任武器：只有成功的截图才计费，失败请求不扣量，缓存命中不扣量 [8]。对按量付费的 API 来说，这是把"对账焦虑"直接做进产品。
- 支持即差异化：秒回工单、不按套餐分三六九等（"I don't differentiate between paid plans"）、要退款就退 [1]。SpyFu 创始人 Mike Roberts 的推荐语直接夸的是"响应快的创始人"[15]。
- SEO 打法反套路：先不管关键词，"Write the most useful piece of content for his ICP. Don't care about SEO, just deliver most value possible"，等索引后再挖 Google Search Console 的展现数据（哪怕排在第 50 页）找优化机会——用第一手数据而不是第三方工具 [11]。结果是 "screenshot API" 这个词做到 Google 第一 [11]。

## 第一批用户/冷启动

- 2022 年 5 月底上线后整整一个月零销售。6 月是"激进营销月"：付费广告、Reddit、Indie Hackers、目录站、Twitter 全试了一遍；他把这个月的复盘发在 Indie Hackers 上成了当月最火的帖子——而当时他差点放弃 [1]。
- 2022 年 7 月 4 日第一个付费客户：Twitter 上认识的 Jannis，做创作者工具目录站，需要自动截图 [1]；第一单只有约 $7/月 [12]。第二个客户来自 Google Ads [1]。
- 2023 年 3 月补了一次 Product Hunt：当日第 4 名、450+ 赞、1,800+ 访问、80+ 注册，直接收入只有一个 $140 年付升级，还收到一个收购提案。他的结论是值——情绪价值 + 一条高权重外链："It is a colossal win for me on all sides."[6]
- 冷启动最重要的资产是 Twitter 关系网："the community of entrepreneurs and developers on Twitter helped me, too, by advice, bringing my first paying customers, supporting my launches"[7]。

## 收入与定价

- 增长曲线是一条"前慢后快的直线"，前两年惨淡到靠接外包养活自己 [1]：
  - 2022-07：第一个付费客户（~$7/月）[1][12]
  - 2023-11：月均 ~$2,500，约 85 个客户，LTV ~$500，服务器成本 $600-800/月 [1]
  - 2024-03：仍未到 $5k MRR（他公开宣布"戒掉 Twitter 直到 $5k+ MRR"）[7]
  - 2024-09：$10k MRR（上线 2 年 4 个月）[3]
  - 2025-06：$20k MRR（从 $10k 到 $20k 只用 8 个月）[3]
  - 2026-03：$25k+ MRR，800+ 付费客户 [2]
  - 2026-05：$33k MRR，1,000+ 付费客户，累计 1 亿+ API 请求（四周年）[4]
- 当前定价（2026-07）：免费 100 张/月全功能；Basic $17/月 2,000 张；Growth $79/月 10,000 张；Scale $259/月 50,000 张 + GPU 渲染；超量按 $0.009/$0.006/$0.004 每张递减计费；年付送两个月 [8]。订阅 + pay-as-you-go 超量是他明确推荐的模型 [2]。
- ARPU 长期只有 ~$30（$25k/800 ≈ $31 [2]；$33k/1000 ≈ $33 [4]）——这门生意是几百个小客户各付一小笔堆出来的，不靠大合同。
- 2026 年他把涨价列为尝试过的增长杠杆之一，但没能打破线性增长 [5]。目标：$50k MRR [2]。

## 内容与增长

- SEO 是第一渠道：产品未动内容先行（2022-01 起），写的都是"我做产品时踩的坑 + 我的产品怎么更快解决"，比如"截图时怎么隐藏聊天挂件"[1]。"screenshot API" 等核心词做到 Google 前列乃至第一 [1][11]。他也坦承 SEO 的代价："SEO is a long-term game"，如果重来不会从 SEO 开始 [1]。
- Google Ads 是早期第二获客渠道 [1]。测过但效果一般的：Reddit 推广、目录站、Twitter Ads、LinkedIn、Product Hunt（拉新弱、外链强）[1][11]。
- 但到 2026 年他的答案变了："The channel that really started working for me was Reddit. But I don't think that would work for everybody... You need to experiment a lot and double down on what works."[2]——同一个渠道早期没跑通、后期成了主力，本身就是个值得深挖的故事。
- 免费工具做流量矩阵：How Browsers Work（GitHub 203 星）、Open Graph Examples、Open Graph Debugger、Puppeteer.Guide——全是围绕"网页渲染"这个母题的 SEO 卫星站 [13][14]。2024-10 他专门写过《Building Free Tools for SEO》[9]。
- 顺手吃 programmatic SEO 的生态位：官方博客教用户拿 ScreenshotOne + Airtable + Launchman 搭建程序化 SEO 站——把"别人做 pSEO 需要批量截图"变成自己的用例 [17]。2025-11 他开始研究"给 SEO 和 AI（LLM 引用）写博客"带来付费客户的路径 [9]。
- 增长哲学是漏斗调优而不是找新渠道："Don't have visitors? Work on attracting them. Have visitors, but they don't sign up? Improve your signup flow."[2]

## 社区

- Build in public 是他最出名的标签：两年把 Twitter 从 ~30 粉丝做到 12,000+，方法只有一个——"I just exposed myself to Twitter daily for two years"[7]。社区给他带来了第一批付费客户和所有 launch 的支持 [7]。
- 但他对这个渠道的清醒罕见：2024-03 公开宣布退出 Twitter 直到 $5k+ MRR，理由是时间黑洞伤害心智和产出 [7]。他保住了底线："I succeeded in not commoditizing myself and staying true to myself."[7]
- 2025-04 他还专门写过《About MRR screenshots but this time honestly》，反思晒 MRR 截图这件事本身 [9]——build in public 的既得利益者公开质疑 build in public，是访谈的好切口。

## 留存

- 留存做在计费诚实上：失败不计费、缓存不计费、90%/100% 用量邮件提醒、30 天退款 [8]。
- 2023-11 时 LTV 约 $500，对照 ~$29 的 ARPU 意味着平均客户生命周期超过一年 [1]。
- 2026 年他把降 churn 列为已尝试的杠杆之一；他的诊断框架是把一次性用户和持续用户分开、向高活跃客户升售 [5]。

## 转型

- 严格说没有转型，只有三次校准：① 弃掉没热情的 Twitter 分析工具，回到 API 老本行 [1]；② 从"服务所有人"收窄到特定客户段——他说花了两年才想明白客户到底是谁："It took me two years to realize that. And it changed everything. How I market things, what I write, what I build, pricing — everything."[2]（具体是什么洞察，公开材料里他始终没说透——见开放问题）；③ 定位从 "for developers" 扩成 "for developers and AI agents"[2][16]。
- 2026-06 他公开承认增长是"零加速"的线性 +$1k MRR/月，并给出自己的诊断方法论："Linear growth is not mysterious. It is what happens when your acquisition, conversion, retention, pricing, and market size are all roughly stable."[5]——一个 solo 创始人在公开场合做增长自我手术，是这个案例最新鲜的部分。

## 如何保持小

- 四年 solo，$33k MRR 没有雇员 [1][4]。基础设施独自搬了四次家：DigitalOcean droplet → Render → GCP 自动扩缩 → 自管 Kubernetes（为省 GCP 成本）[1]；技术栈从 Go + JS 长到 Next.js、Astro、TypeScript、Cloudflare、K8s [2]。
- 工具极简主义：Apple Notes 记想法、Trello 排任务、Google Sheets 手动录月度数据——故意手动，"留出反思时间"[1]。"Don't overcomplicate—customer satisfaction of your service matters more than the tools you use."[1]
- 保持小的哲学就是他成功的原因："I only started seeing results when I downgraded my ambition and focused on achieving small things in easy steps."[2] 下一个目标不是招人，而是把运营自动化到"可以离线一周"[2]。
- 小的回报是生活本身：四周年复盘里他列的成就是家庭时间、阅读、旅行、"proved to myself I can achieve things"，以及 "I found ways to sustain my motivation to work on the product, and I don't see why I would stop."[4]
- 对建议的态度同样"小"："Don't listen to any advice."——他推荐读经济学和商业基本原理，而不是战术指南 [2]。

## 开放问题（值得当面问创始人的）

1. 你说"花了两年才明白客户到底是谁，从此营销、文案、产品、定价全变了"——那个洞察具体是什么？它先改变了哪一项？
2. Reddit 早期试过没用、后来却成了"真正跑通的渠道"，中间你改变了什么？哪些 subreddit、什么姿势（发帖 vs 答题）、怎么归因转化？
3. 一个人运维 headless browser 集群四年，最接近崩盘的一次事故是什么？$33k MRR 还不招人，是财务决定、性格决定，还是对"公司"这个形态的拒绝？
4. 2026-06 你诊断自己是"零加速线性增长"（+$1k/月），按你自己的框架，现在找到那个约束变量了吗——是市场规模就这么大，还是漏斗里还有非线性机会？
5. AI agents 现在占新增用量/客户多少？对截图 API 是十年一遇的顺风，还是最终威胁（agent 自己驱动浏览器）？Product Hunt 之后你收到过收购提案——什么条件下你会卖？

## 来源

1. Starter Story：Quitting My Cushy SDE Job To Build A Screenshot API [$2.2K MRR]（2023-11）— https://www.starterstory.com/stories/screenshotone
2. Indie Hackers：Hitting $25k+ MRR by making his goals less ambitious（2026-03）— https://www.indiehackers.com/post/tech/hitting-25k-mrr-by-making-his-goals-less-ambitious-jQRZDnzwm8DFAaS4Xrq0
3. Dmytro Krasun：Reached $20K MRR. What's next?（2025-07-17）— https://dmytrokrasun.com/posts/20k-mrr-whats-next/
4. Dmytro Krasun：4 Years of Running ScreenshotOne（2026-05-29）— https://dmytrokrasun.com/posts/screenshotone-4-years/
5. Dmytro Krasun：Zero Growth Acceleration（2026-06-21）— https://dmytrokrasun.com/posts/zero-growth-acceleration/
6. Dmytro Krasun：Was the Product Hunt launch worth it?（2023-03）— https://dmytrokrasun.com/posts/the-product-hunt-launch-for-screenshotone/
7. Dmytro Krasun newsletter：I quit Twitter till I reach $5K+ MRR（2024-03-10）— https://newsletter.dmytrokrasun.com/p/i-quit-twitter-till-i-reach-5k-mrr
8. ScreenshotOne Pricing（2026-07 抓取）— https://screenshotone.com/pricing/
9. Dmytro Krasun newsletter 存档（Building Free Tools for SEO 2024-10-21；About MRR screenshots but this time honestly 2025-04-30；Blog posts for SEO and AI that bring paying customers 2025-11-24）— https://newsletter.dmytrokrasun.com/archive
10. ScreenshotOne About — https://screenshotone.com/about/
11. Superframeworks：$269K ARR Simple Screenshot API（2025-01-31）— https://superframeworks.com/blog/screenshot-one
12. Indie Goodies 访谈：Dmytro Krasun — https://indiegoodies.com/interviews/dmytro_krasun
13. dmytrokrasun.com（个人站，项目与访谈列表）— https://dmytrokrasun.com/
14. GitHub @krasun（howbrowserswork 等仓库）— https://github.com/krasun
15. ScreenshotOne 首页（2026-07 抓取，50,000+ cookie 弹窗规则、客户推荐语）— https://screenshotone.com/
16. ScreenshotOne：The screenshot API for AI agents / Use cases — https://screenshotone.com/agents/ 、 https://screenshotone.com/use-cases/
17. ScreenshotOne Blog：How to build a Programmatic SEO site with automated website screenshots — https://screenshotone.com/blog/how-to-build-a-programmatic-seo-site-with-automated-website-screenshots-using-screenshotone-airtable-and-launchman/
