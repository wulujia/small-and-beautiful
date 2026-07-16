# Josh Pigford（Baremetrics）× Tyler Tringas（Storemapper → Calm Company Fund）

> 双人对照档案：两位都把 bootstrap SaaS 卖掉、然后走向完全相反方向的创始人 ｜ Pigford：Stripe 订阅分析工具 Baremetrics，2013 年创立，2020-11 以 $400 万现金卖给 PE 公司 Xenon Partners，本人到手 $370 万 [1][3]；此后走"连续 Maker"路线（Maybe 五年三死、2026 年清算，今天同时做 9 个小项目）[16][21][22] ｜ Tringas：Shopify 商店定位插件 Storemapper，2012 年在一趟航班上写出 v1，2017-10 卖给 SureSwift Capital；此后转身做"给 bootstrapper 的资本"（Earnest Capital → Calm Company Fund，77 家、约 $2000 万 AUM），2024 年底宣布退出早期投资，2025 年去布鲁克林开攀岩馆 [7][10][12][13] ｜ 两人靠同一块公开仪表盘结缘：Storemapper 的公开收入数据就跑在 Baremetrics 上，是 Josh 亲自拉 Tyler 入伙 Open Startups 的 [4][7] ｜ tag：透明增长 / 卖出复盘 / micro-SaaS / 退出后的路线分叉

## 缝隙切入点

- Pigford 的缝隙是"Stripe 有交易、没报表"：2013 年他运营自己的调查工具 PopSurvey / Temper，苦于手工从 Stripe 数据里算 MRR、churn 这些 SaaS 指标，容易错还费时间，于是给自己做了一个 Stripe 订阅分析面板——前后只花了 7 个工作日（摊在一个月里），启动成本 $0，2013 年 11 月上线即收费 [3][25][26]。
- 这不是他第一个项目，而是第 50 个左右：从 2003 年的链接目录站开始，他以壳公司 Sabotage Media 名义连开了十几年项目（TrackThePack、Deck Foundry、PopSurvey、Temper……），Baremetrics 是其中终于长大的那个 [25]。
- Tringas 的缝隙更小："给网店加一张门店地图"。2012 年，他在旧金山飞布宜诺斯艾利斯的一趟约 30 小时航程里写出 Storemapper 第一版 [7][10]。他后来给这类生意起了名字并下了定义——micro-SaaS："A SaaS business targeting a niche market, run by one person or a small team, with small costs, a narrow focus, a small but dedicated user base and no outside funding."（服务利基市场、一人或小团队运营、低成本、窄焦点、无外部融资）[8]。
- Tyler 是先撞了南墙才找到缝的：此前他做过一个 VC 路线的清洁能源创业（太阳能金融），结果是负债、健康受损、亲密关系受伤。他由此得出反 VC 结论：多数成功创始人在冒险之前先有了财务安全垫，而 micro-SaaS 就是普通人造安全垫的方式 [8]。

## 时机

- Baremetrics 吃到的是"Stripe 生态早期红利"：2013 年 Stripe 自己不提供订阅分析，第一波 Stripe SaaS 创业者全都在用表格手算。窗口后来如何关闭也很清楚：Stripe 推出原生报表、ChartMogul 等对手成熟，Baremetrics 在 2017 年底到 2019 年初卡在 $9-10 万 MRR 整整 16 个月 [2]。
- Storemapper 吃到的是"Shopify App Store 早期空位"：它长期是应用商店里唯一的 store locator，每个搜这个功能的商家都会撞到它——分发问题被平台顺手解决了 [10]。
- 两人后来对"窗口"的判断都延伸到了 AI。Tyler 在 2024 年底关停基金的信里写："AI-assisted software development is a massive boost to the Peace Dividend of the SaaS Wars and will make the last wave of 'Micro-SaaS' pale in comparison."（AI 辅助开发会让上一波 micro-SaaS 相形见绌）——并承认这也意味着solo 创始人可以直接跳过 Calm Fund 原本要投的那个资本阶段 [13]。Josh 则用行动投票：2026 年他同时维护 9 个项目，日常靠 Claude Code / Cursor 这类工具 [22][27]。

