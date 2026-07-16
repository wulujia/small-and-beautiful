# Tony Dinh（DevUtils / TypingMind）

> 给 LLM 做一个"自带 API key"的更好用第三方 UI，外加一组 macOS 小工具 ｜ typingmind.com / devutils.com / tonydinh.com ｜ X @tdinh_me（越南，Da Nang）｜ 全职年 2021（9 月 20 日辞职）｜ solo + 1 全职 + 数名 freelancer ｜ tag：AI wrapper / macOS 工具 / 多产品组合 / build in public ｜ TypingMind $130-160K/月（2025-10），B2B 经常性收入占比过半 [6]

## 缝隙切入点

- 核心方法不是"找市场"，而是"解决自己每天的烦"：DevUtils 把开发者高频小工具（JSON 格式化、时间戳转换等）打包成一个离线 macOS 应用，一次性 $9，两周做完，Hacker News 首发就有销售 [1]。
- 反面教材他自己先踩过：辞职前的第一个认真项目是一个 macOS 日志查看器，做了 6 个月，无人问津——之后他改为"小切口、快出货" [1][7]。
- TypingMind 的缝隙极小且具体：ChatGPT 官方 UI 打字慢、频繁掉登录、聊天记录难搜。他的原话（发布推文）："I was so annoyed by how ChatGPT slowly typed out the answers + kept logging me out every day, so I built a new UI on top of its API." [8]
- 辞职决定本身也是"缝隙思维"：月薪约 $9K 的工程师，存够 2 年生活费（在越南可以撑到 4 年），side project 有约 $500 MRR，就给自己买了一张全职试错的门票，2021-09-20 是最后一个工作日 [1]。

## 时机

- TypingMind 是教科书级的时机窗口案例：2023-03-01 OpenAI 发布 ChatGPT API；03-02 他注册 typingmind.com 并开始写原型；一个周末做完；03-06（周一）发推上线——距 API 发布仅 5 天 [2][3][8]。
- 收入按天翻倍：上线当天出首单，之后 $1K → $2K → $4K，03-10 累计 $10K；03-11 上 Product Hunt 拿下当日第一（902 票），再进约 $5K；7 天累计 $22K [2]。
- 他对窗口期的复盘：TypingMind 是"the first of its kind"（自带 API key 的替代 UI）；等 OpenAI 后来修好了掉登录、速度慢、不能搜索这些痛点时，先发优势已经转化为用户和心智，后来者复制不了那波关注 [3]。
- 反向的时机教训：Black Magic（Twitter 工具，2021-05 上线，峰值 $14K MRR）在 2023 年 Twitter API 涨价危机（传闻最低 $42K/月、只有一两周缓冲）中被迫贱卖——他收到过 $500K 的报价，最终为了速度以 $128K 卖给 Hypefury [1][7]。平台风险从此写进他的产品选择：TypingMind 刻意同时接 OpenAI、Anthropic、Google 多家模型对冲 [7]。

## 差异化

- "自带 API key"是定位也是成本结构：TypingMind 上线时是纯静态 web app，没有后端、没有数据库、没有登录系统，只有 license key 激活——用户的 key 存在本地，他的 infra 成本近乎为零 [3]。
- 一次性买断 vs ChatGPT Plus 订阅：官方收 $20/月，他卖一次性 license（$9 起，后涨到 $39），token 费用用户自付 [1][2]。
- 靠更新速度守住阵地：上线后 12 个月推了 171 次更新 [3]；2025 年加上多模型并行对话、Thinking Mode、知识库（RAG）等 [6]。
- 对团队客户主打"不锁定"："switch between any AI models anytime"——把 vendor lock-in 焦虑变成卖点 [来源：TypingMind 官网 About，见 14]。

## 第一批用户/冷启动

- TypingMind 冷启动没有投放、没有媒体，全靠他的 X 账号：上线时约 76K 粉丝，他自述"99% of the sales are from my Twitter reach"；每发一个新功能的推文，销量就跟着涨一波 [2]。
- Product Hunt 是第二级火箭：上线 5 天后上 PH，#1 Product of the Day，902 票，带来约 $5K 收入 [2]。
- 更早的产品也是同一套路：DevUtils 靠 Hacker News 首发拿到第一批付费用户 [1]；Xnapper（截图美化，2022-06 上线）拿过 PH 当日第一 [1]。

## 收入与定价

