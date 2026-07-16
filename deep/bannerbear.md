# Bannerbear（Jon Yongfook）

> 用 API 把"手工做营销图"自动化：模板 + 数据 = 批量生成社媒图 / OG 图 / 视频 / PDF ｜ bannerbear.com ｜ Jon Yongfook Cockle ｜ 2019 年（前身 Previewmojo）/ 2020 年改名并转型 API ｜ 峰值 5 人全职远程，现自述"一人 + AI"（第三方库记录 4-6 人，存疑）｜ API / 开发者工具 / pure-bootstrap / build in public ｜ $1M ARR（2025-09-19 官宣）[5]

## 缝隙切入点

- 痛点来自亲身经历：Jon 早年在电商公司带设计团队，每天为新上架商品手工做视觉素材的重复劳动让他印象深刻，这成了他的"North Star"——为未来的公司解决这个问题 [1][7]。
- 起点极窄：2019 年 9 月上线 Previewmojo，只做一件事——从模板生成 Open Graph 尺寸的分享图。到 2019 年底 MRR 只有 $400 [1]。
- 关键认知：Wavve 创始人给他泼冷水说 OG 图生成"有用但不关键"，只是营销自动化的一小块。Jon 由此悟出他后来反复引用的一句话："The advice 'Niche Down' means niche down your target market—it doesn't mean niche down the pain point you solve." [1][8]
- 2020 年 3-4 月转型为 REST API：同一个模板引擎，用例从 OG 图扩展到电商广告图、meme、个性化邮件配图等一切"数据驱动的图"。没有用户明说要 API——"Nobody specifically said 'I need a REST API that generates images' but rarely do we get handed these things on a plate."（Jon 原话）[10]

## 时机

- 踩中 2020 年 NoCode 浪潮：Jon 主动监测趋势，接入 Zapier 让不会写代码的人也能自动生成图片，用户由此分成两类原型——Zapier 自动化用户和 API 开发者用户，后来的定价方案（Automate / Scale）就是按这两类人切的 [1][8]。
- 2019 年独立开发者圈流行"每篇博客/每个页面配 OG 图"的增长玩法，先有场景热度，Previewmojo 才有第一批注意力（Product Hunt 当日第 2 名）[8]。

## 差异化

- API-first + 设计师基因：Jon 做过 20 年设计师兼程序员（东京设计公司、电通、Aviva 亚洲数字与产品设计负责人），既能写模板引擎又懂视觉，这是他总结的第一条经验"Aim for Product-Founder fit"——"genuine passion will make all the difference between you giving up early, and sticking to it through the ups and downs." [3][9]
- 品牌刻意"可爱化"对冲 API 产品的冰冷：黄色小熊吉祥物、泰迪熊周边、里程碑长文，让一个开发者工具变得"retweet-able"（他的第 5 条经验）[3]。
- 技术上反潮流：$1M ARR 时的技术栈仍是 Rails 6 + jQuery。"Bannerbear got to $1 million ARR on Rails 6 and jQuery. You don't need to be on the cutting edge of tech all the time."（2025-09 推文）[5]

## 第一批用户/冷启动

- 冷启动前的失败教训：纯陌生邮件冷推销"got absolutely nowhere"；Shopify 应用商店虽然每天自然带来 5-10 个安装，但 2020 年 3 月他主动关掉了它——Shopify 用户只肯付 $5/月，且"我做了一个技术型产品，却卖给了非技术用户"，客服成本吃不消 [10]。
- API 上线后转向"warm outreach"：只跟进已注册的高价值用户，而不是陌生名单 [10]。
- 2020 年 6 月约 40 个付费客户、$1,000 MRR；此后靠内容和文档自然增长：6 月 $1k → 7 月 $2k → 8 月 $3k → 10 月 $6k [1][4]。
- 文档是转化引擎："The more documentation I wrote the more conversions I got."（Jon 原话）[1]

## 收入与定价

- 定价演进是最贵的一课：早期 $9/月，他后来算过按这个价要 2,000 个客户才抵得上现在的收入；提价到 $49-$399/月后获客压力骤降 [8]。第 2 条经验直接叫"Don't price too low"——$5-10 的价位吸引的是最爱抱怨的低价值客户 [3]。
- 当前定价（2026）：Automate $49/月（1,000 API credits）、Scale $149/月（10,000 credits）、Enterprise $299/月（20,000 credits），免费试用 30 credits 无需信用卡 [11]。
- 营收里程碑（全部公开可查）：2021-01 破 $10K MRR（耗时 2 年）[1]；2021-12 $27K [2]；2022-06 $40K、2022-10 $50K [4]；2023-07 确认 $50K [3]；2025-09-19 官宣 $1M ARR [5]。第三方 Latka 数据：2024 年收入 $991.4K、596 个客户 [13]。
- 全程 pure-bootstrap，零融资 [16]。

