# Devv.ai（Jiayuan Zhang）

> 在通用 AI 搜索（Perplexity/You.com）和通用 Chatbot（ChatGPT）之间，做只服务开发者的垂直 AI 搜索引擎 ｜ devv.ai ｜ Jiayuan Zhang（英文名 Forrest，X @Tisoga，即刻"加元.Jiayuan"，GitHub forrestchang，Ex-TikTok）[3][4][17] ｜ 2023 ｜ 2-10 人（Product Hunt makers 共 3 人）[3][9] ｜ AI 搜索 / Dev Tools / 出海 ｜ 付费上线首月收入超 $28,000（2024-03），复盘期约 $30k/月 [1]

**名字勘误**：中文圈流传的创始人名"蒋泽宇"查无出处。所有一手来源（Product Hunt maker 页、GitHub、即刻、X）均指向 Jiayuan Zhang；部分中文报道称其为 Forrest Zhang [3][8][17]。联合创始人（PH makers）另有 Bohan 和 Kai（Haoguang Cai）[3]。

## 缝隙切入点

缝隙里还有缝隙。2023 年 AI 搜索已是红海（Perplexity、You.com），甚至"开发者 AI 搜索"也已有 Phind——但 Jiayuan 判断这些产品全部依赖 Google/Bing 的通用搜索结果，而开发场景需要的是另一种索引：Devv 自建了面向开发领域的搜索索引，爬取并索引开发者网站、官方文档和 GitHub 等开源代码库，再套 RAG 管线 [1][2]。官方称在中文等多语言场景下，其引用（citation）准确率明显好于 Perplexity、Bing Chat 和 Phind [15]——这暴露了第二层缝隙：海外 AI 搜索没人认真服务中文开发者。

动手前的验证动作教科书级：先和 50 位不同背景的开发者做 1:1 Zoom 访谈，确认共同痛点是"受够了通用 AI 工具生成不准确的代码片段"；然后给自己定了一周内做完 MVP 上线的目标 [1][2]。

## 时机

- 2023 年 ChatGPT 代码幻觉是开发者的日常抱怨，"可信的 AI 编程答案"是真实空缺 [1][2]。
- 2023-11 中旬在 X 上发布 [5]，正踩在 AI 搜索概念最热、但垂直玩家稀少的窗口。
- 中国开发者当时没有顺手的同类产品（Phind/Perplexity 对中文支持差），Devv 靠中文开发者社群吃到了第一波指数增长 [1][2]。

## 差异化

- 自建垂直搜索索引（文档 + 开源代码 + 开发者网站）+ RAG，而非转发 Google/Bing 结果 [1][2]。
- Agent 模式：自动把任务分类到专门的 agent 类型（代码生成、解释、调试、优化、联网搜索）[1][2]。
- 为开发者做的克制 UI，"简洁直观，无杂乱要素" [2]。
- 中文场景引用准确率优于 Perplexity/Bing Chat/Phind（官方口径）[15]。
- 2023-12-28 就发了桌面端（macOS/Windows），把"默认搜索工具"往系统层推 [10]。

## 第一批用户/冷启动

- 路径：50 场访谈 → 一周 MVP → 发给朋友和同事 → 发到自己的 Twitter（关注者大多是中国开发者）→ 纯口碑传播，几个月内超过 50 万用户 [1][2]。
- 没花一分钱投放，"开发者们在整个中国疯狂安利这个工具" [1][2]。
- 后置的海外动作：Show HN（2024-05）[12]；Product Hunt 2024-06-24 发布，当日榜第 3，475 赞 [3]。注意顺序——先在中文圈起量，被墙后才认真做英文世界的 launch。

## 收入与定价

- 2024-03 推出付费订阅（Premium），首月收入超过 $28,000 [1][2]。
- 复盘发布时（2024-03-27）标题口径为 $30k/月，"数字还在持续增长" [1]。
- 转型后（Devv 2.0）改为按 credits 计费：credits 消耗于 Coding Agent 等计算密集操作，按任务复杂度和所用模型扣减 [18]。
- 具体订阅价、付费转化率、2024 下半年之后的收入曲线均未公开。

