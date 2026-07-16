# SavvyCal

> 在 Calendly 阴影下做"发出去不尴尬"的日程预约链接：双边体验（发送方+收件人）是楔子 ｜ savvycal.com ｜ Derrick Reimer ｜ 2020 ｜ 3–4 人 ｜ bootstrap + TinySeed 小额基金（注意：不是纯零外部资金）｜ 公开里程碑到 2022 初 $20k MRR，此后不公开（2024 年第三方估算 ~$1M ARR，低置信）

## 前传：Level 的失败复盘

- Derrick 的底子：2012 年底与 Rob Walling 联合创办邮件营销公司 Drip（任 CTO），2016 年 7 月被 Leadpages 收购；此前还独立做过 Codetree（GitHub Issues 项目管理，后出售）[16][8]。
- 2018 年 3 月 3 日离开 Drip，全职做 Level——"为深度工作优化的团队沟通工具"，对抗 Slack 制造的虚假紧迫感 [1][18]。造势教科书级：宣言式 manifesto、6,000+ 用户名预留、约 500 场用户访谈、约 50 份 $49 预购、2018 年 10 月 alpha、2019 年 1 月公开发布 [1]。产品本身是开源可查的 Elixir/Phoenix + Elm 全栈应用（GitHub 约 1,000 stars）[18]。
- 2019 年 5 月 17 日发布著名关停长文《I'm Walking Away From the Product I Spent a Year Building》[1][22]。他测算要 $10k–15k MRR 才能养活自己，实际付费转化只有个位数量级 [1]。
- 复盘的四条死因 [1]：
  1. 嘴上痛苦 ≠ 行动。人人都骂 Slack，但追问"你为此做过什么？"——"almost universally the answer was 'nothing.'"
  2. 卡在中间：小团队觉得 Slack "at most a minor annoyance" 不值得迁移；大团队要求 "months (or years) of development work" 才肯考虑。
  3. 买单人错位：付费预购者中只有一小部分认真上手，最兴奋的人往往不是掏钱决策者。
  4. Manifesto 造成确认偏误：访谈对象在复述他的假设，而不是暴露真实需求——数据从源头被污染。
- 一句最狠的自我审判："unless you are raising venture capital and planning to shoot for the moon, unicorn dreams shouldn't bias your decisions"——要么去融资赌登月，要么从第一天就故意做小而可持续的生意，他两头都没选 [1]。
- Level 和 SavvyCal 之间还有一次快速止损：StaticKit（静态站表单后端）。发现这个市场需要庞大免费层伺候"只是玩玩的人"、买家太少，果断降级，2020 年 10 月卖给 Formspree [4][19]。一年多两次放弃，衬托出第三次的选题纪律。

## 选题框架（从失败里提炼）

- 关停 11 天后（2019-05-28）发布《Finding My Next Bootstrapped Business Idea》，方法论借自 Jason Cohen：不给想法打分排名，用过滤器淘汰不合格者 [2]。六条过滤器 [2]：
  1. 市场必须已存在（"the market must already exist"——不教育市场）
  2. MVP 几个月内必须能发货（Level 花了一年）
  3. 产品不能是 mission-critical（宕机不该毁掉客户的生意）
  4. 成交不需要超过几个决策人（Level 需要说服整个团队+老板）
  5. 原生 App 不能是最低要求
  6. 市场要与自己已有受众重叠
- 先想清楚动机再选题：可预测、与工时脱钩的舒适家庭收入；做有趣的产品但不想管人；未来能长时间休假 [2]。公司规模是这些约束的后果，不是目标。
- 2020-02-24 再发《10 Questions for Teasing Out Market Opportunities》，其中直指 Calendly 的几问："What successful companies are resting on their laurels?"、"What successful products have critical flaws for a subset of users?"、"What companies have stopped listening to their customers?" [3]。
- 实操动作：把 Drip 运营期间用过的所有软件列成清单，逐一过六条筛子——scheduling 胜出：切换成本低、单人可用（不需要整个团队迁移）、非关键任务、市场已被 Calendly 验证、每个预约链接天然是广告（他在 Drip 亲眼见过 "Powered by Drip" 病毒环的威力）[4]。
- 读了《The Mom Test》后的一句总结："people lie to you"——这次访谈只认行为不认表态 [5]。

## 缝隙切入点

- 楔子是一种情绪，不是一个功能：发日程链接的社交尴尬。PH 发布的 tagline 就一句——"Sending your scheduling link shouldn't feel weird." [6][20]
- "There are some pockets of industry where people just literally refuse to use them because it's just too faux pas."——有整块行业因为"失礼"而拒用日程链接，这是 Calendly 十年没碰的盲区 [5]。
- 论坛考古当雷达：Calendly 用户的抱怨帖"threads just kind of sitting around for a couple of years with no real response"——巨头停止倾听的实证 [5]。"Calendly has hundreds of thousands of customers and millions of people using the product. It's just hard to turn that ship quickly." [5]
- 策略上主动借势而非避战："draft off of a lot of the awareness that they've built up"——Calendly 教育好的市场，他来接不满意的那部分 [5]。