## 差异化

- 两个产品都是"一句话说得清"的单点工具：一个只做 Stripe 订阅指标的仪表盘，一个只做门店地图。差异化不靠功能堆叠，靠的是把一件小事做到即装即用。
- Baremetrics 真正的差异化动作是把"真数据"当 demo：Josh 懒得造假数据给潜在客户演示，索性把自己公司的实时收入仪表盘公开当 live demo——透明的起点是省事，不是理念 [5]。
- Storemapper 的差异化是低流失而非高客单：Tyler 拆自家数据的结论是月流失仅 1-1.5%（对比当时 Baremetrics 自己是 5.5-10%、ConvertKit 15-20%），他的原话："Even though we don't extract a lot of cash from each user, they just never leave."（我们从每个用户身上赚得不多，但他们从不离开）[9]。
- 他也公开承认自己长期定价过低，并把它总结成给同行的教训："SaaS startups consistently underprice their products and should look to raise ARPU in most instances."（SaaS 创业者普遍定价过低，多数情况下应该提高 ARPU）[9]。

## 第一批用户/冷启动

- Baremetrics 前 100 个客户直接来自 Josh 在 Twitter 上边做边发的进展帖——受众（Stripe 上的 SaaS 创始人）和他本人是同一群人 [26]。
- Storemapper 的冷启动几乎不存在"启动"：Shopify App Store 的类目搜索就是获客渠道，月增长长期 >10%，全部来自自然流量 [7][10]。

## 收入与定价

- 两条收入曲线的量级差一个数量级，但利润结构相反：
  - Baremetrics：融了 $80 万种子轮（General Catalyst + Bessemer，2014/15），10 人团队，常年刻意维持盈亏平衡；2016 年底一度接近断粮，全员降薪 15%、Josh 自降 30%，没有裁员 [2][3]。卖出时约 1000 个客户、ARR 约 $150 万（播客口径 MRR 约 $15 万），倍数约 2.65 倍 ARR [2][3]。
  - Storemapper：零融资。两年做到 $5 万 ARR，2015-02 破 $10 万 ARR（当时年净利约 $9-9.5 万，净利率 90%+），2016 年 Q1 破 $20 万年化，卖出时 ARR 约 $21.6-25 万（两个来源口径略有出入）[7][8][10]。每周投入约 10 小时，团队 3-5 个远程兼职 [6][10]。
- 对照点：Josh 用 10 个人和 $80 万外部资本换来了规模上限更高但脆弱的公司；Tyler 用 10 小时/周换来一台几乎全是净利的小机器。两人后来各自复盘时，痛点也正好相反——Josh 痛在"管理角色"，Tyler 痛在"天花板"。

## 内容与增长

- 透明是两人共用的增长引擎，而且是同一套基础设施：
  - 2014 年 Baremetrics 公开自家仪表盘后，Buffer 跟进公开了自己的 Baremetrics 面板。Josh 说 Buffer（体量远大于他）这一下"totally changed the trajectory"（彻底改变了 Baremetrics 的增长轨迹）——大客户的公开数据成了最强的产品广告 [5]。
  - 2015-04-22，Baremetrics 正式推出 Open Startups 计划，七家创始成员：Baremetrics、Buffer、ConvertKit、Ghost、Hubstaff、Promoter、Storemapper——Tyler 就在其中，是 Josh 主动邀请他公开数据的 [4][7]。计划上线后有超过 12.5 万创业者围观这些公司的实时收入 [4]。
  - 两天后（2015-04-24），Tyler 发文逐家拆解 Open Startups 名单的 ARPU、流失、LTV 数据——这篇分析成了他 micro-SaaS 论文系列的实证底座。他对透明的总结："Being helpful to other businesses and entrepreneurs pays itself back hugely."（帮助其他创业者，回报是巨大的）[9]。