## 内容与增长

创始人本人就是增长渠道，全程 build in public：

- **X @Tisoga**：发布日推文（2023-11）[5]；《devv.ai 是如何构建高效的 RAG 系统的》系列长 thread（讲索引构建、RAG 评估、生产环境实践），被腾讯云开发者社区等平台转载，技术分享直接反哺产品获客 [15]；后续还有"从零开始 AI 编程"系列（用 Devv Builder + Lovable 搭博客）[16]。
- **即刻"加元.Jiayuan"**：高频复盘产品进展（60 万开发者、PH 日榜第 3、头部美元基金投资、招实习生等一手信息都先发在这里）[4]。
- **Newsletter**：竹白 jiayuan.zhubai.love，定期发系统性观点与 weekly reading；随竹白平台衰落现已无法访问 [19]。
- 复盘长文本身也是增长动作：《How we built an AI search engine for devs that makes $30k/mo》发在 Indie Hackers，被人人都是产品经理、腾讯新闻、阿里云创业频道等中文媒体大量转译 [1][2]。

## 转型

这家公司的主线剧情是两次被迫/主动的急转弯：

1. **被墙（≈2024 年初）**：Devv 突遭防火长城封禁，一夜之间失去中国大陆用户——当时几乎全部的用户盘子。团队"重新出发，调整 Devv 以适应全球受众" [1][2]。
2. **回攻国内（2024-11）**：发布国内版「代悟」（beta.daiwu.cn）进入 Beta，定位不变：开发者专属 AI 搜索 [8]。后续进展未见公开报道。
3. **从搜索到 Coding Agent（2025）**：2024 下半年先加 Playground（实时代码生成预览）、Contexts、Claude 3.5 Sonnet/o1 支持 [6]；2025-02-12 发 Devv Builder 公测（自称"全球首个 AI-powered Instant Backend"，prompt 直接生成后端 API）[6]；2025-05-14 Devv 2.0 私测，彻底从"AI 搜索引擎"转为"AI App Builder"，邀请码在 X 上发放 [6][13][16]；2025-08-27 公开发布，新定位"The First AI Coding Agent to Build Full-Stack AI Products" [6][7]。
4. **新定位的差异化**：明确对标 Lovable/Bolt——"不是做漂亮 landing page 和 demo，而是做真正的 AI 产品"，内置 LLM、图像/音频生成、后台任务、鉴权、数据库、邮件等集成；目标用户从开发者扩展到产品经理、设计师、创始人等"有想法但没工程能力的人" [14]。官网现宣称 700k+ 开发者信任、"backed by millions in funding" [7][14]。

背景值得注意（推断，创始人未公开说明转型动因）：2024-2025 年 ChatGPT/Claude/Cursor 相继内置联网搜索与编程能力，独立"开发者 AI 搜索"的生存空间被系统性挤压，Phind 同期也转向了 coding agent。Devv 的转身与其说是机会驱动，不如说是缝隙关闭后的求生。

## 如何保持小

- 团队三年维持在个位数：PH makers 3 人（Jiayuan、Bohan、Kai）[3]，LinkedIn 公司规模 2-10 人 [9]，即刻上公开招聘的岗位是实习生 [4]。
- 拿了"头部美元基金"的早期投资（即刻自述），官网口径"millions in funding"，但没有走烧钱扩张路线 [4][7][14]。
- Dogfooding 压成本：Devv 2.0 的 landing page、邀请系统、内部工具都是用 Devv 2.0 自己搭的，自称比旧工作流快 5 倍 [14]。
- 增长全靠创始人的内容输出与口碑，无投放团队、无销售团队（见"内容与增长"）[1][4]。

## 开放问题（值得当面问创始人的）

