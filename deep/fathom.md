# Fathom Analytics

> 隐私优先的极简网站分析，反 Google Analytics ｜ usefathom.com ｜ Paul Jarvis & Jack Ellis（另有初代技术合伙人 Danny van Kooten，2018 年底离开）｜ 2018（加拿大 Victoria, BC，公司实体 Conva Ventures）｜ 2 位创始人 + 1 名全职开发 + 数名兼职（隐私官/法务/内容）[1][7] ｜ pure-bootstrap / privacy SaaS / 反巨头 ｜ 收入从不公开；Starter Story 页面标注 $1M/月但系页面标签而非访谈原话，存疑；官方口径是"两年内盈利、两位创始人都拿薪水"[1][10]

**关键更新（核实结果）：Paul Jarvis 已于 2024 年 12 月 1 日正式退出。** 两人在 2024-10-25 达成协议——距离 Paul 提出想退休只隔了 24 小时——Jack Ellis 买断股份成为唯一所有者，Paul 退休，仅以兼职自由职业身份继续做设计 [3]。Paul 本人 2020 年起已删除 Twitter/Instagram、彻底离网 [6]；其个人域名 pjrvs.com 现在 301 跳转到 usefathom.com/pjrvs，页面写明"He no longer exists on social media... Please do not contact Fathom Analytics' customer support to get in touch with him"[5]。《一人公司》作者本人从互联网上消失了，这本身就是他理论的终极注脚。

## 缝隙切入点

2018 年，Google Analytics 装在约 85% 的网站上——臃肿、侵犯隐私、免费但以数据为代价 [1]。Paul Jarvis 发了一条推："What if website analytics software didn't take your users data to line their pockets for advertising?"，并附上一张他想象中的极简分析面板 mockup。截图疯传，数百人表示愿意付钱 [1][4][12]。缝隙的本质：**为一个"免费"巨头产品的隐性代价（隐私、复杂度）提供付费替代品**——用户不是买功能，是买"更少的功能 + 干净的良心"。先做了开源版 Fathom Lite（Golang，下载量数百万次）验证需求，再转付费托管版 [4][16]。

## 时机

- 2018-04 成立，一个月后（2018-05-25）GDPR 正式生效 [1]——踩在欧洲隐私执法元年的门槛上。
- 2020-07 Schrems II 判决后，Fathom 与隐私官、律师研究方案，2021 下半年上线 EU Isolation（欧盟访客数据留在德国 Hetzner 服务器处理）[19][7]。
- 2022-01-13 奥地利数据保护局裁定 Google Analytics 违反 GDPR，2022-02 法国 CNIL 跟进 [18][20]——Fathom 的内容机器立刻跟上（博客《Your website analytics are breaking the law》等），把每次监管裁决变成获客事件 [18][19]。
- Starter Story 访谈（2022-03，Paul 自述）："in the last year we've grown more than 70%" [1]。
- 每一次不是运气，而是提前 1-2 年备好合规基础设施再等监管开枪。

## 差异化

**对 Google**：付费、无 cookie、无需同意弹窗、单页面板；商业模式差异是根——"我们靠卖软件赚钱，所以根本不需要考虑卖数据"[10]。客户包括 GitHub、IBM、Buffer、Bootstrap、HashiCorp、纽约时报、Laravel [1][4]。

**对 Plausible（同缝隙最直接对手，2019 年起步）**：
- Plausible 开源（AGPL）+ 可自托管 + 全欧盟基础设施 + 公开路线图；Fathom 闭源、仅云端、加拿大公司 + EU Isolation 混合架构 [17]。
- 按 BuiltWith 数据（2024-10），Top 100 万网站中 Plausible 部署 3,500 个 vs Fathom 1,832 个——开源路线在 indie hacker 群体里赢了声量 [17]。
- Fathom 的反向下注：放弃开源换取商业控制，赌企业客户在乎"永久数据保留 + 企业级基础设施"而非可审计性 [9][14]。两条路都活得不错，同一条缝隙容得下两家 bootstrap 公司。

**技术叙事（Jack Ellis 的杠杆）**：2019 年 V2 用 Laravel 重写（替换 Go），成为 Laravel Vapor（serverless 部署平台）发布时第一批全量上线的公司 [2][15]。Jack 的逻辑："we pay so each page view goes through a lambda request... AWS maintains that for us"[7]——**用 serverless 把运维团队外包给了 AWS，这是"保持小"的技术前提**。