- 透明在卖出环节继续付息：Tyler 说因为仪表盘本来就是公开的，跟买家的初步沟通几乎不需要"披露"环节 [6]；Josh 那边，公开营收让 Baremetrics 常年自带买家流量——他从交割前 18 个月就开始"接offer 接到手软" [1]。
- Tyler 的 micro-SaaS 系列长文（2016 起）本身就是内容增长的教科书：一套免费电子书，把"个人做小 SaaS"讲成方法论，直接为他后来募基金攒下了受众和 deal flow。核心论断："Recurring revenue is unequivocally the most powerful revenue model in the world today."（经常性收入是当今世界最强大的收入模型）[8]。

## 转型：两场卖出

- **Josh 卖 Baremetrics（2020-11，$400 万现金）**[1][2][3]：
  - 先经历过一次失败交易：2019-04 有买家出价约 $500 万，但采用资产交易结构，税负近 50%，税后反而不划算；拖了 6 个月尽调后于 2019 年 8/9 月告吹，烧掉近 $2 万律师费。他形容那 6 个月"incredibly draining"（极其消耗）[2][3]。
  - 成交的这单刻意反着来：LOI 到交割只用 6 周；Xenon 保证无论尽调发现什么，Josh 到手 $370 万不变；无 earnout、无强制留任；付款分三期（交割、12 个月、18 个月）[1]。他明知 earnout 条款是"the greatest limiting factor on acquisition price"（限制收购价的最大因素），仍宁可少卖也不留尾巴："The prospect of sticking around for years to actually get the payout was soul-crushing."（为了拿到尾款再耗几年的前景令人窒息）[1]。
  - 分配：团队 10 人分 $30 万，期权持有人全额兑现；两家 VC 同意把 $80 万投资直接写掉，成全交易 [1][3]。Josh 因 QSBS（合格小企业股票）几乎免掉全部联邦资本利得税，只交了 5% 的阿拉巴马州税——他承认当年注册 C-corp 时根本没想过这层 [2]。
  - 卖出动机不是价格是身份："At my core I'm a maker. I'm at my most fulfilled when I'm creating."（我本质上是个创造者）；"Did I really want to have spent 10 years of my life building a business analytics software company? No, not really."（我真想把人生十年花在一家商业分析软件公司上吗？并不想）[1]。压垮他的是管理角色 + 疫情 + 家事，以及最后一个新功能 Intros 的惨败——做了大量访谈验证后上线，"I didn't get a single paying customer for it"，他称之为 Baremetrics 历史上最大的士气杀手之一 [1][2]。
- **Tyler 卖 Storemapper（2017-10，价格保密，自称 "level up money"——够把任何下一步变成合理选项，但不够退休）**[6][10]：
  - 渠道是线下社区：他人生第一次参加 MicroConf，就认识了 SureSwift 的 Kevin（McArdle）；同期有三个认真买家，五个月走完全程；没请 broker，因为"我是机会型卖家，不是被迫卖家"[6]。
  - 谈价方式反行规：拒绝"SDE × 倍数"的公式化框架，直接谈整数金额 [6]。
  - 卖出动机同样不是钱："I wasn't burned out, on the contrary life was pretty good and running Storemapper only took about 10 hours per week."（我没有倦怠，生活挺好，每周只花 10 小时）真正的驱动是分散风险 + 腾出全部精力："The real driver was largely non-financial... Storemapper was a means to an end, not necessarily a passion project."（Storemapper 是达成目的的手段，不是热情所在）[6]。还有一句和 Josh 完美互为镜像的身份宣言："I did not want my legacy to be the King of Store Locators."（我不想让"门店地图之王"成为我的人生注脚）[6]。

## 卖出之后：路线分叉

