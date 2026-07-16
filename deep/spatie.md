# Spatie（Freek Van der Herten 等）

> 比利时安特卫普的 Laravel 小作坊：一边接客户项目，一边把项目里的可复用件拆成开源包，20 年只长到 ~11 人，却成了 Laravel 生态最大的第三方包供应商 ｜ spatie.be ｜ Willem Van Bockstal 2004–05 年独自创办，2009 年 Freek Van der Herten（技术）与 Jef Van der Voort（客户）加入成三人合伙 [16][17][5] ｜ 537 个开源包、26.6 亿次下载（约每月 4500 万次，2026-07）[1][2] ｜ 收入 = 客户项目 + 付费产品（Ray/Flare/Mailcoach）+ 视频课程，全自筹、无融资

## 缝隙切入点

Spatie 起点毫无传奇色彩：设计师 Willem 的单人设计小店，2009 年拉来两个朋友——做了七年银行 COBOL 程序员的 Freek 和做客户关系的 Jef [4][17]。公司名取自荷兰语"空格"："Spatie is in-between everything, cause 'spatie' in Dutch means the whitespace between words" [5]。

转折点是两个外部输入的叠加。2013 年 Freek 通过 Dries Vints 的一篇博客发现 Laravel，把公司从 Zend Framework 1 迁了过去——"I was immediately blown away by how much better Laravel handled things such as creating routes than Zend" [1][5]。2014 年 3 月，他看了 Jeffrey Way 在 Laracasts 上讲包开发和 Travis CI 的教程，做出第一个包 Browsershot（PhantomJS 封装）[1][3]。此后一发不可收："In the beginning it was really crazy, I think I released a package every week or every two weeks" [5]。

真正的缝隙不是某个产品点子，而是一条生产纪律：**所有包都从客户项目里长出来**。"Currently every new package that we create gets born inside a client project. When we feel like we can make something we can reuse ourselves and share with the community the decision is often made to just make a package out of that functionality" [3][6]。客户付钱解决一次的问题，被抽象成全世界复用的资产——同一份劳动卖两次：一次卖给客户，一次换成声誉。

## 时机

- Laravel 2013–2015 年正处爆发前夜，生态里"框架很好用、周边件奇缺"，谁先批量填坑谁就占住命名空间——今天 Laravel 开发者说"用 spatie 那个包"几乎成了口头禅。
- Composer/Packagist 让 PHP 包分发成本降到零；Laracasts 把"怎么写包"变成了可学的手艺 [1][3]。
- 下载曲线跟着生态复利：2017 年约 800 万次（170 个仓库）[3]，2020 年底破 1 亿 [7]，2021 年底 2.15 亿 [8]，2026 年 26.6 亿+ [2]——后期增长大头来自 CI 流水线时代整个 Laravel 生态的膨胀，Spatie 是生态贝塔的最大受益者之一。

## 差异化：包工厂的生产系统

Spatie 的独特资产不是任何单个包，而是一套可持续二十年的"农产品式"生产系统：

- **4+1 排期**（外界常误传为"4 天工作制"，需澄清：他们每周工作五天，但只排四天客户活）："When scheduling out to the coming week we only plan four days. So we have one work day we can be a bit flexible with"——第五天做开源、实验或自己的项目，这个制度从 2014 年前后持续至今约十年 [1][3][6]。配套政策是不加班（no overtime）。
- **维护上的"绝情"纪律**：只支持最新版 Laravel 和 PHP，旧版本一律不管 [4]；Freek 的心态是 "I've also learned to sometimes just let it go… I'm not obliged at all to do this kind of work unless I'm very happy to do it myself" [4]。这是 11 个人扛住 537 个包、12,000+ issue、18,000+ PR 的前提 [1]。
- **社区当共同生产者**：laravel-fractal "90% of the code of that package was written by the community" [6]；全部包累计 1,000+ 贡献者 [2]。
- **Postcardware**：许可证仍是 MIT，但附一条友好请求——包上了生产环境，请从家乡寄张明信片到安特卫普，最好的明信片贴在官网上。2018 年每月能收 15–35 张 [4][19]。零成本把匿名下载量变成看得见摸得着的人情连接，也是被 HN 热议的免费传播事件 [19]。
- **内部规范公开化**：guidelines.spatie.be 把公司的代码与协作规范整站开源，"The guidelines used at our company" [20]——手册本身又成了招聘和品牌素材。

