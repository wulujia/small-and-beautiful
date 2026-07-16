# Sidekiq（Mike Perham）

> Ruby 后台任务框架的商业开源：免费版做到市场第一，把"可靠性"和"企业需求"做成付费版 ｜ sidekiq.org ｜ Mike Perham ｜ 2012 ｜ 1 人（"1 employee (me!)"）｜ 开源 open-core / 开发者工具 / pure-bootstrap ｜ 2023 年自述"closer to $10m than $1m"年收入，2022 年初累计销售 $13.5M [1][6]

## 缝隙切入点

2011 年的 Ruby 后台任务市场被 Resque（GitHub 出品）和 DelayedJob 统治，两者都是单进程单任务模型，内存开销巨大。Perham 判断"existing background job solutions for Ruby were slow and inefficient"，于 2012 年 1 月 16 日推了 Sidekiq 第一个 commit，2 月公开发布 [1][5]。

技术缝隙是"多线程"：Sidekiq 是第一个只跑多线程的主流 Ruby 任务系统（"Sidekiq was the first major Ruby job system to run multi-threaded only"）。当时整个社区害怕线程安全问题，他赌的是"someone had to entice the community to address thread-safety"，结果"the promise of a huge leap forward in performance won the day"——一年之内主流 gem 的线程安全问题基本被社区修完 [1]。

商业缝隙是"开源维护者的倦怠循环"：他见过太多 OSS 项目"热情—创造价值—被支持请求淹没—弃坑"的死亡螺旋，发布几个月后他公开宣布 Sidekiq"unsustainable"，要做"financial experiments"来保证长期维护 [1][5]。免费拿走世界 500 强的劳动成果、作者分文不取——他把这个行业级别的不公平当成了自己的生意入口 [5]。

一个细节：他在 2012 年初入职新公司前，特意在雇佣合同里加了 Sidekiq 的知识产权豁免条款（"I made sure my employment contract had a IP carve out for anything related to Sidekiq"）——从第一天就打算把它变成自己的资产 [6]。

## 时机

- 2012 年正值 Rails 应用大规模上 Heroku，按 dyno（进程）计费，Resque 的进程模型直接烧钱。Sidekiq 多线程把内存占用砍掉一个数量级，"Within a month of releasing Sidekiq, I had people coming to me and telling me that they were saving thousands of dollars a month in server hosting costs"——省下的服务器账单就是现成的付费理由 [9]。
- 他从 2007 年起持续写 Ruby/开源博客，发布时已有现成的声誉和读者，冷启动不需要买流量 [5]。

## 差异化

对开发者：快 10 倍以上、省内存、自带重试和监控 UI。对付费客户，他卖的不是软件而是"不用自己造分布式系统"："A job system is a distributed system… Building your own almost always leads to a worse system than the mature, well-debugged system" [6]。

对竞品的差异化是商业结构本身：VC 支持的竞品"tend to go bankrupt, because they either get big or they go out of business"，而他"bootstrapped、profitable"，打算"be around forever"——对采购基础设施的企业来说，供应商能活 20 年本身就是卖点 [7]。

**免费/付费的边界设计（本案例最核心的资产）**：

- 免费版必须强到能拿下市场第一：完整的任务系统、重试、定时、Web UI，绝大多数小团队永远不需要付费 [5][10]。
- Pro（现 $995/年，公司数计费、服务器无限）卖的是**可靠性和工作流**：Ruby VM 崩溃时任务不丢（super_fetch）、Redis 网络抖动时客户端不丢任务、Batches 批量工作流、Web UI 搜索、作者优先邮件支持 [11]。翻译成一句话：免费版够用，但"任务绝对不能丢"是付费功能。
- Enterprise（从 $269/月起，按生产环境线程数滑动计费，封顶 unlimited license $79,500/年）卖的是**组织级需求**：限流、周期任务（cron 替代）、任务去重、加密、滚动重启、多核 swarm，外加大公司才需要的东西——可谈判的商业许可证和发票/PO 采购流程 [3][10][12]。他说得很直白："Sidekiq Pro's low price means I cannot accept license changes which the lawyers at larger corporations often demand"——律师要改条款？请升级 Enterprise [3]。
- 分层的真正依据不是功能多少，而是**买家是谁**：Pro 定价 $1,000/年左右是刻意压在企业内部免审批额度之下（"way less than… a salary or even a laptop"），工程师刷卡就能买 [7][8]；Enterprise 的发票溢价则把行政成本定价进去——"you can either pay with a credit card or you can not use Sidekiq. Like, that's it" [7]。

## 第一批用户/冷启动

- 2012 年头 9 个月他先试了 LGPL + $50 商业许可证：33 单、$1,650，他自己定性为"failure"——价太低，买的人反而不当回事 [2]。
- 2012 年 10 月推出 Sidekiq Pro，$500 一次性买断（按公司计），第一年卖出约 140 份、$70,000 [1][2]。
- 销售完全靠口碑和文档："it's sold purely through word of mouth and mentions in the Sidekiq documentation"——付费功能就写在免费用户天天查的 wiki 里，文档本身是销售渠道 [2]。
- 线下唯一有效的动作是 Ruby 会议："my best response has been at developer conferences: when I meet and network with other Rubyists to answer their questions and soothe their fears, they buy Sidekiq Pro" [2]。
- 早期大客户拿下 Heroku、New Relic（他原本的目标是 GitHub/Basecamp 级别的 logo）[9]。