## 时机

- 2020 年初开工（工作名 MightyCal），2020 年 7 月燃尽图 96%、自称 "running out of excuses"；2021 年 1 月上 Product Hunt 正式发布，拿下当月 #2 Product of the Month [4][6][20]。
- 发布同月，Calendly 融资 $350M、估值 $3B——巨头上桌反而把品类蛋糕做大，也坐实了"它必然继续向上市场走"的判断 [12]。
- 2022 年 1 月 26 日 Sam Lessin 引爆 "Calendly 礼仪"论战：发链接是 "a 'get in line' move"，是 "The Most Raw / Naked Display of Social Capital Dynamics in Business" [11]。CNBC、Fortune 等主流媒体跟进，"发日程链接是否失礼"成了全行业议题——恰好是 SavvyCal 立命的那个问题 [12]。Calendly CEO Tope Awotona 公开回应称论战反而带来注册量激增——品类整体受益，而 SavvyCal 是唯一把"礼貌"写进定位的玩家 [12]。

## 差异化

- 定位语把双边体验写进一句话（2026 官网）："The fresh way to find a time to meet. You'll love it for the flexible controls to keep your calendar sane. They'll love it for the ultra-convenient booking experience." [9]
- 机制三件套，全部服务"把'你来排队'变成'我们一起找时间'"：
  1. 收件人日历 overlay——对方可以把自己的日历叠在你的可约时间上看，不用来回切窗口 [9]；
  2. Personalized links——为每个收件人生成带其名字的专属链接，落地页直接称呼对方 [23]；
  3. Single-use links——一次性链接，约完即失效，"给你专门开了一扇门"而不是"进我的公共队列"[24]。
- 对比营销打到功能级：逐条发推对比，如"SavvyCal 每条链接可跨多日历查冲突、指定存入哪个日历；Calendly 所有会议存同一个日历" [21]。
- 不拼功能广度，攻一个 nagging pain point（"the awkward power dynamic of exchanging scheduling links"），配上让人"注册即惊艳"的 UX、免信用卡试用、以及链接底部 "Scheduling by SavvyCal" 的内建病毒环 [6]。
- 早期定位刻意宽："intentionally keeping your positioning pretty broad cause you're trying to have like a big fishing net to capture a lot initially"——先广撒网再收拢 [5]。

## 第一批用户/冷启动

- 受众复用：Art of Product 听众、Twitter、邮件列表——Level 时期攒下的等待名单和多年 build in public 的信任直接变成 SavvyCal 的种子池 [5][6]。
- 用 Mom Test 式访谈切割功能优先级："the majority of people just kind of need to present their availability and all the rest of the stuff it's like nice to have"——先只做呈现可约时间这件事 [5]。
- 约 $1k MRR 时（2020 年底）就用 TinySeed 的钱雇了兼职营销负责人 Corey Haines，创始人专注产品 [6][19]。
- Onboarding 问卷"你从哪听说我们"的高频答案："I used a link with someone else"——病毒环真实在转 [5]。

## 收入与定价

- 公开里程碑：2020 年底 ~$1k MRR [6] → 2021 年中破 $10k（他定义的 "default alive"：能发自己全额工资+覆盖全部成本还有盈余）[5] → 2022 年初破 $20k（团队 3 人）[6] → 此后停止公开。2024 年 Latka 估算 ~$1M ARR，仅第三方估算 [17]。官网社会证明口径："Join over 2,000 happy customers" [9]。
- 定价（2026）：Basic $10/人/月、Premium $17/人/月（加 custom domains、助理代管、付费预约），年付省 2 个月，30 天退款；试用不限时——"Kick the tires for free and only upgrade when you're ready" [10]。
- 融资纪实（重要修正）：SavvyCal 不是零外部资金的 pure bootstrap。Derrick 在 Level 关停后进入 Rob Walling 的 TinySeed 首批（2019）加速器，拿了小额资金外加个别天使支票；这笔钱跟着他的公司从 StaticKit 一路转向到 SavvyCal——TinySeed 官网公告页的 URL 至今还留着中间工作名 "mightycal" [7][8][6]。TinySeed 自我定位是"为 bootstrapper 设计的基金"，不控股、不逼增长，但书稿引用时应写"bootstrap 式小额融资"而非"纯自筹"。

## 内容与增长

- Art of Product 播客（2017–2022，共 220 集，与 Tuple 创始人 Ben Orenstein 合播）：每周直播两家公司进展，Level 的兴衰和 SavvyCal 从 0 到 $20k+ 的全程都有录音存档——公开可查的"创业黑匣子" [14][15]。
- 渠道组合：播客广告（难归因）、SEO 落地页、affiliate 计划、产品自带口碑环 [5]。
- 借高权重域名的外链做 SEO 冷启动（发布期媒体报道的副产品）[6]。
- 工具选型即价值观营销：用 Fathom Analytics 做无侵犯性统计，与目标受众（indie/隐私敏感人群）气味相投 [5]。

