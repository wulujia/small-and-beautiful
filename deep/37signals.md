# 37signals（Basecamp / HEY）

> 给被"甘特图式"复杂项目管理软件折磨的小团队，做一个只管沟通和待办的简单工具 ｜ 37signals.com ｜ Jason Fried & David Heinemeier Hansson（DHH）｜ 1999（芝加哥，前身为网页设计工作室）｜ 约 60 人（2024 年初峰值 77 人 [22]，2025 年约 62 人 [25]）｜ pure-bootstrap / 反 VC 精神图腾 / 远程 ｜ 营收不公开，第三方估算 2024 年约 $80.8M ARR [27]（可信度一般）；官方口径"连续 27 年盈利、零负债、私有" [19]

## 缝隙切入点

1999 年成立时是三人网页设计公司（Jason Fried、Carlos Segura、Ernest Kim），名字来自天文学家 Paul Horowitz 识别出的 37 个疑似地外无线电信号 [2]。Basecamp 不是"找到的商机"，是自用工具外溢：设计业务变多后"we found ourselves increasingly disorganized"，靠邮件管项目管不动了，于是自己造了个只有三样东西的工具——留言板、待办清单、里程碑。"This was all the first version of Basecamp did. It's all we needed and nothing we didn't."[1] 缝隙的本质：当时市场上的项目管理软件都在做规划（甘特图、资源调度），他们赌项目管理的真问题是沟通，不是规划 [1]。客户用过之后主动问"能不能也给我们用"——"Once you hear that enough, a lightbulb turns on and you say 'Maybe we've got something here'."[1]

## 时机

- 2004 年 2 月 Basecamp 上线 [1]：SaaS 概念尚未普及，浏览器软件+月订阅在当时是异类，项目管理赛道几乎没有轻量级竞品——空地。
- 同年 DHH 把开发 Basecamp 时抽出的框架开源，即 Ruby on Rails [2]。Rails 后来养出 GitHub、Shopify、Airbnb 一整代公司，等于 37signals 免费获得了此后二十年的全球开发者好感和雇主品牌——这是最不可复制的时机红利。
- 2006 年贝索斯通过个人投资机构 Bezos Expeditions 买下少数股权 [2]，公司层面从未做过 VC 轮融资。

## 差异化

产品差异化=观点差异化，三条主线贯穿 20 年：

- **少即是多**：Basecamp 从第一版起靠"故意做少"对抗功能竞赛，对手比功能数量，它比简单 [1][19]。
- **平价定价结构**（见下节）：全行业按人头收费，它敢收固定价。
- **公司本身是产品**：37signals.com 首页挂着 37 条原则当宣言——"An obligation to independence"、"Small teams"、"Work isn't war"、"Pay people, not addresses"、"Companies aren't families" [24]。反 VC 立场在 DHH 2015 年的《RECONSIDER》里说到底："Nobody these days is content to merely put their dent in the universe. No, they have to f*&%ing own the universe." 以及给创业者的反鸡汤："Curb your ambition. Live happily ever after."[17]
- HEY（2020）是同一逻辑打电子邮件：对抗 Gmail 的免费+广告+读隐私模式，收 $99/年 [9]。DHH 把商业模式浓缩成一句话："Monetize by charging money. That's it. That's the business plan."[11]

## 第一批用户/冷启动

- 及格线定得极低：上线前商定"一年后做到 $5,000/月（约 $60K 年收入）就算成"。结果"Turns out, we hit that number in about 6 weeks."[1]
- 冷启动靠的是产品之前就存在的受众：设计博客 Signal v. Noise 积累的读者+设计客户口碑。Rework 后来把这条方法论写成明文：先教东西、攒受众，再卖产品 [15]。
- HEY 的冷启动则展示了 20 年受众复利+争议营销的极端效果：2020 年 6 月上线，"300,000 users signed up to try our service in three weeks instead of our forecast of 30,000 in six months"——超预测 60 倍 [4]。上线半年多"we've already signed up many tens of thousands of paying customers"，成为公司史上增长最快的产品 [11][26]。其中苹果因 HEY 拒绝内购分成 30% 而威胁下架、DHH 公开开战（后以"免费临时账号"折中过审，并联合发起 Coalition for App Fairness）[9][10]，这场架本身就是最大的免费分发；2024 年 1 月 HEY Calendar 上架再被拒一轮，剧情重演 [29]。

## 收入与定价