- **Josh：连续 Maker 路线，五年内高开低走** [2][16][17][18][19][21][22]：
  - 第一年刻意远离软件：还清房贷、买了 Model X，全职做激光雕刻推文木杯垫（Laser Tweets），自述做实物"therapeutic"（有疗愈感）[2]。
  - 2021 年重返软件创办 Maybe（个人理财规划），众筹 $145 万（Republic，1300 名投资人），8 人团队闭门开发 18 个月，上线后 1 万等候名单只转化出约 50 个付费用户（均价 ~$15/月）；2023 年年中关停，账上只剩约 $24 万 [16]。
  - 2024-01 把代码开源（"价值 $100 万的 fintech 软件"），恰逢 Mint 关停，仓库爆红登顶 GitHub 趋势榜，反手拿到 OSS Capital 领投的 $150 万，以商业开源模式复活 [17]。
  - 2025-07 转 B2B 财务预测："We're about 6,000 paying customers short of breaking even, with only around 200 paying customers"（离盈亏平衡还差约 6000 个付费客户，现在只有约 200 个）[18]；2025-08-30 他把这次转向定性为回到原点："I sold my startup 5 years ago for $4m, now I'm building it again... New company, same problem."（五年前我把公司卖了 400 万，现在我在重建它——新公司，同一个问题）[19][20]。
  - 2026 年初决定彻底关闭 Maybe，清算全部资产：几十个域名、40+ 代码仓库、上千张设计稿 [21]。截至 2026 年中，他的个人站上同时挂着 9 个进行中的小项目，自称在做"an offensive number of things"（多到冒犯的一堆东西）[22]。
- **Tyler：资本路线，把 micro-SaaS 论文变成一只基金，再亲手关掉它** [11][12][13][14][23]：
  - 2018 年底开始公开写"给 bootstrapper 的融资结构"构想，发明 SEAL（Shared Earnings Agreement，共享收益协议）：像股权投资，但公司可以用利润分成逐步回购大部分股份，不逼公司卖身或上市 [23]。Earnest Capital 由此起步，2021 年更名 Calm Company Fund。
  - 成绩单（2024-12）：4 只小基金、约 $2000 万 AUM、77 家公司、250+ 个人 LP、750+ 股权众筹投资人；只有 4 家关停（占已投资本 6%）；12 家在按季度分红；4 位创始人拿到改变人生的退出；前两只基金 DPI 约 0.5 倍 [12]。
  - 结论是残酷的一句话："The thesis of Calm Company Fund absolutely works, but the business model does not."（论文完全成立，但商业模式不成立）[11]。固定管理费养不活团队："Imagine trying to run a startup where you knew you were going to be stuck at a low-six-figure revenue for 10+ years, meanwhile your customer base, feature requests and support tickets just kept growing every year."（想象经营一家明知十年卡在低六位数收入、而客户和工单每年都在涨的创业公司）[11]。
  - 压垮骆驼的另一根稻草充满戏剧性：起诉方正是当年买走 Storemapper 的 SureSwift——2023-05 SureSwift 在特拉华衡平法院起诉其前 CEO Kevin McArdle 和 Calm Company Fund，指控二者把它挤出 Founder Summit 活动的合资 [14]。诉讼拖了两年多，"让基金的基本运转——听创始人 pitch、辅导被投公司、跟 LP 沟通——几乎不可能"[13]。（2025-06 Tyler 撰文称借助 AI 工具以有利结果了结了这场官司 [15]。）
  - 2024-06 宣布暂停，自嘲："The irony is not lost on me how 'un-calm' these past five years have been."（这五年有多"不平静"，讽刺之处我心里有数）[11]。2024-12 把 Fund IV 已缴资本退还投资人、宣布不再回到早期投资 [13][24]。
  - 新篇章叫"Code & Concrete"（代码与混凝土）：一边在停写代码约 10 年后靠 AI 重新上手（2-3 天做出第一个产品 Sparks，"I am blown away by how much faster (and fun!) it is to build products"），一边和合伙人在布鲁克林 DUMBO 筹建攀岩馆，"I've been feeling incredibly motivated to bring local humans together to do fun things in real life."（我特别想把身边的人聚到线下做有意思的事）[13]。

## "卖还是不卖"：两人的原话对照