## 内容与增长

- 核心方法论（他最广为流传的一句话）："If you want to go from 0 to $10K MRR you should divide your time 50:50 between coding and marketing." 具体执行：一周写代码、一周做营销（博客/推特/论坛），每个周期发一期 newsletter，用看板 + 故事点保持节奏。这个节奏画出了他说的"straight diagonal line upwards"的增长曲线 [1][3][8]。
- Build in public 是获客渠道而非表演：2021 年 1 月《Journey to $10K MRR》长文上了 Hacker News 首页；每个里程碑（$10K/$20K/$50K/$1M）都做成"flagship content"，这是他的第 5 条经验"Be retweet-able" [2][3]。Indie Hackers 上的 AMA、播客 #208 访谈都带来持续曝光 [2][7]。
- 免费工具做 SEO：Free Certificate Generator 冲到 "certificate maker" 谷歌第一页，加上 Tweetagram 等工具，定位是"backlinks、搜索流量和 SEO 排名，而非直接转化"（第 4 条经验）[2][3]。
- 技术长尾内容只有创始人能写：《8 Tips for Faster Puppeteer Screenshots》、FFmpeg 教程等带来稳定自然流量，Jon 明说这类内容"basically impossible to delegate or outsource" [2]。
- 花过的最古怪营销钱：约 $2,000 在 Cameo 上请《硅谷》演员录了条背书视频，换来一波 Twitter 传播 [2]。
- 他自己承认的盲区：没装 cookie 跟踪，说不清哪个动作最有效 [2]。

## 留存

- 2020 年 3 月经历过一次明显 churn：COVID 恐慌 + API 转型让一部分老客户（OG 图用户）流失，但 MRR 很快补回 [10（转型背景）][16]。
- Latka 记录的月流失率 4.8%，客户 LTV 超过 $1,800 [13]——API 深度集成进客户工作流后粘性强，但数据来源为第三方，未经 Jon 本人确认。
- 2021 年中参照 Stripe 重做 API 文档、上线 quick start 示例页、补知识库，本质都是降低集成摩擦的留存动作 [2]。

## 转型

- 三次关键转身：① 12 startups 挑战做到第 7 个烧尽（burnout），零收入——他的总结是挑战的价值不是找到爆款，而是"time box yourself and ship something"，并给出方向感（"compass bearing"）指向图片自动化 [1][8]；② Previewmojo（OG 图工具）→ Bannerbear（图片生成 API），同时砍掉 Shopify 应用 [1][10]；③ 2025 年底静默发布 V5——"Most significant upgrade in the last 4 years"，重写模板引擎/编辑器/API，加入 AI 能力（渲染时 AI 生成背景、AI 抠图、人脸/主体检测）[6][14]。
- V5 用 Claude Code、Cursor 等 AI 工具完成大量重写，Jon 在推文里坦言：用 AI 干完这一切之后，发布"少了些成就感/仪式感"（feel like much less of an "occasion"）[6]。

## 如何保持小

- 第 6 条经验"Hire when it hurts"：只在痛到做不动时才招人，第一个岗位通常是客服；反对"aspirational hires"（需要大量带教的期望型招聘）[3]。实际路径：原以为会一人做到底，$15K MRR 时撑不住才招第一个人 [16]；2021 年底有 1 名全职内容写手 + 2 名客服 [2]；2022 年是 5 人全职、100% 远程 [18]。
- 2025 年的反向操作：$1M ARR 之际他重新以"solo tech founder"自述 [4]，靠 AI 工具维持产出（第三方称其"velocity of a 10-person engineering team while remaining a team of one"）[17]。但 Tracxn 2026-04 记录 6 名员工、Latka 2025-04 记录 4 名 [13][17]——从 5 人团队到"一个人"之间发生了什么，公开资料完全空白，是最值得当面问的问题。
- 透明度也做了减法：曾是完全公开指标的 open startup（open 页上还挂过给自己买摩托车的进度条"Moto Meter"），2023 年后改为"only share selected metrics" [2][12]。
- 生活方式设计的完整弧线：英国长大（英中混血，1980 年生）[15] → 东京设计公司、电通 → 1.5 年数字游民"在海滩上做社交媒体软件" → 新加坡 Aviva 亚洲数字负责人，2018 年 7 月辞职 [9] → 定居新加坡做 Bannerbear 至今。他把 12 startups 挑战称为"an anti-MBA where instead of sitting in a classroom learning theory, you get out of the building"，目标是找到自己的 ikigai [9]。

