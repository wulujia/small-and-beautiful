# Resend（Zeno Rocha）

> 在 SendGrid/Mailgun 统治十几年的邮件 API 市场，用"开发者体验 + 设计品味"重新切开一条缝 ｜ resend.com ｜ Zeno Rocha & Bu Kinoshita ｜ 2023（2022-08 起步为 side project）｜ 28 人（2025-12）[1][8] ｜ 开发者工具 / 邮件基础设施 / 开源引流 ｜ 2025 年营收增长 5 倍（绝对值未公开；第三方估 2024 年约 $5M ARR）[8][17] ｜ ⚠️边界样本：2024-12 a16z 领投 $18M A 轮 [2]

## 缝隙切入点

- 表面上这是个"已经赢了"的市场：SendGrid、Mailgun、Postmark、SparkPost 全部诞生于 2009-2010 年前后。但 Zeno 的判断是：这批玩家全都被收购了，卖给了企业销售逻辑，十几年没人为开发者重新做一遍——"there's no player that is just coming up and trying to really rethink email in 2023"[4]。
- Launch HN 帖子里他把缝隙说得更直白："Nobody is building an exceptional developer experience. Nobody is trying to innovate."[5]
- 缝隙来自亲身痛点：Zeno 在 Liferay 当 CPO、在 WorkOS 当 VP of Developer Experience 时，反复被同一个问题折磨——事务性邮件进垃圾箱、邮件工具是为营销人员而非开发者设计的 [1][5]。
- 他自己承认这种切入需要一点无知的勇气："you need to be that naive to go and say 'Let me take on SendGrid.'"[4]

## 时机

- 2022-2023 年的具体窗口：前端一代（React 开发者）已经成为购买决策者，但邮件模板还停留在 HTML table 和 Handlebars 时代 [5]；Stripe/Vercel 已经验证了"开发者体验本身就是产品"的打法，Resend 的三步计划公开对标 Vercel 用 Next.js 开源引流的路径 [4]。
- a16z 投资备忘录给出的宏观时机：事务性邮件和营销邮件的边界在消失（"the line between transactional and marketing emails has blurred"），AI 驱动的程序化发信量暴涨，需要新一代基础设施 [3]。
- 个人时机：拿到公民身份、刚当爸爸、在 WorkOS 看到小团队也能做出差异化产品——"I'm going to work crazy hours...I might as well do that for myself instead of someone else."[4]

## 差异化

- 核心赌注是 DX：用 React 写邮件模板（react.email），前端团队"can re-use everything they already know from React land"[5]；注册后立刻能发第一封邮件，而不是填表单等两天审批 [4]；多区域发送（US/EU/LATAM）降低 time-to-inbox；webhook 事件流做可观测性 [5]。
- 设计品味是显性武器：官网、文档、dashboard 全部按消费级产品标准打磨。Evil Martians 播客总结他的北极星是 "building work so good your heroes want to copy it"[6]。方法论是"不牺牲质量也不牺牲速度，狠砍范围（ruthlessly cut scope）"[4][6]。
- 差异化的另一面要如实记录：Launch HN 上的质疑相当尖锐——React 编译后还是那些 HTML 标签，解决不了送达率；有人指出底层疑似 AWS SES（"Custom Email feature reveals SES"）；Postmark 用户反驳"Postmark has great developer experience"[5]。Zeno 的回应是承认送达率才是根本，私测 6 个月大量时间花在反欺诈上，还去参加了办了 20 年的反滥用行业会议 [4][5]。
- 他给可靠性排的优先级："We can have the most beautiful product in the world, but if it's not online or if the emails are going to spam, then it's all for nothing."[7]

## 第一批用户/冷启动