## 收入与定价

涨价史（全部有出处的节点）：

| 时间 | 动作 | 数字 |
|---|---|---|
| 2012 初 | LGPL + $50 商业许可 | 9 个月 $1,650，失败 [2] |
| 2012.10 | Pro 上线，$500 一次性/公司 | 首年 140 份、$70k [1][2] |
| ~2014 | 一次性改年订阅 | "The only big mistake that I made on day one was I didn't sell the software as a subscription"；改完"much more predictable revenue" [9] |
| 2014 夏 | 副业收入超工资，辞职全职 [5] | 2013 年中已到 $10k/月 [5] |
| 2015.8 | Enterprise 上线，按线程滑动计费；Pro 时价 $950/年 [3] | 2015 年收入同比 2.6x，客单价翻倍到约 $2,000 [4] |
| 2016.11 | — | $80k/月（HN 热帖标题）[16] |
| 2022.1 | 十周年 | 累计销售 $13.5M、1,850 客户、"1 employee (me!)" [1] |
| 2023.4 | — | "I'm closer to $10m than $1m in annual revenue now"、约 2,000 客户 [6] |
| 现价 | Pro $995/年；Enterprise $269/月起，unlimited $79,500/年，appliance 授权 $14,995–39,995/年 [10][11][12] | |

定价哲学：只收年费不收月费——"Once you integrate it, it's likely to stay as part of your app for years"，产品的粘性决定了计费周期 [5]。2015 年他总结出关键一课：与其做量，"it turns out to be easier to convert 500 customers at $2000 each"——靠 Enterprise 拉客单价，而不是降价拉客户数 [4]。

客户分层的清醒认知："有的客户一年付五位数、几乎从不联系我（理想）；有的付 $99/月、天天抱怨（麻烦）" [7]。

## 内容与增长

- 增长引擎是开源采用漏斗：免费版做到市场第一（超过 Resque + DelayedJob 之和 [4]），开发者跳槽把 Sidekiq 带进新公司，公司规模到了自然撞上付费边界。"figure out … the breakpoints where you can give something away for free but charge money for additional value" [5]。
- 营销预算约等于零："My only planned marketing is attending Rubyconf and Railsconf every year, handing out stickers and t-shirts"，不买广告、不办企业活动、不见 CIO [5][9]。
- 他持续用博客公开经营数据（2013 年《How to make $100k in OSS by working hard》、每年生日帖、2015 年报），透明本身成了最强的内容营销——每篇都上 HN 头条 [1][2][4][16]。

## 社区

- 商业化公开透明：动手收费前先公开预告"I'm going to be experimenting with financial stability and sustainability with this project"，社区没有反弹 [7]。
- 支持策略 GitHub-first：免费用户私信一律回"I'm sorry I don't respond to private email, unless you're a customer"；问题引到公开 issue，因为"that's a public record that people can search… If one person has that problem, there's probably a dozen other people that have that same problem"——支持工作沉淀为可搜索的资产，而不是消耗 [7]。
- 截至 2022 年：11,500 stars、4,100 commits（含社区贡献）、1.15 亿下载 [1]。

## 留存

- 年订阅 + 基础设施粘性 = 低流失："not a huge amount of churn"，近年客户数年增约 15–20%，在 Ruby 大盘停滞的背景下靠留存复利慢慢长 [7]。
- 支持负担不随客户数线性增长："once customers are on Sidekiq and they've got it working, then by and large, you don't hear from them all that much" [7]。付费墙本身过滤掉了不会读文档的初学者 [7]。

## 转型

- 一次性买断 → 年订阅（~2014）：他自认的唯一"day one 大错" [9]。
- 单产品 → 双层（2015 Enterprise）：客单价翻倍的杠杆 [3][4]。
- 失败的多元化：服务器监控工具 Inspeqtor 因无人问津停掉 [4]；跨语言任务系统 Faktory（Ruby/Python/Go 通吃）活着但定位克制——Ruby-only 项目他自己都推荐用 Sidekiq [7]。
- 正面迎战免费替代品：2024 年底 Rails 8 把 Solid Queue 设为默认任务后端，他亲自发 benchmark——50 万任务入队 Sidekiq 3.3 秒 vs SolidQueue/sqlite 63 秒——用性能数据而非口水战回应，2025 年 4 月发布 Sidekiq 8.0（新增 profiling）[17][18]。
- 交接问题已公开摆上桌：2022 年他写道自己"likely won't see 2030 as project owner and maintainer"，BDFL 是单点故障，快 50 岁了想享受成果，"One idea is to turn Sidekiq over to Ruby Central" [1]。

## 如何保持小

这是全案例库里"拒绝规模化"最系统的样本——不是没能力扩张，而是把"能一个人跑"写进每一条商业政策：