## 开放问题（值得当面问创始人的）

1. 从 5 人全职团队回到"一个人 + AI"，中间发生了什么？是主动收缩还是自然流失？做这个决定时怎么跟团队交代、心理上怎么过关？（公开资料完全没有这段。）
2. 2023 年你关掉了 open metrics 页面，从"完全透明"退到"选择性公开"——是什么让透明的成本开始超过收益？竞争对手抄袭、客户拿数字砍价，还是别的？
3. 你说用 AI 重写 V5 之后发布"少了成就感"——一个人公司里，成就感的来源没了怎么补？这会动摇你继续做下去的动力吗？
4. 12 startups 做到第 7 个 burnout 停下。回头看，"该停"的信号是什么？如果当时第 3 个月就有人告诉你答案在图片自动化，你会信吗——还是必须亲自烧完那 7 个？
5. Bannerbear 的终局是什么？$1M ARR 之后，你想过卖掉、当现金牛、还是做到不能做为止？新加坡的定居生活（对比数字游民时期）怎么影响这个答案？

## 来源

1. Jon Yongfook, "Here's How I Bootstrapped a SaaS to $10k MRR", bannerbear.com, 2021-01 — https://www.bannerbear.com/journey-to-10k-mrr/
2. Jon Yongfook, "1 Year of Marketing a SaaS from $10K MRR to $27K MRR", bannerbear.com, 2021-12 — https://www.bannerbear.com/blog/one-year-of-marketing-a-saas-from-10k-to-20k-mrr/
3. Jon Yongfook, "7 Lessons Growing a Bootstrapped SaaS to $50K MRR", bannerbear.com, 2023-07 — https://www.bannerbear.com/blog/7-lessons-growing-a-bootstrapped-saas-to-50k-mrr/
4. "Journey to $1 Million ARR", bannerbear.com — https://www.bannerbear.com/journey-to-1-million-arr/
5. Jon Yongfook, X post, 2025-09-19 — https://x.com/yongfook/status/1969022369336356874
6. Jon Yongfook, X post（V5 发布 + AI 感想），2025-12 — https://x.com/yongfook/status/2069252888287924337
7. Indie Hackers Podcast #208, "How this Indie Hacker Blew Past $10K MRR with Jon Yongfook of Bannerbear" — https://www.indiehackers.com/podcast/208-jon-yongfook
8. The Wizdom Project, "Living the Indie Hacker Dream | Jon Yongfook"（播客笔记）— https://thewizdomproject.com/jon-yongfook-podcast-notes
9. Coconuts Singapore, "This man quit his job in Singapore to start 12 startups in 12 months", 2019 — https://coconuts.co/singapore/news/man-quit-job-singapore-start-12-startups-12-months/
10. Jon Yongfook, "Launched my API and shut down my Shopify app", Indie Hackers, 2020-03-12 — https://www.indiehackers.com/product/bannerbear/launched-my-api-and-shut-down-my-shopify-app--M2CybHO6hWH_0q6jm2d
11. Bannerbear Pricing（2026-07 抓取）— https://www.bannerbear.com/pricing/
12. Bannerbear Open Startup 页 — https://www.bannerbear.com/open/
13. Latka, Bannerbear 公司数据（2024 收入 $991.4K、596 客户、4.8% 月流失、LTV >$1,800；2025-04 更新，第三方估算需谨慎）— https://getlatka.com/companies/bannerbear
14. "Bannerbear V5 Full List of New Features", bannerbear.com, 2026-06 — https://www.bannerbear.com/blog/bannerbear-v5-new-features-list/
15. Jon Yongfook, X post（个人背景：英国人、英中混血、1980 年生）— https://x.com/yongfook/status/1958534892528206227
16. Starter Story, "How Jon Yongfook Bootstrapped Bannerbear To $50K MRR in 3 Years" — https://www.starterstory.com/stories/bannerbear-breakdown
17. Tracxn, Bannerbear 公司档案（2026-04：6 名员工）— https://tracxn.com/d/companies/bannerbear/__go5dE-3gKuTGKX4WRnkrIu0vqP91IPeatFtrfgyzIMQ ；另见 solobusinesshub 等对"team of one + AI"的转述
18. Jon Yongfook Cockle, LinkedIn（2022："a small 100% remote company with 5 full time team members"）— https://www.linkedin.com/posts/yongfook_about-activity-6906859861288611840-k6u0