- **Basecamp**：$15/人/月起；旗舰是 Pro Unlimited——$299/月（年付）不限人数 [19]。全行业按 seat 收费时的反向定价：20 人团队合 $15/人，50 人合 $6/人，人越多越便宜，天然抗流失、抗采购砍价 [19]。
- **HEY**：$99/年（约 $8.25/月）个人，团队 $12/人/月 [9][11]。
- **ONCE / Campfire**：$299 一次性买断、自托管、不限人数（2024 年 1 月）[8]。
- 盈利口径：官网自述"27 profitable, financially responsible years in business. Zero debt, privately held, and built to stay, not exit"[19]。利润具体数字不公开；据 Fried 披露的 2024 年分红信息推算，公司每年拿出利润的 10% 按工龄分给员工，2024 年 20 人拿到六位数分红、约 60 人拿到五位数，人均营收超 $100 万 [22]（注意：这是第三方基于 Fried 公开发言的估算）。
- 成本端最著名的决定：**退云自建**。2022 年 10 月 DHH 发《Why we're leaving the cloud》，当时仅 AWS 的数据库+搜索服务就"over half a million dollars per year"，核心论断："Renting computers is (mostly) a bad deal for medium-sized companies like ours with stable growth."[4] 年云支出 $3.2M，买了约 $700K 的戴尔服务器，2023 年当年回本，2024 年云账单降到 $1.3M（年省约 $200 万）[5][6]。2025 年夏 S3 合约到期后连 10PB 存储（年费超 $100 万）也迁到自有 Pure Storage（18PB），五年总节省预计"over ten million dollars"，且运维团队规模没有增加 [5]。DHH 的建议："As soon as the cloud bills start to become substantial…you owe it to yourself…to at least do the math."[5]

## 内容与增长

37signals 是"内容先于产品"的教科书，增长引擎就是写作：

- Signal v. Noise 博客（1999 年起）→ 免费电子书 Getting Real（2006）→ **Rework**（2010）："It was our first big-publisher book, and it hit the New York Times bestseller list right out the gate"，头两年卖 20 万册，累计超 100 万册、40 多种语言 [15]（中文版《重来》系列在中国创业者中影响巨大）。
- It Doesn't Have to Be Crazy at Work（2018）把方法论定名"the calm company"：8 小时工作日、40 小时周、不加班不熬夜 [24]。
- 方法论开源：Shape Up（6 周开发周期，免费在线书，对应官网原则"Shape Up every six"[24]）。
- REWORK 官方播客持续输出 [24]。
- 争议即分发：与苹果开战 [10]、退云宣言 [4]、每一次都是头条。DHH 个人博客 world.hey.com/dhh 本身就是行业媒体。

## 社区

严格说 37signals 没做过"用户社区运营"，它的社区是**开发者生态**：Rails 开源社区 20 年 [2]；ONCE 商业实验失败后把 Campfire、Writebook、Fizzy 全部开源（宽松许可），DHH："That worked! Tons of people have been running these apps on their own servers, contributing code back, and learning how we build real production applications."[7]（注：Fizzy 用的 O'Saasy 许可证是否算"开源"在社区有争议 [21]。）

## 留存

- 制度化的"永不下线"承诺：**Until the end of the internet**——产品进入 legacy 阶段后老客户可以永远用下去，2004 年的初代 Basecamp Classic 至今还在为老客户运行 [20]。
- 平价定价的留存逻辑：$299/月不限人数意味着客户团队越大、单位成本越低，迁移动机随规模递减 [19]。
- Fried 的说法："We're here for them, 23 years and running."（basecamp.com/about）

## 转型

二十多年里四次大转向，每次都反行业直觉：

1. **2005-2006 砍掉咨询业务**：Basecamp 上线一年左右收入超过设计业务，果断从服务转产品 [2]。
2. **2014 一个产品**：公司改名 Basecamp，43 名员工全部聚焦单一产品（当时称有 1500 万用户），Highrise/Backpack/Campfire 或分拆或停止接新客 [3]——在"多产品矩阵"教条盛行时主动做减法。
3. **2020-2022 重新多产品**：HEY 成功后，2022 年 5 月改回 37signals 之名，理由是不再只有 Basecamp 一个产品 [23][2]。
4. **2024 ONCE 买断制实验及其失败**：宣称回到"买一次、永远拥有、自己部署"的老式软件模式，Campfire 卖 $299 [8]。18 个月后 DHH 公开认输："That didn't work. Sure, we recouped the investment on Campfire, our chat app, but that was it."以及"You gotta listen when the market tells you what it wants! And it didn't seem to want to pay for self-hosted web apps in a one-off way."于是全部转开源 [7]。——失败被处理成公开的、低成本的、可回收的实验（代码沉淀为开源影响力），这是小公司做新尝试的范本。