- 第一个付费用户的故事：2022 年 9 月，MVP 刚能跑，一个在别家创业公司的朋友直接用到了生产环境。两人发给他一个 $10 的付款链接测试意愿——他真付了。就这一单给了他们申请 YC 的信心 [1]。
- 开源先行的"总体规划"只有三行："Build an open source project around email. Establish ourselves as email experts. And then build a SaaS product for it."[4] 2022 年 12 月先发 react.email，2023 年 1 月才宣布 Resend——Zeno 称之为 "Jab, Jab, Right Hook"：give, give, give, then ask [6]。
- React Email 的文档故意教用户怎么搭配 SendGrid、Postmark 等竞品使用——先建立信任，再收转化 [6]。
- Resend 公告推文超过 100 万次浏览 [1]。YC 期间全程 waitlist：YC launch 时（上线 7 周）6,469 人排队 [19]，2023 年 6 月公开发布前累计到 20,000 人 [6]。
- 精准打 YC 生态做种子用户：15 个月时已有 120+ 家 YC 公司在用 [4]。2023 年 3 月第一次 Launch Week 一周发 7 个功能 [1]。

## 收入与定价

- 定价对开发者极简：免费档 3,000 封/月（每天上限 100 封）；Pro $20/月 5 万封起；Scale $90-$1,150/月；营销邮件按联系人数收费（$40-$650/月），发送量不限；独立 IP $30/月，含自动预热 [9]。
- 付费里程碑：2023-12 达到 1,000 个付费客户 [1]；上线 15 个月（2024 年春）1,400 个付费客户、约 10 万用户 [4]；a16z 投资时 3,000+ 客户，包括 Warner Brothers、Decathlon、Supabase、Raycast、Braintrust [2][3]。
- 营收绝对值未公开。第三方 Getlatka 估 2024 年约 $5M ARR（仅供参考）[17]；官方口径是 2025 年营收增长 5 倍 [8]。

## 内容与增长

- 增长引擎就是开源：React Email 从 A 轮时的 30 万次/周 npm 下载、14k stars、130+ 贡献者 [2]，涨到 2025 年的 140 万次/周 [8]，再到 6.0 版本时的 200 万次/周、196 位贡献者 [20]。
- Zeno 的个人品牌是冷启动的隐形资产，且早在 Resend 之前就已变现验证：2013 年做的免费主题 Dracula，2020 年 2 月推出 $49 的 Dracula PRO，3 天卖了 $5,428.91 [12]，2021 年 3 月累计 $111,465.77（2,043 份）[13]，2022 年 9 月突破 $250,368.68，月均 $8,076.40 [11]。他还写过《14 Habits of Highly Productive Developers》（电子书 $9.99/精装/有声书）[14]，讲过 110+ 场技术大会，22 岁时是 GitHub 全球最活跃的 20 个用户之一 [10]。
- 节奏感极强的内容机器：仅 2025 年就有 90 篇博客、45 支视频、28 篇 changelog、9 场大会、2 次 Launch Week [8]。

## 社区

- React Email 有 196 位开源贡献者、17k stars（2025 年底）[8][20]，社区本身成了获客渠道和信任背书。
- 内部机制反哺社区口碑：dogfooding 塑造产品、RFC 流程、每周一天无会议日，都写进公开的 handbook [18]。

## 留存

- 把客服当产品做而不是成本中心："great support is a core part of what makes Resend valuable"[2]。2025 年数据：帮助 82,416 名用户，首次响应中位数 2 小时 45 分，90% 紧急工单 47 分钟内响应 [8]。
- 留存的底层是送达率和可靠性——A 轮资金三个投向里两个是可靠性和送达率洞察 [2]。

## 转型

- 不是转型，是从"一根 API"长成通信平台：2024 年 4 月 Launch Week 推出 Audiences 和 Broadcasts，切入营销邮件，把事务性与营销统一 [7]；2025 年连续收购两家公司——Mergent（后台任务）和 Briefer（YC S23，数据基础设施）[15][16]；随后推出 new.email（公开发布前一个月 waitlist 即超 14,386 人）[21]，并面向 AI agent 做 Email Skills 和 CLI [1]。使命定为 "Resend exists to make human communication easier."[2]
- 规模刻度：2025 年用户从 24.9 万涨到 100 万，2026 年 7 月官宣破百万用户，日发送量达数千万封 [8]。

## 如何保持小