1. 被墙那天的真实账本：50 万用户里活跃/付费占比多少？转向全球后老用户留下来多少？如果没被墙，今天会是一家什么样的公司？
2. $30k/月 之后的收入曲线是什么形状？决定做 Devv 2.0 时，搜索订阅收入是在涨还是在跌——转型是进攻还是撤退？
3. "头部美元基金"是哪家、金额多少？拿了机构的钱之后，为什么还能顶住压力保持 2-10 人、不扩张？投资人对"小"的容忍度有多久？
4. 从服务 70 万开发者转向服务"不会写码的人"，等于换了一遍用户画像——老用户迁移率多少？自建的开发者搜索索引这项核心资产，在 2.0 里还值钱吗？
5. 代悟现在什么状态？一个个位数团队同时打海外（Lovable/Bolt 的战场）和国内（合规 + 大厂竞争），这个双线决策今天怎么评价？

## 来源

1. Indie Hackers：How we built an AI search engine for devs that makes $30k/mo（Jiayuan Zhang 本人，2024-03-27）— https://www.indiehackers.com/post/how-we-built-an-ai-search-engine-for-devs-that-makes-30k-mo-SlB19aYcVZ8pGu3hNwhg
2. FisherAI 中译：Devv 是如何打造一个月入 3 万美元的开发者 AI 搜索引擎的 — https://fisherdaddy.com/posts/how-we-built-an-ai-search-engine-for-devs/ （同文另见人人都是产品经理 https://www.woshipm.com/chuangye/6069656.html ）
3. Product Hunt：Devv.AI（2024-06-24 发布，日榜 #3，475 赞；makers：Jiayuan Zhang/Bohan/Kai）— https://www.producthunt.com/products/devv-ai
4. 即刻"加元.Jiayuan"主页（简介"Building AI | Devv.AI 创始人 | Ex-TikTok"）— https://m.okjike.com/users/EC14C663-82C2-4584-A8C7-FF95F306B779
5. X @Tisoga：Devv 发布推文（2023-11）— https://twitter.com/Tisoga/status/1724623193582060018
6. Devv Changelog（Playground 2024-10-16；Builder 公测 2025-02-12；2.0 私测 2025-05-14；公开发布 2025-08-27）— https://hub.devv.ai/changelog
7. Devv 官网（"The First AI Coding Agent to Build Full-Stack AI Products"）— https://devv.ai/ ；中文版 https://devv.ai/zh
8. 站长之家：Devv 国内版「代悟」发布，进入 Beta（2024-11-26）— https://www.chinaz.com/ainews/13493.shtml
9. LinkedIn：Devv.AI 公司页（Software Development，2-10 人，founded 2023）— https://www.linkedin.com/company/devv-ai
10. GitHub：devv-ai/devv（官方 issues 仓库，1.5k stars；Devv Desktop 2023-12-28 发布）— https://github.com/devv-ai/devv
11. Verne in GitHub：面向开发者的垂直搜索引擎 devv.ai（2023-11 早期第三方评测）— https://blog.einverne.info/post/2023/11/devv-ai.html
12. Hacker News：Show HN: Devv – AI search engine for devs, built on a custom search index（2024-05）— https://news.ycombinator.com/item?id=40288111
13. AIbase：Devv 2.0 正式进入私测（2025-05）— https://www.aibase.com/news/18037
14. navi.tools：Devv 条目（转引官方描述：700k+ developers、对标 Lovable/Bolt、dogfooding 5x）— https://navi.tools/tools/devv
15. Typefully @Tisoga：Building an Efficient RAG System 系列 — https://typefully.com/Tisoga/PBB58Vu ；腾讯云转载：devv.ai 是如何构建高效的 RAG 系统的 — https://cloud.tencent.com/developer/article/2376781
16. X @tisoga：Devv 2.0 邀请码（2025-05）— https://x.com/tisoga/status/1922819244099764315 ；从零开始 AI 编程系列（2025-02）— https://x.com/tisoga/status/1886218057921782258
17. GitHub：forrestchang（Jiayuan Zhang）— https://github.com/forrestchang
18. Devv Pricing（credits 计费）— https://devv.ai/pricing
19. 竹白：Jiayuan 的 Newsletter（已无法访问）— https://jiayuan.zhubai.love/