代表作的分量：spatie/laravel-permission 单包安装量 1.05 亿次（2026-07），是 Laravel 第三方包里的顶流 [15]；他们做的错误页 Ignition 从 Laravel 6（2019）起被官方设为**默认错误页**——每一个新建的 Laravel 应用都自带 Spatie 的代码 [9]。

## 收入与定价

开源本身不收一分钱（无双许可、无付费版包），变现走三条腿。客户项目长期是大头：2020 年"about 30% of our total time was spent on our own products and 70% on client stuff"，且"all of these products are profitable" [7]。策略上只接长周期大项目："We don't do projects with a short deadline anymore, because you can't really experiment or learn too much in such a time"（客户包括 Tomorrowland 音乐节）[5]。

产品与课程时间线（有出处的数字）：

| 时间 | 产品 | 已知数字/事实 |
|---|---|---|
| 2019.08 | Flare（Laravel 错误追踪 SaaS），与 Ignition 一起 6 个月造完，在 Laracon EU 上以"Apple 发布会"方式亮相 [9] | 2021 年"significant uptick in MRR… according to our expectations" [8] |
| 2020 初 | Mailcoach（自托管邮件营销，Laravel 应用/包）| "After a few weeks, all development costs were already earned back" [7]；卖点是按发信量而非联系人数收费，对大列表比 Mailchimp 省 €200–1,000/月 [12] |
| 2019–2021 | 课程线：Laravel Package Training、Laravel Beyond CRUD、Front Line PHP、Testing Laravel、Event Sourcing in Laravel | Laravel Beyond CRUD 是"our best selling course"；Front Line PHP"a commercial success"；Event Sourcing 定价更高、销量一般 [7][8] |
| 2021.01 | Ray（桌面调试工具，直播发布）| 首年"We sold thousands of licenses and reached revenue numbers with six digits" [8]；现价年费 $41、限时买断 $167，免费试用每次会话 20 条消息 [14] |
| 2022.10 | Mailcoach Cloud（托管版）| 转云原因："Mailcoach was hard to install for people without a technical background" [13] |
| 2025.10 | Flare 性能监控上线 | 开发耗时 20 个月 [10] |

公司整体营收从未披露；能确认的只有"产品全部盈利 + Ray 首年六位数"这个量级。另注：Freek 个人还与 Mattias Geniar 合伙做监控 SaaS Oh Dear（2018，Spatie 体外），MRR 连续数年翻倍或更好 [4][7][8]。

## 内容与增长

- **Freek 的博客是整个飞轮的轴**。freek.dev（前身 murze.be）2014 年开写，五周年时累计 1,509 篇、最后一年发 292 篇（其中 45 篇原创，其余是高频率的链接推荐——"高产"的真相是原创+策展混排）[21]；2020 年全年约 94 万 pageviews [7]。newsletter 9,500+ 订阅 [22]。他在多档播客反复现身（Laravel Podcast 至少三期）[4]，但并不自己主持播客——这点与传闻不符。
- 博客直接带货："the more people we get to visit our products page, the more sales we have"；2020 年把所有产品收拢到 spatie.be 自营销售 [7]。
- 发布会式上新：Flare 在 Laracon EU 舞台首发 [9]，Ray 用直播发布 [8]——每次上新都是打给既有受众的，冷启动问题在多年内容积累里已提前解决。
- 线下枢纽：从 Antwerp PHP meetup 做到 Full Stack Belgium，再到 2019 年与 Dries Vints、Rias Van der Veken 共同创办 Full Stack Europe 会议（安特卫普）[18][5]。
- 2016 年 Freek 对开源获客的评估还很克制："Recently we've landed some clients because of our open source work"，多数客户仍来自过往案例 [6]；到 2017 年已变成"The past year we've landed some cool projects because of our open source work" [3]。获客是慢变量，声誉先行。