- 极端的人效：2024 年 4 月，6 个人服务 8-10 万开发者 [4][7]；到破百万用户时也只有 28 人 [8]。"Every minute we spend on infrastructure is a minute we're not spending on building the best email product in the world."[7]
- 种子轮刻意"反 VC"：2023 年 4 月的 $3M 种子轮拒绝了 a16z、Sequoia 的兴趣，只从 28 个天使（含 Guillermo Rauch、Figma 的 Dylan Field）拿钱，限制单张支票金额，把稀释控制在约 10%[4]。
- 顶住 VC 让团队回办公室的压力，坚持远程优先，理由是保住和家人的 "micro moments"[4]。
- ⚠️但边界就在这里：2024 年 12 月还是接了 a16z 领投的 $18M A 轮（跟投：Ali Rowghani、前 Mailchimp CTO Eric Muntz、YC、Basecase 等）[2]。种子轮的克制与 A 轮的选择之间的张力，是本案例最值得当面追问的部分。

## 开放问题（值得当面问创始人的）

1. 2023 年种子轮你刻意只拿 28 个天使的钱、把稀释压在 10%，18 个月后却接了 a16z 的 $18M——中间哪个具体时刻让你改了主意？邮件基础设施是不是注定无法 bootstrap？
2. 拿了 a16z 之后，"6 个人服务 10 万用户"的那种小而美气质，哪些保住了、哪些被增长预期挤掉了？有没有 board 要求和你的节奏冲突的具体例子？
3. Dracula 月均 $8,000 被动收入加上书的版税，你完全可以过 indie hacker 的日子。决定 all-in Resend 的那一刻，你放弃的最大的东西是什么？
4. React Email 文档教用户配合 SendGrid/Postmark 使用——当时内部有没有人反对"给竞品导流"？从 20,000 人 waitlist 到付费客户，"give give give then ask"的实际转化率是多少？
5. Launch HN 上最扎的批评是"你们只是 SES wrapper"。三年过去，发送基础设施自建到了什么程度？送达率上外人看不见的成本有多大？

## 来源

1. Resend Handbook: How we got here — https://resend.com/handbook/company/how-we-got-here
2. Resend Blog: Resend raises $18M Series A（2024-12-04）— https://resend.com/blog/series-a
3. a16z: Investing in Resend — https://a16z.com/announcement/investing-in-resend/
4. The Changelog Interviews #585: Getting to Resend with Zeno Rocha（2024）— https://changelog.com/podcast/585
5. Launch HN: Resend (YC W23) – Email API for developers using React（2023-06）— https://news.ycombinator.com/item?id=36309120
6. Evil Martians Podcast: Zeno Rocha, founder of Resend — https://evilmartians.com/events/podcast-zeno-rocha-resend
7. Railway Blog: How Resend is Building a New Kind of Email Platform（2024-04）— https://blog.railway.com/p/zeno-rocha-resend
8. Resend Blog: 1,000,000 users（2026-07）— https://resend.com/blog/1-million-users
9. Resend Pricing — https://resend.com/pricing
10. Zeno Rocha: About — https://zenorocha.com/about
11. Zeno Rocha LinkedIn：side project 收入破 $250,368.68（2022-09）— https://www.linkedin.com/posts/zenorocha_a-side-project-of-mine-just-crossed-25036868-activity-6970755736679186433-iYf6
12. Zeno Rocha (Medium): I made $5,428.91 in 3 days with a side project（2020）— https://medium.com/@zenorocha/i-made-5-428-91-in-3-days-with-a-side-project-2116f4121e86
13. Rob O'Leary: Making money from open source（2021-03，Dracula PRO 累计 $111,465.77）— https://www.roboleary.net/2021/03/03/making-money-open-source
14. 14 Habits of Highly Productive Developers 官网 — https://14habits.com/
15. Resend Blog: Resend acquires Mergent（2025）— https://resend.com/blog/resend-acquires-mergent
16. Resend Blog: Resend acquires Briefer（2025）— https://resend.com/blog/resend-acquires-briefer
17. Getlatka: Resend 营收估算（第三方估计，非官方）— https://getlatka.com/companies/resend.com
18. Resend Handbook — https://resend.com/handbook
19. Launch YC: Resend – Email API for developers — https://www.ycombinator.com/launches/I6M-resend-email-api-for-developers
20. Resend Blog: React Email 6.0 — https://resend.com/blog/react-email-6
21. Resend Blog: new.email Public Launch — https://resend.com/blog/new-email-public-launch
