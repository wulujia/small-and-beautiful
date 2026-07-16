# Zeabur（林沅霖）

> 在 Vercel 只管前端、Railway 没有亚洲机房的空档里，做对华语开发者最顺手的全栈一键部署 PaaS，再借 AI 浪潮转身为"AI DevOps 工程师" ｜ zeabur.com ｜ 创始人：林沅霖（台湾桃园人，浙大计算机系 2023 届）｜ 2022 毕设起步、2023 正式成立 ｜ 团队 11 人（2026，平均年龄 24 岁）｜ tag：PaaS / DevTool / 学生创业 / 华语开发者 ｜ 营收未公开（付费用户 5000+，注册 10 万+，2025 底）[1][9]

## 缝隙切入点

- 缝隙的发现来自亲身接案：林沅霖大学期间接了 30-40 个外包项目，发现"真正花时间的不是写程式，而是部署与交付"[1][4]。于是把毕设题目主动选成部署自动化工具（前身叫 Zeebird），室友试用觉得有用，才走向创业[1]。
- 竞品留下的三个空档：Vercel 只托管前端，Zeabur 把前端、后端、数据库、消息队列一站打包[2]；Railway 没有亚洲节点，Zeabur 提供香港/新加坡/东京机房，亚太用户延迟 15-60ms 对比欧美平台 150-200ms[12]；国际平台只收信用卡，Zeabur 支持支付宝和台湾本地支付方式，对无国际信用卡的华语开发者是硬门槛的消除[13][12]。
- 本质是对 AWS/GCP/阿里云的"二次封装"（用户戏称"二房东"），与云巨头合作而非竞争——巨头做底层资源，Zeabur 做"最后一哩路"的体验层[2][1][14]。
- 分层定位很清晰：资深工程师直接用 AWS/GCP，中阶开发者用 Heroku 类 PaaS，Zeabur 赌的是 AI 时代冒出来的"新开发者"——会让 AI 写代码、但不会部署的人[4]。

## 时机

- 2023 年入奇绩创坛（前 YC China，陆奇）春季营，那一届 60 个项目 100% 技术驱动，正值大模型创业潮起点[19][2]。
- 真正的时机红利是 2024-2025 年 AI 代码生成工具（Cursor 等）普及：大量"程式小白"能让 AI 写出代码，却卡死在部署环节。林沅霖坦言早期面向工程师时"付费意愿不是很高"，直到 Vibe Coding 人群涌入才找到愿意付钱的市场[6]。
- 他对"为什么巨头不来抢"的判断：科技大厂聚焦"写程式"这种离钱近的 AI 应用，"用 AI 管理基础设施离钱太远"，产投比不符合大厂战略——这正是小团队的时间窗[6]。
- 他的天花板叙事：如果 Vibe Coding 给云市场带来 1% 增量，Zeabur 吃下这个新增市场的 1%，"我们就能成为独角兽"[6]。

## 差异化

- 产品层：zbpack 自动识别语言/框架，不用写 Dockerfile；GitHub push 自动部署；前端+后端+数据库一站式；按量计费[3][12]。Next.js 项目实测约 90 秒部署完成[12]。
- 地理层：香港/新加坡/东京机房是对 Railway/Render 的直接错位——对做 Bot、API、实时服务的亚洲开发者，延迟差一个量级[12][13]。
- 语言与支付层：中文文档（zh-CN/zh-TW）、Discord 中英文社区、支付宝/台湾本地支付[11][2][13][12]。早期用户约 50% 来自中国大陆、近 50% 台湾、约 10% 欧美——这是 Vercel/Railway 天然照顾不到的人群[2]。
- 叙事层的三次升级：目标用户从"工程师"→"Vibe Coders"→"Builders（任何认真做产品的人）"，产品定位从部署工具升级为"AI DevOps Engineer"——用自然语言跟 AI Agent 对话完成部署、租服务器、配数据库、排查故障[1][20]。

## 第一批用户/冷启动

- 冷启动全在华语开发者聚集地：Telegram 周刊 + V2EX 发帖推广；一次半价订阅活动，在总用户仅 4000-6000 人时换来约 100 个付费用户——这是他们最早的付费验证[2]。
- 最聪明的一招：给热门开源 AI 项目的 GitHub README 提供"一键部署按钮"，把别人项目的流量变成自己的注册入口[2]。
- 创始人自己就是内容渠道：把个人博客从 Vercel 搬到 Zeabur 并写成文章，之后持续产出"用 Zeabur 部署 Django/Supabase/Line Bot"系列教程[20]。
- 2023 年 7 月 23 日 Product Hunt 首发，323 票拿下当日 #1[8]。媒体称其为台湾团队在 PH 的标志性成绩[1][3]。
- 增长数据轨迹：2024 年初 4000-6000 注册[2] → 成立 1.5 年 4 万注册、1.6-1.8 万活跃、1600+ 付费[4] → 2025 年底 10 万+ 注册、约 5000 付费[1]。