- 定价哲学一句话：没有持续成本就不收持续费用。DevUtils、Xnapper、TypingMind 初版都是一次性买断；Black Magic 和后来 TypingMind 的云同步/团队版因为有服务器和 API 成本才收订阅 [7]。
- TypingMind 混合模型：一次性 license（终身版）+ 订阅（Cloud Sync、Team/Custom 版、额度包）。他的原话："The revenue from the subscription sources could easily justify the costs for lifetime users." [3]
- 关键数字线：7 天 $22K（2023-03）[2] → 单产品月均 ~$30K（2023-10）[1] → 累计 $500K、订阅部分 $15K MRR（2024-02）[3] → 滚动 12 个月收入破 $1M，折合月均 ~$83K，此时一次性收入仍占约一半（2024-11，上线 20 个月）[5] → $130-160K/月，B2B 经常性收入占比超 50%（2025-10）[6]。
- 组合收入：2023-09 全组合 $45K/月，利润率约 90%，当时团队是 1 名全职 + 3 名 freelancer [1]。
- 两次卖产品也是收入的一部分：Black Magic $128K（2023-05）[1]；Xnapper $150K（$100K 首付 + $50K 分成，2024-03），卖价高于月收入是它 3.5 倍的 Black Magic——他自己都说"Unpredictable 😂" [4][12]。卖 Xnapper 时他绕开了 Acquire.com 的 4% 佣金（本案约 $6K），买家是发推公告后从 Twitter 上找到的，Escrow.com 手续费 $890 双方分摊 [4]。

## 内容与增长

- 粉丝-产品飞轮的完整数据线：2020-11 只有 100 粉 → 2021-05 700 → 2021-08 8K → 2022-02 28K → 2023-03 76K → 2023-07 破 100K [1][2][13]。
- 飞轮的起点是自用工具：Black Magic 最初就是他给自己涨粉做的"头像进度条"，Twitter 工具服务 Twitter 用户，产品本身就在 Twitter 上自传播 [1]。
- 他否认刻意经营"indie hacker 人设"：受众重叠是自然发生的，"built for myself"（为自己而做），只是把过程公开发出来 [7]。
- 付费投放对他基本无效：LinkedIn Ads 花 $2K 收入 $0（2024-04）[10]；后来又试投放，"I've spent $600 so far, resulting in only 2 conversions"，主要增长仍是口碑（2025-10）[6]。
- 增长动作外溢成新产品：为解决自己做 OG 图的麻烦做了 image.social（2024-04）[10]；2025-11 又在做 AI 时代的邮件客户端 Midday（"The way we use email has changed, but the email clients we use have not."）[11]。

## 转型

- 三次关键转身，节奏都是"信号出现→快速处置"：
  1. 平台危机→卖：Twitter API 涨价传闻出现后一两周内把 $14K MRR 的 Black Magic 以 $128K 卖掉，明确选择速度而非最高价 [7]。
  2. 注意力稀缺→修剪组合：TypingMind 到 $40K+/月后，把还有增长空间（他认为可做到 macOS 截图应用第一二名）但无暇顾及的 Xnapper 卖掉，"I decided to clean up my portfolio a bit" [4]。
  3. B2C 工具→B2B 平台：2024 年起主推 Team/Custom 版（企业内部 AI 平台），签下一单 3000 席位和数单 1000 席位的合同，为此花 $20K+ 做 SOC 2 Type II、HIPAA、GDPR 和安全审计，并开始招 sales closer [5]。到 2025-10，B2B 经常性收入已超月收入一半 [6]。

## 如何保持小

- 工作方式：平均每天约 4 小时，没有 deadline、没有例会，把健康和家庭放在前面 [1][5][7]。B2B 占比过半之后依然如此："I still only work ~4 hours a day"（2024-11）[5]。
- 团队刻意最小化：2023-09 是 1 名全职（客服+营销的 business assistant）+ 3 名 freelance 开发 [1][7]；宁可卖掉产品也不为维护它们扩编 [4]。
- 客服/infra/税务的 solo 解法：
  - infra：TypingMind 起步是无后端静态应用，license key 即全部"账号系统"，把运维压到接近零 [3]。
  - 客服：最早雇的全职就是处理支持和营销的助理，把最消耗心力的部分先外包给人 [7]。
  - 收款与税务：公司主体为越南的 Typing Technology Co. Ltd.，以 Paddle 为 merchant of record（Paddle 作为名义卖家处理全球销售税/增值税与开票）[9]；早期用 Lemon Squeezy，2024-04 因订阅分析太弱把订阅计费迁到 Stripe [3][10]。
  - 合规例外：唯一一次"像大公司一样花钱"是为 B2B 掏 $20K+ 买 SOC 2/HIPAA/GDPR 认证 [5]。