## 如何保持小

- 团队 3–4 人：Derrick + 2 名客服（Reggie Rendal、Stephen Lovino）；Corey Haines 后离开自立门户，团队没有回填成建制的营销岗 [7][19]。
- 保持小是选题框架的第一性推论：可预测收入、不管人、能休长假——见"选题框架"节 [2]。
- 2025 年 5 月近况：开辟第二条产品线——面向服务型企业（如远程医疗）的 appointment scheduling，先与一家 agency 合作定制流程，小步试探而非大举扩张 [13]。
- 反潮流的基础设施观：反对早期公司学 Basecamp 下云自建服务器——PaaS 等于"SREs and DevOps people...as a functional extension of your team for metered cost"；TinySeed 204 家被投公司里只有 1 家有正当理由自购硬件 [13]。
- AI 工具（2025）：日常用 Windsurf/Cursor，承认 AI 大幅缩短 MVP 周期，但对纯 AI 生成代码库的长期可维护性存疑；最看好 AI 写测试和边界分析 [13]。

## 开放问题（值得当面问创始人的）

1. 当前真实 MRR 和增长率是多少？为什么在 $20k（2022 初）之后停止公开数字——和 Transistor 在相近量级停播收入是同一个原因吗（公开数字开始伤害谈判/招聘/心态）？
2. TinySeed 的支票具体多大、什么条款？这笔"跟着创始人转向"的钱在 StaticKit→SavvyCal 两次转向中起了什么作用——如果没有它，第三次尝试还存在吗？
3. Calendly 此后几年用免费层+品牌投放向下渗透，SavvyCal 的新增/流失实际受了多大冲击？被"礼貌楔子"吸引来的用户，长期留存是否真的显著更好？
4. Level 有 6,000 人等待名单、500 场访谈，全是假阳性。SavvyCal 立项时他设计了什么"反向验证"来对冲访谈对象说谎？今天再看，六条过滤器里哪条其实是幸存者偏差？
5. 2025 年开 appointments 第二曲线，是单产品增长见顶的信号，还是从容的相邻扩张？他判断"该扩张了"的触发指标是什么？

## 来源

1. https://www.derrickreimer.com/walking-away （2019-05-17，Level 关停复盘长文）
2. https://www.derrickreimer.com/finding-ideas （2019-05-28）
3. https://www.derrickreimer.com/market-opportunities （2020-02-24）
4. https://www.startupsfortherestofus.com/episodes/episode-506-shutting-down-and-starting-up-with-derrick-reimer （2020-07-21）
5. https://www.indiehackers.com/podcast/210-derrick-reimer （2021 年中，Indie Hackers Podcast #210）
6. https://producthunt.com/discussions/i-launched-savvycal-to-2-product-of-the-month-in-january-and-have-since-crossed-20k-mrr-ama （2022 年初，PH AMA）
7. https://savvycal.com/company
8. https://tinyseed.com/latest/2019-batch-announcement-mightycal （2019-09-03，注意 URL 中的旧名）
9. https://savvycal.com/ （2026-07 快照）
10. https://savvycal.com/pricing （2026-07 快照）
11. https://x.com/lessin/status/1486477359717187589 （2022-01-26）
12. https://www.cnbc.com/2022/02/07/what-is-calendly-.html （2022-02-07）
13. https://www.startupsfortherestofus.com/episodes/episode-775-a-i-coding-tools-user-experience-racking-your-own-servers-and-more-listener-questions-with-derrick-reimer （2025-05-20）
14. https://podcasts.apple.com/us/podcast/the-art-of-product/id1243627144 （Art of Product，2017–2022，220 集）
15. https://www.derrickreimer.com/work
16. https://www.prnewswire.com/news-releases/drip-acquired-by-leadpages-300297707.html （2016-07）
17. https://getlatka.com/companies/savvycal.com （2024 年第三方估算，低置信）
18. https://github.com/levelhq/level （Level 源码库）
19. https://thebootstrappedfounder.com/corey-haines-mastering-product-marketing/
20. https://www.linkedin.com/posts/derrick-reimer-93916020_savvycal-sending-your-scheduling-link-shouldnt-activity-6752866289661952001-rE7Q （2021-01，PH 发布帖）
21. https://x.com/derrickreimer/status/1334176410605412352 （2020-12，对比营销示例）
22. https://x.com/derrickreimer/status/1129419549487427584 （2019-05-17，关停官宣）
23. https://docs.savvycal.com/article/14-personalizing-links
24. https://changelog.savvycal.com/single-use-links-196557 及 https://docs.savvycal.com/article/30-single-use-links