- **Tyler 论"表格永远让你别卖"**："A spreadsheet will almost always tell you to hold the SaaS and reconsider selling it in six months."（电子表格几乎永远会告诉你：先拿着，六个月后再考虑卖）——所以他不用 DCF 思维做决定，用的是黑天鹅风险管理思维：单一资产占个人净值比例太高，本身就是该卖的理由 [6]。
- **Tyler 的"泰山法则"**：先抓住下一根藤，再松开这一根（the Tarzan approach）——他是在确认自己想全力投入投资和新项目之后才关闭交易的 [6]。
- **Josh 论"为确定性折价"**：接受无 earnout 的 $400 万，而不是有尾巴的更高价——"What I really wanted was to not *need* to start something."（我真正想要的，是"不必"再开始什么）[1]。
- **Josh 论情绪账**：卖公司"bittersweet, in the same way that sending a kid off to college is bittersweet"（苦乐参半，就像送孩子上大学）；交割后他"mentally freer than I had in the previous seven years"（比过去七年任何时候都轻松）[1][2]。
- **五年后的反转（本档案最重的一条对照）**：2025 年 Josh 公开承认绕了一圈又回到原题——"For the seven years I worked on Baremetrics, the questions I..."（那七年我一直想回答的问题，现在还想回答）[19]；而这次重建也在 2026 年初随 Maybe 一并清算 [21]。Tyler 则从未回头做 SaaS，他的"再抓一根藤"一路荡到了基金、再荡到攀岩馆——两人用五年时间分别验证了：卖掉一门还在赚钱的生意，代价不是钱，是你和那个问题的关系。

## 如何保持小

- Storemapper 是"保持小"的范本：10 小时/周、3-5 个兼职、90%+ 净利、1-1.5% 月流失，Tyler 给它的定位是"Not a startup; a healthy growing internet small business."（不是 startup，是一门健康成长的互联网小生意）[6][7]。
- Baremetrics 是反例——它从一开始就没打算小：融资、10 人团队、常年盈亏平衡，Josh 事后承认自己根本不想要"growing or scaling things"，管理角色让他不堪重负 [1]。做 Maybe 时他重复了同样的错误：8 人团队闭门 18 个月憋大招 [16]。他真正舒服的形态，是 2026 年这种"9 个小项目并行、AI 当员工"的一人模式 [22][27]。
- 最辛辣的教训来自 Tyler 自己：一只专门投"calm company"的基金，自己却活成了 un-calm 公司。他说五年最大的一课是要确保"Calm Company Fund is itself a calm company"（Calm Fund 自己首先得是一家 calm company）——而管理费模式在结构上不允许 [11][12]。他还发现被投组合里"死掉或停滞的头号原因"恰恰是创始人融资过多或过度关注融资 [12]——资本方亲手验证了资本的害处。

## 开放问题（值得当面问本人的）

1. 问 Josh：为"无 earnout + 保底 $370 万"你实际放弃了多少对价？如果再卖一次公司，"确定性折价"的底线画在哪——比如买方出 1.5 倍价格但要你留任两年，接不接？
2. 问 Tyler：泰山法则说"先抓住下一根藤"，但你松开 Storemapper 时，Earnest 还只是个想法、没有一分钱收入——你当时凭什么判断那根藤"已经抓住了"？回头看是运气还是方法？
3. 问 Josh：五年里三次回到"帮创始人看懂财务数据"这个问题（Maybe B2C、B2B 转向、"new company, same problem"），全部失败——是问题本身选错了，还是"Maker 的工作方式"与"需要十年经营的数据业务"天然冲突？如果 2020 年不卖，Baremetrics 今天会更好还是更糟？
4. 问 Tyler："论文成立、商业模式不成立"之后，给 bootstrapper 的资本正确形态到底是什么——holdco、SPV、收益分成平台，还是（按你自己的 AI 判断）这个资产类别在 AI 时代根本不再需要存在？
5. 问两人同一个问题：钱到账后的第 18 个月，各自最意外的心理变化是什么——Josh 说过想要"不必再开始什么"，结果开始了比以前更多的东西；Tyler 想要 calm，结果过了五年最不 calm 的日子。你们现在如何解释这个悖论？

## 来源