## 团队与如何保持小

- 规模曲线：2009 年 3 人 [17]，2018 年 8 人（5 开发 + 1 设计 + 1 PM）[4]，2018 年做 Flare 时 7 人，2025 年 11 人 [10]，官网现列 13 名成员（含客户经理与支持工程师）[16]。二十年翻了四倍不到——与 26.6 亿下载量形成本案例库里最悬殊的"影响力/人头比"之一。
- 挑人标准是"passionate people"，公司刻意只维持"a few big clients that are technically challenging" [5]。
- 混合办公，约一半时间进办公室；不加班文化 + 第五天制度是留人手段也是产能来源 [1][3]。
- 人才外溢成了生态贡献：写出 Laravel Beyond CRUD 的 Brent Roose 在 Spatie 干了近 5 年后被 JetBrains 挖去做 PhpStorm 布道师 [24]——小作坊当不了终身雇主，但能当职业生涯的放大器。
- Flare 团队 2025 年的自省文帮我们看到小团队的真实代价：客户活不断把人从产品上抽走，"classic project management traps: scope creep, underestimating tasks, optimistic planning, losing momentum, perfection paralysis"；甚至在 Laracon EU 2024 发现"很多参会者根本不知道 Flare 存在"——高估了自己的品牌认知 [10]。

## 转型与平台风险

Spatie 的枢纽地位建立在别人的平台上，2024 年起两面受压：

- **平台自己下场**：Laravel 公司 2024 年 5 月拿了 Accel 5,700 万美元，随后把 Spatie 的 Ignition 从默认错误页里换掉，又推出自家监控产品 Nightwatch 直接与 Flare 竞争。Flare 团队坦承这"forced difficult internal discussions but ultimately motivated better product decisions" [10]。依附生态的红利与风险是同一枚硬币。
- **AI 拆解"装包"这个动作本身**：2026 年 4 月 Sebastian De Deyne 发文《The robots are replacing the packages》，判断 AI agent 把问题从"Should I use a package?"变成"Do I want to own this problem?"——"Installing a Laravel package takes thirty seconds. Writing a solid implementation takes time. But with AI-assisted development, time isn't as much of a factor because the writing happens in the background." 他给出包仍然成立的三类场景（多年边角案例沉淀的难问题、替你扛外部 API 变更的维护负担、体现作者品味的方案），其余的："we'll happily sunset those packages and aim our sights at more interesting problems" [11]。
- 公司同步转向：官网主张已改为"Websites & web applications in Laravel & AI"，2026 年博客几乎全在写 AI 辅助开发（用 Claude Skills 做客户项目、AI 读代码而非生成代码等）[25]；Freek 博客副标题也从"Laravel and PHP"改成"Laravel, PHP and AI" [22]。回应方式与当年做包一致：先在客户项目里用新东西，再把心得公开化。

## 开放问题（值得当面问本人的）

1. 2026 年的收入结构里，客户项目、产品、课程各占多少？2020 年"30% 时间做产品"的比例现在是多少——产品养得起团队了吗，还是客户活仍在补贴一切？
2. Laravel 官方拿 VC、换掉 Ignition、推出 Nightwatch——枢纽位置被平台自己挤压时，你们内部"difficult discussions"的结论是什么？有没有认真考虑过跨出 Laravel 生态？
3. AI 让 agent 现写代码替代装包，537 个包的下载曲线预计何时见顶？"乐意 sunset"之后，Spatie 下一个可防守的资产押在哪——品味、课程、Flare，还是 AI 时代的新工具？
4. 二十年停在 11 人：最接近扩张/融资/被收购的一次是什么时候？客户工期紧张时，"只排四天"和第五天制度靠什么活下来？
5. 公开叙事里几乎只有成功产品——哪些产品或课程没赚回成本？判断"该停"的标准是什么？