## 第一批用户/冷启动

三级火箭：① Paul 的既有受众——他当时有热门 newsletter 和活跃 Twitter，"Paul's audience was the primary source of customers to pay for Fathom"[12]；② 开源版 Fathom Lite 作为漏斗，数百万下载 [4]；③ 付费托管版收网。官方承认从没有过某个爆点："There was never really a giant wave or surge of customers... it's been a slow and steady ramp-up"[1][12]。

## 收入与定价

- 不公开收入。可确认的硬点：产品让公司"from zero to profitable (including salaries for both cofounders) in less than two years"[10]；2021→2022 年增长 70%+ [1]。
- 定价哲学三个"不"：**无免费版**（"我们重投企业级基础设施"）；**永不打折**——"Never. Not even for Black Friday"；**无合同**，随时取消 [9]。
- 现行定价（2026-07 官网）：按月度 pageview 阶梯计费，50 万 pageviews 档 $45/月，年付送两个月，7 天免费试用，所有档含 50 个站点 + 永久数据保留 [9]。
- 副线收入：Jack 2020 年推出 Serverless Laravel 课程，个人入账 $150,000 [11]——早期用课程收入补贴创始人生活，降低公司增长压力。

## 内容与增长

- 主渠道是口碑，广告投入极少（Paul 时代）[1]。
- 内容双引擎：博客（隐私法规追热点 + Jack 的硬核技术长文）+ 播客 Above Board [1]。Jack 的《We rebuilt Fathom + moved to Laravel Vapor》类技术文在 Laravel 社区自带传播，他另有数千人的工程文章邮件列表 [8][15]。
- 监管即营销：奥地利/CNIL 每次裁定 GA 违法，Fathom 都第一时间出解读文章收割搜索流量 [18][19]。
- 反 VC 行为艺术：Jack 在 LinkedIn/X 发"Fathom Analytics raises $100 million series A"，点进去是 Rickroll 视频——"convinced everybody that we'd taken $100 million in funding but then redirected them to a Rickroll"[3][13]。嘲讽融资文化本身成了品牌资产。
- 带隐私保护条款的联盟计划 [1]。

## 转型

三次关键转折，每次都可能死：

1. **开源→闭源（2019）**：曾公开承诺 V2 开源，后反悔闭源，官方播客承认"we messed up by announcing V2 would be open-source, but then changing our minds"，态度是"changing your mind is ok"[14]。Fathom Lite 保留维护但不加功能 [16]。
2. **近死亡时刻（2018-12）**：初代技术合伙人 Danny van Kooten 退出，Paul 一度打算关掉——"There were definitely a few days where I thought I was definitely going to shut Fathom down for PRO customers"。转机是他和 Jack Ellis 在合作另一个项目 Pico 时随口提起，Jack 主动提出接任技术合伙人（2019 年初）[2]。V2 重写迁移 6000 万+ 历史 pageview 零丢失 [2]。
3. **创始人买断（2024）**：Paul 想退休，Jack 觉得自己还有很多年——"We actually came to an agreement within 24 小时 of discussing Paul's desire for retirement"（原话 within 24 hours），10-25 握手，12-01 交割，之后花一个月走律师和会计流程 [3][13]。Jack 接手后的调整方向：加码 enterprise sales 和付费广告/赞助 [3]——开始偏离 Paul 时代"几乎不投广告"的打法，值得持续观察。

## 如何保持小

- 雇人铁律："We don't hire unless it's too painful not to, and we don't hire unless we can easily remain profitable when we factor in a new salary"，并且明确说"sometimes adding more people can slow things down"[8]。
- 结构：两位创始人 + 1 全职工程师 + 兼职资深工程师（负责 EU Isolation）+ 全职客服 + retainer 制的隐私官（Rie Aleksandra Walle）、法务、内容、SEO 外包 [1][7][4]。Starter Story 页面标签甚至写"Employees: 0"[1]。
- 技术换人头：serverless（Lambda + Vapor）让基础设施"坏了就自动换一个"，无需运维团队 [15][21]。
- 治理极简到危险的程度：**六年没有股东协议**——"We have been able to run this company without a shareholder agreement since starting it because we are aligned in many ways"（Jack）[3]。
- 无投资人 = 无人头压力："we don't have investors who expect us to increase our headcount rapidly"[8]；"We're not searching for investors, exits, or IPOs"[3]。
- Paul 的注解：他从不把身份绑在公司上（"has never tied his identity to the business"），所以退出很平滑 [13]。Fathom 是《Company of One》（2019 年 1 月出版，20+ 语言版本，含中文版《一人公司》）的实践场：不追增长、公司设计即生活方式设计 [5][6]。