1. Josh Pigford, "I Sold Baremetrics", Baremetrics Blog, 2020-11-10. https://baremetrics.com/blog/i-sold-baremetrics
2. Startups For the Rest of Us, "Episode 534 | A $4M Exit with Josh Pigford of Baremetrics", 2020-12. https://www.startupsfortherestofus.com/episodes/episode-534-a-4m-exit-with-josh-pigford-of-baremetrics
3. They Got Acquired, "SaaS analytics startup Baremetrics sells to private equity firm Xenon Partners". https://theygotacquired.com/saas/baremetrics-acquired-by-xenon-partners/
4. Baremetrics Blog, "The Open Startups Initiative", 2015-04-22. https://baremetrics.com/blog/open-startups
5. Leave Me Alone Blog, "Embrace Transparency: Lessons from Baremetrics, Buffer, and Glitch". https://leavemealone.com/blog/embrace-transparency-and-openness/
6. Tyler Tringas, "Selling My Bootstrapped SaaS Business", 2017-10. https://tylertringas.com/selling-my-bootstrapped-saas-business/
7. Tyler Tringas, "The Storemapper Story – Radical Transparency". https://tylertringas.com/storemapper/
8. Tyler Tringas, "Chapter 1: What Is Micro-SaaS & Why Should You Read This"（Micro-SaaS ebook）. https://tylertringas.com/1-what-is-micro-saas/
9. Tyler Tringas, "Digging in to the Open Startups List", 2015-04-24. https://tylertringas.com/digging-in-to-the-open-startups-list/
10. They Got Acquired, "This founder built his SaaS beta on a flight and sold it when he hit $216,000+ ARR"（Storemapper → SureSwift）. https://theygotacquired.com/saas/storemapper-acquired-by-sureswift-capital/
11. Calm Company Fund, "Calm Company Fund is taking a break", 2024-06. https://calmfund.com/writing/pause
12. Calm Company Fund, "Calm Company Fund: Five Years In", 2024-12. https://calmfund.com/writing/five-years
13. Tyler Tringas, "Code & Concrete: A New Chapter in 2025", 2024-12-23. https://tylertringas.com/code-concrete/
14. Delaware Business Court Insider (Law.com), "SaaS Company Claims Freeze-Out By Ex-CEO, Joint Venture Partner", 2023-05-16. https://www.law.com/delbizcourt/2023/05/16/saas-company-claims-freeze-out-by-ex-ceo-joint-venture-partner/
15. Tyler Tringas, "How AI Saved My Company From a 2-Year Litigation Nightmare", 2025-06-08（tylertringas.com 首页列表）. https://tylertringas.com/
16. Failory, "3 Reasons Why Maybe Failed". https://newsletter.failory.com/p/3-reasons-maybe-failed
17. The Bootstrapped Founder（Arvid Kahl）, "Josh Pigford — The Open-Source Transformation of Maybe". https://thebootstrappedfounder.com/josh-pigford-the-open-source-transformation-of-maybe/
18. @Shpigford, "Maybe is making a pivot to B2B", X, 2025-07. https://x.com/Shpigford/status/1947725345244709240
19. @Shpigford, "I sold my startup 5 years ago for $4m, now I'm building it again", X, 2025-08-30. https://x.com/Shpigford/status/1961548168749092968
20. @Shpigford, "Maybe Investor Update: September 2025", X, 2025-09. https://x.com/Shpigford/status/1962858318336004419
21. @Shpigford, Maybe 关停清算推文, X, 2026-03. https://x.com/Shpigford/status/2038774838475805081
22. joshpigford.com（2026 年项目列表："Currently building...an offensive number of things"）. https://joshpigford.com
23. Crunchbase News, "Too Small For Venture? SEALs And Early-Stage Investment Firms Offer Financing". https://news.crunchbase.com/startups/too-small-for-venture-seals-and-early-stage-investment-firms-offer-financing-although-options-still-limited/
24. @tylertringas, 年末决定线程（"the fund will not be returning to early stage investing"）, X, 2024-12-30. https://x.com/tylertringas/status/1873736640226787529
25. Baremetrics Founder Chats, "50 Projects in 15 Years: Lessons from Josh Pigford". https://baremetrics.com/founder-chats/josh-pigford
26. Starter Story, "How Josh Pigford Grew Baremetrics to $4M as a Side Project". https://www.starterstory.com/baremetrics-breakdown
27. self.md, "Josh Pigford"（Maybe 开源复活与 AI 工作流）. https://self.md/people/josh-pigford-maybe-finance