## 如何保持小

- **不设目标**：Fried 2016 年名文《I've never had a goal》："a goal is something that goes away when you hit it…I just don't function in steps like that."[16] 公司不做年度增长目标，只求"每年比去年利润多一点"。
- **薄公司、厚产品**：Fried 的"thin business"论——"A high performance business is a thin shell around a thick product"，成本压低才有犯错和留在牌桌上的自由 [25]。
- **结构性抗膨胀**：6 周周期的 Shape Up 限制并行项目数 [24]；薪酬"Pay people, not addresses"——全员按旧金山市场前 10% 支付、不看居住地，且设 $73,500 薪酬下限 [18][24]；5 月 1 日到 8 月 31 日全员每周 4 天 32 小时；每 3 年一次 6 周带薪长假 [18]。高薪+高福利+不扩编，替代"用人数换产出"。
- **代价也真实——2021 年风波**：起因是内部清算一份留存多年的"搞笑客户名单"（含亚非裔姓名）引发的 DEI 争论，Fried 于 2021 年 4 月 26 日发文禁止在公司平台讨论社会政治议题、解散 DEI 委员会，并提供最高 6 个月工资的买断 [12][13]。57 名员工中约 20 人（约 1/3）离职，包括设计、市场、客服负责人 [12][14]。公司能扛住 1/3 员工离职而产品照常运转，本身证明了"小而利润厚"的冗余度——但这也是创始人绝对控制权的代价样本：没有董事会能制衡两位创始人，文化风险全押在他们的判断力上。

## 可学 vs 幸存者特权

**可学的：**
- 用自己的真问题做产品，上线前定一条极低的"及格线"（$5K/月），达标才加注 [1]。
- 反向定价做差异化（固定价 vs 按人头）[19]。
- 先攒受众再做产品，"教"是最便宜的获客 [15]。
- 公开算账的文化：退云省多少钱、ONCE 怎么失败的，全部原文公开 [5][7]——诚实本身成为品牌资产和分发。
- 薄公司结构 + 不设增长目标 = 可以无限期玩下去 [16][25]。

**幸存者特权（不要直接模仿）：**
- Rails 光环：DHH 写出了行业基础设施，换来 20 年免费的开发者好感、媒体关注和招聘优势 [2]——绝大多数小团队没有这张牌。
- 2004 年的空地：SaaS 竞争真空期的先发身位，今天任何品类都不存在。
- HEY 三周 30 万注册 [4] 是"20 年受众 × 苹果争议头条"的共振，不是产品冷启动的常态。
- 贝索斯 2006 年的钱进了创始人口袋 [2]，"永不融资"的姿态背后有个人财务安全垫。
- 两位创始人都是顶级写作者，"内容增长"对他们是零边际成本，对普通团队是全职投入。
- 1/3 员工离职还能照常出货 [14]，前提是产品已成熟 20 年、利润极厚——早期公司照抄这种强硬治理方式会直接死掉。

## 开放问题（值得当面问创始人的）

1. 2021 年风波四年后复盘：那次事件真实的代价和收益各是什么？如果重来一次，还会用同样的方式（一刀切禁令+买断）处理吗？
2. ONCE 失败的归因：败在 $299 的定价、自托管的部署门槛，还是"买断制"这个模式本身？如果再做一次实验，你们会只改哪一个变量？
3. 幸存者特权的自我评估：如果没有 Rails 的光环和 Signal v. Noise 的受众，2004 年的 Basecamp、2020 年的 HEY 还能成吗？一个普通小团队该复制你们的哪部分、坚决不该复制哪部分？
4. 贝索斯那笔钱在心理层面到底值多少？它是否让"永不融资"的立场，说出来比实践起来更容易？
5. 终局问题：你们说"built to stay, not exit"[19]，但公司 60 人、两位创始人都年过五十——20 年后的 37signals 是什么？有接班计划，还是接受"最后一个客户关灯"？

## 来源