## 开放问题（值得当面问创始人的）

1. 你们六年没签股东协议，靠"对齐"运转——对齐是怎么维护的？最接近破裂是哪一次？
2. 2024 年买断在 24 小时内谈定：一家从不公开收入的公司，你们俩是怎么给它定价的？用了什么估值逻辑？
3. "不雇人除非不雇会痛"——有没有哪次这条规则让你付出了代价（雇晚了）？serverless 具体替代了几个人头？
4. 《一人公司》的理论在 Fathom 的实践里哪里失灵过？Paul 心里"enough"到底是一个具体数字，还是一种感觉？
5. 接手后你说要加码 enterprise sales 和付费广告——Fathom 在什么边界之前还算"small tech"？如果重来一次，Fathom Lite 还会开源吗（看着 Plausible 靠开源在装机量上反超）？

## 来源

1. Starter Story 访谈 Paul Jarvis（约 2022-03）：https://www.starterstory.com/stories/fathom-analytics-4887dc81-8d94-4296-a88b-5613b8c2aa80
2. Fathom 官方博客《From almost shutting down to tripling our MRR》：https://usefathom.com/blog/v2
3. Fathom 官方博客《Fathom Analytics has been acquired》（2024-12）：https://usefathom.com/blog/acquired
4. Fathom About 页：https://usefathom.com/about
5. Paul Jarvis 页面（pjrvs.com 301 跳转至此）：https://usefathom.com/pjrvs
6. Justin Jackson《What happened to Paul Jarvis?》（2023-08）：https://justinjackson.ca/paul-jarvis
7. The Bootstrapped Founder 播客访谈 Jack Ellis：https://thebootstrappedfounder.com/jack-ellis-taking-on-google-as-a-bootstrapper/
8. Fathom 官方博客《Jack and Paul interviewed》：https://usefathom.com/blog/interview
9. Fathom 定价页（2026-07 抓取）：https://usefathom.com/pricing
10. Fathom《for bootstrappers》页：https://usefathom.com/for-bootstrappers
11. Indie Bites #35（Jack Ellis，课程 $150k）：https://indiebites.com/35
12. Transistor 客户故事（Paul Jarvis 原始推文引语）：https://transistor.fm/customers/paul-jarvis/
13. Above Board 播客《Paul has retired》：https://usefathom.com/podcast/paul-retired ；Indie Bites #126《Why Jack Ellis acquired Fathom Analytics from his co-founder》：https://indiebites.com/126
14. Above Board 播客《The open-source dilemma》：https://usefathom.com/podcast/opensource
15. Fathom 博客《We rebuilt Fathom Analytics + moved to Laravel Vapor》：https://usefathom.com/blog/moved-to-vapor
16. Fathom Lite 开源仓库：https://github.com/usefathom/fathom
17. Swetrix《Fathom Analytics vs Plausible》对比（引 BuiltWith 2024-10 数据）：https://swetrix.com/comparison/fathom-analytics/vs-plausible
18. Fathom 博客《CNIL finds Google Analytics in breach of GDPR》：https://usefathom.com/blog/cnil-illegal-google-analytics ；《Your website analytics are breaking the law》：https://usefathom.com/blog/illegal-analytics
19. Matomo 博客（奥地利 DPA 2022-01-13 裁决）：https://matomo.org/blog/2022/01/google-analytics-gdpr-violation/ ；Fathom EU Isolation 时间线见 [18]
20. Termageddon（奥地利 DPA 裁决综述）：https://termageddon.com/austrian-dpa-rules-that-google-analytics-is-not-gdpr-compliant/
21. Servers for Hackers《5 reasons why we chose serverless for Fathom Analytics》：https://serversforhackers.com/c/fathom-analytics-serverless