## 来源

1. Story of a billion downloads（Spatie 官方时间线站）— https://1billion.spatie.be/
2. Spatie: Committed to open source（537 包 / 26.6 亿下载 / 1,000+ 贡献者）— https://spatie.be/open-source
3. Freek Van der Herten, The story behind our open source efforts（2017）— https://freek.dev/947-the-story-behind-our-open-source-efforts
4. The Laravel Podcast: Interview: Freek Van der Herten, Lead Developer at Spatie（2018-07，transcript）— https://laravelpodcast.com/episodes/db8ee53b/transcript
5. Agiledrop 访谈 "Living the dream with Spatie" — https://www.agiledrop.com/blog/interview-freek-van-der-herten-living-dream-spatie
6. Laravel Daily 访谈 "80 Laravel packages?! WOW!"（2016-09）— https://laraveldaily.com/post/80-laravel-packages-wow-interview-freek-van-den-herten-spatie
7. Freek Van der Herten, A recap of 2020 — https://freek.dev/1863-a-recap-of-2020
8. Freek Van der Herten, A recap of 2021 — https://freek.dev/2155-a-recap-of-2021
9. Flare blog, Running Ignition on five years of Laravel — https://flareapp.io/blog/running-ignition-on-five-years-of-laravel
10. Flare blog, Lessons from the deep end（2025-10-02）— https://flareapp.io/blog/lessons-from-the-deep-end
11. Sebastian De Deyne, The robots are replacing the packages（2026-04-30）— https://spatie.be/blog/the-robots-are-replacing-the-packages
12. Freek Van der Herten, Building Mailcoach（2020）— https://freek.dev/1558-building-mailcoach
13. Freek Van der Herten, Mailcoach Cloud is now available（2022-10-26）— https://freek.dev/2363-mailcoach-cloud-is-now-available-affordable-email-marketing-for-bloggers-artisans-and-entrepreneurs
14. Ray 产品页（定价）— https://spatie.be/products/ray
15. Packagist: spatie/laravel-permission（1.05 亿安装，2026-07）— https://packagist.org/packages/spatie/laravel-permission
16. Spatie About us（成立年份、团队名单）— https://spatie.be/about-us
17. Freek Van der Herten, An interview with Jef, Spatie's account manager（2017）— https://freek.dev/827-an-interview-with-jef-spaties-account-manager
18. Announcing the Full Stack Europe conference（2019）— https://freek.dev/1123-announcing-the-full-stack-europe-conference
19. Our packages are now postcardware + 官网明信片墙 + HN 讨论 — https://freek.dev/531-our-packages-are-now-postcardware ／ https://spatie.be/open-source/postcards ／ https://news.ycombinator.com/item?id=15498717
20. spatie/guidelines.spatie.be（公司规范整站开源）— https://github.com/spatie/guidelines.spatie.be
21. freek.dev turns five!（博客五周年数据）— https://freek.dev/1510-freekdev-turns-five
22. freek.dev About（300+ 包、20 亿下载、newsletter 9,500+、Oh Dear）— https://freek.dev/about
23. Spatie 官方 newsletter "Let's talk about Ray"（Global Ray、免费月度 license）— https://spatie.mailcoach.app/webview/campaign/d6a2398e-eb03-4826-b5fe-a408182a2ca4
24. Brent Roose, Goodbye（离开 Spatie 加入 JetBrains）— https://stitcher.io/blog/goodbye
25. Spatie 官方博客（2025–2026 AI 主题密集）— https://spatie.be/blog