## 收入与定价

- 订阅 + 按量混合：现行方案 Free $0 / Dev $5 / Pro $19 / Team $79（3 席位）/月，月费内含等额资源额度，超出按量计费[10][12]。小型全栈应用月成本约 $5-10，与 Railway（$5 起）、Render（$7 起）同档，但机房选择更优[12]。
- 营收未公开。按 5000+ 付费用户、主流方案 $5-19/月粗估，MRR 在数万美元量级（估算，非官方）[1][10]。一个关键发现：美国用户付费意愿远高于其他市场，"同等用户数营收贡献是 1.5 倍以上"——这直接推动团队 2025 年把资金投向北美[6]。
- 定价在收紧：2026 年 3 月宣布取消免费层（老用户不受影响）[15]，2026 年 4 月停用共享集群、推动用户迁移到专属服务器，部分用户成本上升 20-50%，社区出现"都有 Vercel + Supabase 了还要 Zeabur 干嘛"的质疑声[12][14]。涨价争议暴露了"二房东"模式的被动性：底层成本不由自己控制，护城河只能靠整合体验[14]。
- 融资：奇绩创坛 pre-seed（2023 春季营）[19][3]；2025 年约 200 万美元种子轮，500 Global 领投，台湾 AVA 天使基金与老股东跟投，资金主要用于拓展北美市场[1][3][6]。

## 内容与增长

- 教程即获客：创始人博客（yual.in）的文章几乎都是"用 Zeabur 部署 X"的实操教程，覆盖 Django、Supabase、n8n、Line Bot 等长尾搜索词[20]。
- 播客与社区曝光密集：硬地骇客 EP51（2024.3，大陆独立开发圈）[2]、INSIDE 塞掐 Side Chat E330（台湾科技圈）[5]、COSCUP 2024 开源年会讲者[21]——同一个故事在两岸开发者圈层反复讲。
- "一键部署按钮"是分发杠杆：开源项目作者放按钮，Zeabur 按转化付 $5 credit/人，等于把 BD 外包给了整个开源生态[2][11]。
- 2025 年转向 build in public + 北美线下：团队驻点硅谷一个月，参加当地社区活动验证市场，推出 Zeabur AI Hub[1][6][7]。

## 社区

- Discord 是客服 + 社区双中心：中英文频道、异步论坛式交流；实测 Discord 几分钟有人响应，远快于官方工单的 8-24 小时——社区实质上承担了支持职能[2][12]。
- 模板市场是社区的经济系统：用户可把部署方案打包成模板上架，新模板过审奖励 ≥$10 credit，累计 30 次使用再奖 $20，一键部署按钮每带来一个付费用户奖 $5[11][4]。模板市场已有 50+ 预设服务（n8n、WordPress、Ghost、PostgreSQL 等）[12]。
- GitHub 组织开放（zeabur/zeabur 主仓 666 stars，MPL-2.0），文档和模板接受社区 PR[18]。

## 留存

- 成立 1.5 年时活跃/注册比约 40%（1.6-1.8 万活跃 / 4 万注册），付费转化约 4%[4]。托管型产品天然有迁移成本，跑着的数据库和域名就是留存。
- 反向压力测试正在进行：2026 年砍免费层和共享集群后，价格敏感用户公开讨论迁移方案；留下来的理由收敛为"多服务整合 + AI Agent 的 CLI/API/MCP 接口最顺手"——留存正在从"便宜"切换到"省时间"[12][14][15]。

## 转型

- 三次可见的转身：①部署工具 → 面向 Vibe Coder 的"AI 时代部署神器"（2024，随 AI 编程工具爆发）[6]；②工具 → "AI DevOps Engineer"对话式 Agent（2025）[1][16]；③向上做企业市场：Zeabur Atlas 更名 Nuphos（nuphos.ai），面向平台工程/SRE 团队的 AI 原生 DevOps 工作空间，"Nuphos is a Zeabur product"[16][17]。
- 公司结构同步升级：2025 年 1 月在美国特拉华注册 Zeabur Inc.，双总部台北 + 硅谷[9][1]。
- 值得注意的身份变化：早期是浙大双人联创（林沅霖 + 宇航，两人都拒了蚂蚁/阿里 offer）[2][5]，到 2025 年硅谷播客中林沅霖已以 Solo Founder 身份谈独立创办人的利弊[7]——联创变动未见公开说明。

## 如何保持小