- "I explicitly create business policies so that I can run solo"：只收信用卡（"Sidekiq Pro is credit card only, no exceptions"）、发票只给 400 线程以上的 Enterprise 大单、官方支持政策是每客户每季度一张工单 [7][10]。
- 基建极简：gem 服务器是 3 台 $6 的 DigitalOcean droplet（合计 $18/月），一年只需一天维护，扛每天 300 万次请求 [1][6]。
- 拒绝雇人的理由不只是省事，还有一个罕见的公平论证：付工程师 $20 万年薪、自己留下剩余利润，"almost seems a little bit unfair"——两个人都是每周 40 小时 [7]。以及直白版："I didn't want to hire people, period. I don't want to be a manager" [8]。
- 拒绝融资：不用"take funding and find investors and split your attention"，低成本慢慢长，风险自己扛 [5]。
- 保持一线的产品理由："If I take myself out of the trenches… then I lose that sense of pain that customers might be feeling" [8]。
- 终点定义："the whole point of becoming a success is not having to work very hard and getting to enjoy your life therein"——空闲时间用来"relaxing and enjoying my success rather than pushing the ball forward"，接送孩子上下学 [14]。
- 他甚至反过来质疑自己这套模式的可复制性："Turning everybody into a businessman so that they can keep their project going, it itself is not sustainable… that's why everything turns into a SaaS"——他认为开源基础设施长期应该像公路和自来水一样由公共资金维护（举例荷兰 NLNet 资助 Mastodon）[7]。

## 开放问题（值得当面问本人的）

1. 免费/付费的那条线是怎么一刀一刀试出来的？有没有哪个功能你差点放进免费版、最后决定收费（或相反）？"可靠性归付费"是事先的原则还是事后的总结？
2. 从 $500 买断到 $995/年 + Enterprise 滑动计费，每次涨价是怎么定的？有没有哪次涨价的结果（流失/抱怨）和你预期差别最大？
3. 14 年里最接近改变主意的一刻是什么——最高的收购出价/最动心的雇人冲动是哪次，为什么最终没做？
4. Solid Queue 成为 Rails 8 默认后，免费→Pro 的转化漏斗有可测的变化吗？你的应对预算里，性能（技术）和定价（商业）各占多少？
5. 2022 年你说不会以 owner 身份见到 2030，Ruby Central 是一个想法。现在走到哪一步了？一门"一个人的千万美元生意"，该怎么设计它的身后事——客户合同、商标、gem 服务器、还有你脑子里那些没写下来的东西？

## 来源

1. Happy 10th Birthday, Sidekiq!（2022-01-17）— https://www.mikeperham.com/2022/01/17/happy-10th-birthday-sidekiq/
2. How to make $100k in OSS by working hard（2013-10-01）— https://www.mikeperham.com/2013/10/01/how-to-make-100k-in-oss-by-working-hard/
3. Sidekiq Enterprise 发布帖（2015-08-06）— https://www.mikeperham.com/2015/08/06/sidekiq-enterprise/
4. Contributed Systems: the 2015 wrapup（2016-01-05）— https://www.mikeperham.com/2016/01/05/contributed-systems-2015/
5. Indie Hackers 文字访谈 "How Charging Money for Pro Features Allowed Me Quit My Job"（2016）— https://www.indiehackers.com/interview/how-charging-money-for-pro-features-allowed-me-quit-my-job-6e71309457
6. HN 讨论串（2023-04，含 mperham 本人评论）— https://news.ycombinator.com/item?id=35566768
7. Software Sessions 播客 "Keeping it solo"（RubyConf 2023）— https://www.softwaresessions.com/episodes/keeping-it-solo/
8. Startups For the Rest of Us Ep. 661（2023）— https://www.startupsfortherestofus.com/episodes/episode-661-millions-in-revenue-as-a-one-person-software-company
9. Garrett Dimon, Starting & Sustaining 访谈 — https://garrettdimon.com/starting-and-sustaining/interviews/mike-perham
10. Sidekiq Commercial FAQ（GitHub wiki）— https://github.com/sidekiq/sidekiq/wiki/Commercial-FAQ
11. Sidekiq Pro 产品页 — https://sidekiq.org/products/pro/
12. Sidekiq Enterprise 产品页 — https://sidekiq.org/products/enterprise/
13. saas.group SaaS Unbound 播客（标题称 bootstrap 到 $7M）— https://saas.group/podcasts/saas-unbound-interview-mike-perham-sidekiq/
14. Just the Useful Bits 播客 — https://justtheusefulbits.com/jtub/mike-perham-sidekiq-and-whitepapers-and-what-success-is-for/
15. mikeperham.com About 页 — https://www.mikeperham.com/about/
16. HN "How Sidekiq makes $80,000 a month"（2016-11）— https://news.ycombinator.com/item?id=12925449
17. Sidekiq 8.0: Profiling（2025-04-08）— https://www.mikeperham.com/2025/04/08/sidekiq-8.0-profiling/
18. Sidekiq vs Solid Queue in 2026（引用 Perham 本人 2024-11 benchmark gist）— https://taywind.com/en/blog/sidekiq-vs-solid-queue-in-2026-when-to-switch-and-when-not-to/