- 他也公开承认小的代价与张力："I feel like Typing Mind needs a lot more attention than I'm giving it right now, it needs a whole team to push this forward." [4] 但到 2025-10 他的结论是自由优先："with TypingMind making more than $1M a year, I now have an option to stop working entirely and live off my investment interest." [6]
- 保持小的另一面是持续开新坑而非做深单品：2025 年在带 Da Nang 的 Hacker Residency（10 名 indie hacker，2025-11 启动）[6]，同时做 Midday 邮件客户端 [11]。

## 开放问题（值得当面问本人的）

1. 辞职时只有约 $500 MRR，两年跑道的"失败线"具体画在哪里？如果 2023 年 3 月那个 API 窗口一直没出现，Plan B 是什么？
2. 做 TypingMind 那个周末，你怎么评估"OpenAI 自己两周内把 UI 修好"的风险？是判断了什么，还是纯粹因为成本只有一个周末所以不用判断？
3. 什么信号让你决定"卖掉"而不是"雇人维护"？Black Magic（被迫）和 Xnapper（主动）两次决策的框架有什么不同？现在会用同样的框架看 DevUtils 吗？
4. B2B 收入过半、客户里有 3000 席位的企业之后，每天 4 小时、没有例会的模式还能撑多久？你给"保持小"设的硬性红线是什么？
5. 越南主体 + Paddle MoR 这套结构，对其他新兴市场（收不了 Stripe/PayPal）的 solo 开发者，最大的坑在哪：税务申报、外汇回款，还是企业客户的合规尽调？

## 来源

1. Tony Dinh, "My solopreneur story: zero to $45K/mo in 2 years", Tony Dinh's Newsletter, 2023-09. https://news.tonydinh.com/p/my-solopreneur-story-zero-to-45kmo
2. Tony Dinh, "Making $22K in 7 days: the story", Tony Dinh's Newsletter, 2023-03. https://news.tonydinh.com/p/making-22k-in-7-days-the-story
3. Tony Dinh, "$500K milestone – my reflections after 1 year of building Typing Mind", Tony Dinh's Newsletter, 2024-02. https://news.tonydinh.com/p/500k-milestone-my-reflections-after
4. Tony Dinh, "Another 6-figure exit, and the future", Tony Dinh's Newsletter, 2024-03. https://news.tonydinh.com/p/another-6-figure-exit-and-the-future
5. Tony Dinh, "Nov 2024: My first million!", Tony Dinh's Newsletter, 2024-11. https://news.tonydinh.com/p/nov-2024-my-first-million
6. Tony Dinh, "Oct 2025 Updates: Code, Money, and Travel", Tony Dinh's Newsletter, 2025-10. https://news.tonydinh.com/p/oct-2025-updates-code-money-and-travel
7. Arvid Kahl, "Tony Dinh — Ups and Downs of an Indie Hacker Journey", The Bootstrapped Founder podcast. https://thebootstrappedfounder.com/tony-dinh-ups-and-downs-of-an-indie-hacker-journey/
8. @tdinh_me, TypingMind 发布推文, 2023-03-06. https://x.com/tdinh_me/status/1632631838866051074
9. TypingMind Terms of Service（主体 Typing Technology Co. Ltd.；merchant of record 为 Paddle）. https://docs.typingmind.com/security-and-compliance/terms-of-service
10. Tony Dinh, "April 2024 updates, new product!", Tony Dinh's Newsletter, 2024-04. https://news.tonydinh.com/p/april-2024-updates-new-product
11. Tony Dinh, "I'm building a new email client", Tony Dinh's Newsletter, 2025-11. https://news.tonydinh.com/p/im-building-a-new-email-client
12. @tdinh_me, Xnapper 出售推文（"Funny but I end up selling Xnapper at a higher amount than Black Magic"）, 2024-03. https://x.com/tdinh_me/status/1765546696799600652
13. @tdinh_me, 100K 粉丝 / Twitter 分成推文, 2023-07. https://x.com/tdinh_me/status/1679702389476196352
14. TypingMind Custom, "About Us". https://custom.typingmind.com/about-us