- 规模轨迹：2 人联创 → 3 全职 + 1 实习生（2024 初）[2][5] → 约 5 人（2025 全员会议）[6 检索摘要] → 11 人（2026 官网），平均年龄 24 岁[9]。10 万用户 / 11 人 ≈ 每人服务近万用户。
- 保持小的机制：Discord 异步交流替代会议、Linear 管项目、GitHub 协作；客服靠 Discord 社区自助 + 互助；BD 靠模板奖励计划外包给开源生态；获客靠教程 SEO 和一键按钮，几乎不投广告[2][5][11][12]。
- 与巨头"合作不竞争"本身就是保持小的策略：不自建机房、不做 GPU 推理，只做体验层，资本开支极轻[2][1]。

## 开放问题（值得当面问创始人的）

1. 联创宇航后来去哪了？从两人联创到你在硅谷以 Solo Founder 自述，中间发生了什么，对"要不要联创"你现在的答案是什么？
2. "二房东"模式的真实毛利有多少？2026 年砍免费层/共享集群后，付费转化和流失数据分别怎么变？
3. 早期用户一半在中国大陆，如今重心转向台湾和北美——大陆市场是主动放弃还是被支付/合规逼走的？支付宝通道还留着吗？
4. 11 个人同时养 Zeabur 主产品和 Nuphos 企业线，是缝隙的自然延伸还是失焦的开始？资源怎么切？
5. 先拿奇绩（大陆体系）再拿 500 Global（美元体系）的台湾创业者极少见，两边条款、预期和身份敏感性怎么平衡？

## 来源

- [1] 链新闻 ABMedia：台灣 AI 新創 Zeabur 如何拿下 6400 萬融資 — https://abmedia.io/taiwan-startup-zeabur-500global
- [2] 硬地骇客 EP51《一个毕业设计拿下奇绩的投资｜对话 Zeabur 创始人》（2024.3）— https://hardhacker.com/podcasts/65ef09708e6f71a5b75bcf82 / https://www.xiaoyuzhoufm.com/episode/65ef09708e6f71a5b75bcf82
- [3] AIPostHub：台灣24歲天才創辦人！Zeabur 從畢業專題變身 AI 部署神器 — https://www.aiposthub.com/zeabur-taiwan-ai-deploy/
- [4] Meet 创业小聚：新創 Zeabur 用一鍵雲端部署，解決 AI 開發者的最後一哩路 — https://meet.bnext.com.tw/articles/view/52158
- [5] 少数派：新兴云端部署服务 Zeabur 创始团队都装了啥 — https://sspai.com/prime/story/zhuanglesha-230412
- [6] 数位时代 BusinessNext：乘上 Vibe Coding 特快車！Zeabur 光天使輪就有 6,400 萬元 — https://www.bnext.com.tw/article/84596/zeabur-closed-2m-seed-round
- [7] Podwise：獲得200萬美金投資！來矽谷一個月學到了什麼？ft. Zeabur 創辦人 — https://podwise.ai/dashboard/episodes/6544865
- [8] Product Hunt：Zeabur（2023.7.23 当日 #1，323 票）— https://www.producthunt.com/products/zeabur
- [9] Zeabur 官网 About（团队 11 人、Zeabur Inc. 特拉华）— https://zeabur.com/about
- [10] Zeabur 官网 Pricing — https://zeabur.com/pricing
- [11] Zeabur 文档：贡献奖励计划（模板/按钮 credit 奖励）— https://zeabur.com/docs/zh-CN/billing/reward
- [12] 恒远数位行销：Zeabur 評價：值得推薦的 PaaS 部署平台 — https://foreverwebs.com/blog/zeabur-review-deploy-platform
- [13] 火山引擎开发者社区：盘点 5 大免费平台（Zeabur 支持支付宝）— https://developer.volcengine.com/articles/7392435468396970034
- [14] Raymond Houch：Zeabur 漲價後值得用嗎？ — https://raymondhouch.com/lifehacker/digital-workflow/zeabur-vercel-cloudflare-deploy-comparison/
- [15] NodeLoc 论坛：zeabur 好像要开始没有免费的了（2026.3 changelog）— https://www.nodeloc.com/t/topic/78752
- [16] LinkedIn：Yuanlin Lin（"Founder @ Zeabur, now building nuphos.ai"；Build in Public #4: Zeabur Atlas is now Nuphos）— https://www.linkedin.com/in/yuanlinlin/
- [17] Nuphos 官网（"Nuphos is a Zeabur product"）— https://nuphos.ai
- [18] GitHub：zeabur/zeabur — https://github.com/zeabur/zeabur
- [19] 知乎：奇绩创坛 2023 春季创业营路演日（60 个项目）— https://zhuanlan.zhihu.com/p/635712662
- [20] 林沅霖个人博客 — https://yual.in/
- [21] COSCUP 2024 讲者页：林沅霖 — https://pretalx.coscup.org/coscup-2024/speaker/GRWZLM/