1. Jason Fried, "Basecamp: The origin story", Medium — https://medium.com/@jasonfried/basecamp-the-origin-story-f509fdd725f8
2. Wikipedia: 37signals — https://en.wikipedia.org/wiki/37signals
3. Forbes, "37Signals No More - Changes Name To Basecamp And Drops All Products But Its Namesake", 2014-02-05 — https://www.forbes.com/sites/benkepes/2014/02/05/37signals-no-more-changes-name-to-basecamp-and-drops-all-products-but-its-namesake/
4. DHH, "Why we're leaving the cloud", 2022-10-19 — https://world.hey.com/dhh/why-we-re-leaving-the-cloud-654b47e0
5. DHH, "Our cloud-exit savings will now top ten million over five years", 2024 — https://world.hey.com/dhh/our-cloud-exit-savings-will-now-top-ten-million-over-five-years-c7d9b5bd
6. Datacenter Dynamics, "37signals claims it saved almost $2m last year from cloud repatriation" — https://www.datacenterdynamics.com/en/news/37signals-claims-it-saved-almost-2m-last-year-from-cloud-repatriation/
7. DHH, "ONCE (Again)" — https://world.hey.com/dhh/once-again-3e99f755
8. 37signals on X: "ONCE/Campfire is now available! …one-time price of $299", 2024-02 — https://x.com/37signals/status/1753133521378660474
9. TechCrunch, "Basecamp launches Hey, a hosted email service for neat freaks", 2020-06-16 — https://techcrunch.com/2020/06/16/basecamp-launches-hey-a-hosted-email-service-for-neat-freaks/
10. TechCrunch, "Apple approves Hey bug fix update after Basecamp agrees to tweak app…", 2020-06-22 — https://techcrunch.com/2020/06/22/apple-approves-hey-bug-fix-update-after-basecamp-agrees-to-tweak-app-at-center-of-store-policy-spat/
11. DHH, "We will monetize by charging money", 2021-02-24 — https://world.hey.com/dhh/we-will-monetize-by-charging-money-a1f71413
12. TechCrunch, "Basecamp sees mass employee exodus after CEO bans political discussions", 2021-04-30 — https://techcrunch.com/2021/04/30/basecamp-employees-quit-ceo-letter/
13. NPR, "Basecamp Blowup: Banning Politics At Work Prompts Over A Dozen Employees To Quit", 2021-05-07 — https://www.npr.org/2021/05/07/994812274/basecamp-blowup-banning-politics-at-work-prompts-over-a-dozen-employees-to-quit
14. Gizmodo, "One-Third of Basecamp Employees Have Reportedly Quit Following New Policy on Speech", 2021-05 — https://gizmodo.com/one-third-of-basecamp-employees-have-reportedly-quit-fo-1846801378
15. DHH, "Celebrating a million copies of REWORK" — https://world.hey.com/dhh/celebrating-a-million-copies-of-rework-9d5eb543
16. Jason Fried, "I've never had a goal", 2016 — https://medium.com/signal-v-noise/ive-never-had-a-goal-c89219aedddf
17. DHH, "RECONSIDER", 2015 — https://medium.com/signal-v-noise/reconsider-41adf356857f
18. 37signals Employee Handbook: Benefits & Perks — https://basecamp.com/handbook/benefits-and-perks
19. Basecamp Pricing（含 "27 profitable years / zero debt / built to stay, not exit" 口径） — https://basecamp.com/pricing
20. 37signals, "Until the end of the internet" — https://37signals.com/policies/until-the-end-of-the-internet
21. DHH, "Fizzy is our fun, modern take on Kanban (and we made it open source!)", 2025-12 — https://world.hey.com/dhh/fizzy-is-our-fun-modern-take-on-kanban-and-we-made-it-open-source-54ac41b6
22. Zhimin Zhan, "37signals' Remarkable Profitability and Unique Employee Profit Sharing Model", Medium（基于 Fried 公开披露的第三方估算） — https://zhiminzhan.medium.com/37signals-remarkable-profitability-and-unique-employee-profit-sharing-model-06dd71f7c6aa
23. Jason Fried, "37signals: Hello again", 2022-05 — https://world.hey.com/jason/37signals-hello-again-117eae60
24. 37signals.com 首页（37 条原则宣言） — https://37signals.com/
25. coachparin, "Jason Fried - The Thin Business", 2025 — https://coachparin.substack.com/p/jason-fried-the-thin-business
26. DHH on X, 2021-06-03："HEY has signed up far more customers, far faster, than any new product we've ever launched before." — https://x.com/dhh/status/1400502770332012545
27. Getlatka（第三方营收估算，hey.com/37signals LLC） — https://getlatka.com/companies/hey.com
28. saas.group podcast, "Building Campfire with Jason Fried @37signals/@Once.com" — https://saas.group/podcasts/saas-unbound-interview-jason-fried-37signals-once-com/
29. Daring Fireball, "Heyja Vu: App Store Rejects 37signals's New Hey Calendar App", 2024-01 — https://daringfireball.net/2024/01/heyja_vu_hey_cal
