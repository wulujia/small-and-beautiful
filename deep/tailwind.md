# Tailwind Labs（Tailwind CSS）

> 开源 CSS 框架自带流量，靠卖"设计品位"（Refactoring UI 电子书 + Tailwind UI/Plus 组件库，全部一次性买断）自养 ｜ tailwindcss.com ｜ Adam Wathan & Steve Schoger ｜ 2017 年开源框架 / 2019 年全职公司 ｜ 峰值 8 人，2026 年 1 月裁员后约 5 人 ｜ pure-bootstrap / 开源+付费周边 / audience-first ｜ 2020 年起"reliably mid-seven figures per year"；2023 年初收入见顶，2026 年 1 月披露因 AI 较峰值跌约 80%

## 缝隙切入点

- Tailwind CSS 是副产品的副产品：Adam 直播开发一个从未上线的 SaaS（KiteTail），观众反复追问他 HTML 里那套 utility class 从哪来，问的人多了他才在 2017 年 11 月 1 日发布 v0.1.0 [1][17]。"I really believed that's what I was doing（做 KiteTail）, which I think is the only reason that I did the live streaming" [17]——框架从来不是他计划中的生意。
- 真正的商业缝隙是"不懂设计的开发者"：会写代码、想把产品做好看、但请不起设计师。Refactoring UI（2018 年 12 月）卖的就是把设计师 Steve Schoger 的品位拆解成开发者能执行的规则 [2][3]。
- Adam 入场前已经有一个信息产品生意：第一本书 Refactoring to Collections（2016）首周卖了 $61,392，当时他只有约 3,500 个 Twitter 粉丝、1,500 个邮件订阅 [6]；Test-Driven Laravel 课程累计超 $100 万，Advanced Vue 约 $30 万 [6]。开源框架是插在这台已验证的变现机器上的。

## 时机

- 顺风期（2017–2022）：框架安装量 2018 年 67 万次 [2] → 2019 年累计约 400 万 [7] → 2020 年 7 月累计 1,000 万 [1] → 2020 年底累计 1,900 万、每月 200 万+ [5]。开源增长直接抬升付费产品销量（见"内容与增长"）。
- 逆风期（2023–2026）：同一个漏斗反向坍塌。LLM 替开发者写 Tailwind 代码，文档流量从 2023 年初的峰值跌了约 40%，而框架使用量"growing faster than it ever has"——用的人更多，进官网看到付费产品的人更少 [10][11]。同一条护城河，前一个时代是发动机，后一个时代成了故障点。

## 差异化

- 商业结构：框架本体 MIT 开源永远免费，收费的是框架之上的"品位层"——电子书（Refactoring UI）、官方组件与模板（Tailwind UI，2025 年 3 月更名 Tailwind Plus）[1][9]。卖的不是功能是设计能力，这部分 LLM 时代之前无法被抄——因为竞品缺的是 Steve，不是代码。
- 定价姿态：全线一次性买断、终身访问、明确"no subscription"[9]；Tailwind Plus 个人 $299、25 人团队 $979 [11]。不做 Black Friday 促销："I try to put our marketing effort into things with a long-term pay-off" [6]。
- 对外合作全部拒绝："We get so, so, so, SO many messages about partnerships...and we say no to every single one" [6]。

## 第一批用户/冷启动

- 受众先行是显式战略：决定做 Refactoring UI 后，两人花了两年先养 Steve 的 Twitter（起点接近零粉丝），用设计 hot tips 建立信任再发书 [6]。单条 tip 会打磨两周近全职投入，换来 5,000 转推、15,000 赞 [6]。
- Adam 自己的分发渠道：Full Stack Radio 播客 2018 年月下载 8 万+ [2]。
- Refactoring UI 上线（2018-12）：两周卖出 6,000+ 份 [2]，约一个月毛收入超 $135 万 [3]。
- Tailwind UI 上线（2020-02-26 早期访问）：首日 $40 万 [5]——受众池直接变现，没有冷启动期。

## 收入与定价

- Refactoring UI：定价 $79 / $149 两档，78% 的买家选了贵的"Complete Package"（贵档才有完整内容，锚定设计刻意为之）[3]。累计：2020 年 8 月 $230 万 [4] → 2022 年 9 月超 $250 万 [6]；仅 2020 一年就卖了 $60 万，"perennial seller" [5]。
- Tailwind UI："首年 $2M+" 基本成立且更快——上线 5 个月即 $197 万 [4]（Adam 原话："$2.3m Refactoring UI, $1.97m Tailwind UI, really simple just two one-time sale products" [4]）；2022 年口径"doing seven figures per year and growing" [6]。
- 公司整体：2020 年 8 月"over $4m in revenue in under 2 years" [1]；2020 年底"We're reliably doing mid-seven figures per year" [5]。收入 2023 年初见顶，之后累计下滑约 70–80%（见"转型"）[10][15]。
- 一次性买断的代价事后暴露：终身授权 + 老客户免费升级 [9] 意味着存量客户不再贡献现金流，新增流量一断收入就断。Adam 2026 年复盘是否后悔没做订阅："I honestly don't think so"，但承认企业授权（enterprise licensing）本可以帮上忙 [15]。

## 内容与增长

- 开源就是营销部门：Adam 确认发版、发性能基准的当天销量可测量地上涨——"releasing open-source updates directly correlates with sales increases" [17]。公司不投广告、没有销售，文档站是唯一漏斗 [10][11]。
- v4（2025-01-22 发布）延续了"性能即内容"打法：完整构建快 3.78 倍、增量构建微秒级，这些数字本身就是传播素材 [8][17]。
- 做内容的成本被严重低估：Tailwind UI 开发期（2019-09 起与 Steve 合作，年底攒出 100+ 组件）被 Adam 称为"the most frustrating, morale-destroying project I've ever worked on" [7]。

## 转型（AI 冲击，2023–2026）

- 2025-11-18，Adam 拒绝了一个让文档对 LLM 更友好的社区 PR，理由写得很直白："Making it easier for LLMs to read our docs just means less traffic to our docs which means less people learning about our paid products" [11]——护城河与生态利益第一次公开冲突。
- 2026 年 1 月初裁掉 4 名工程师中的 3 名（占工程团队 75%）：假期做财务预测发现"if nothing changed, then in about six months we would no longer be able to meet payroll obligations" [10]。他在自己的播客 Adam's Morning Walk 以一期《We had six months left》公开全过程，告别的三人是 Philipp、Jordan 和 Dan，均给了优厚遣散 [12]；Philipp Spiess 入职仅一年半 [13]。合伙人 Jonathan Reinink："having to say goodbye to three brilliant people here at Tailwind Labs was absolutely gutting" [14]。
- 危机的荒诞结构：用量涨到历史最快、收入却跌了近 80%——Adam 担心 Tailwind 沦为"unmaintained abandonware" [10]。社区归因还包括 shadcn/ui（2023-09 起免费组件直接对撞 Tailwind Plus）和缺官方 Figma 插件，但这些是 HN 分析，非官方口径 [20]。
- 自救与反转：播客爆火后 Vercel、Google AI Studio 成为新赞助商 [10]，Gumroad 跟进 [11]，社区自发买授权声援 [11]；Adam："Overwhelmed by the support over the last 24 hours" [18]。到 2026 年 3 月，赞助收入已能覆盖公司开支 [15]。
- 新赌注：ui.sh——增强 AI 生成前端代码能力的工具，把"给人看的文档漏斗"换成"给 agent 用的工具漏斗" [15]。Adam 本人退回 IC 写代码，用 AI 做 issue 分诊和运维 [12]。

## 如何保持小

- 从未融资，无任何外部资本记录；团队巅峰也只有 8 人 [15]（2022 年 7 人 [6]，2020 年一年招了 4 人：Brad Cornes、Robin Malfait、Simon Vrachliotis、David Luhr [5]）。裁员后约 5 人：三位共同所有人（Adam、Steve、Jonathan Reinink）+ 工程师 Robin Malfait + 运营 Peter Suhm [10]。
- 保持小是价值观不是阶段："I'm optimizing for maximum freedom and a fun and happy life. Pulling more people in any way doesn't help us get to that goal...it slows us down" [6]。自知之明："I don't think I'm a great manager even though I try hard at it, and it's very draining for me" [6]。被问超过 10 人会怎样，他直言怀疑规模化后还能不能保住质量 [17]。
- 招人极重：2024 年两个岗位收到 1,600+ 份申请，Adam 花两个月全职筛选（"basically my full time job for 2 months"），最后录取的两人都不是走申请通道，而是从已有人脉里来的 [16]。工程师薪酬据报道在 $25–30 万总包 [19]；Adam 说员工从没主动要求过加薪——因为公司多次先给 [15]。
- 注意：没有查到 Adam"拒绝过具体 VC 报价"的直接引语。书稿只能写"从未融资、拒绝一切合作请求 [6]"，不要写"多次拒绝 VC"。另外高分配（高薪+一次性买断收入全消化）与只剩 6 个月现金 runway 之间的关系，是这个案例的暗面，值得写。

## 开放问题（值得当面问创始人的）

1. mid-seven figures 跑了三四年，利润去了哪里（工资/分红/储备的比例）？为什么没有留出超过 6 个月的现金缓冲——是刻意的"利润即分掉"哲学，还是没料到断崖？
2. 如果 2021 年把 Tailwind UI 转成订阅制，AI 冲击会不会只是增长放缓而非生存危机？他承认 enterprise licensing 本可帮上忙——当年为什么没做？
3. 文档流量 -40% 的归因拆解：LLM 代写、Google AI Overviews、shadcn/ui 分流各占多少？内部有没有分层数据？
4. 拒绝"LLM 友好文档" PR 是护城河还是逆潮流？半年后回头看，这个决定他还会做吗？
5. ui.sh 收谁的钱——开发者、AI 公司还是平台？"给 agent 做工具"的漏斗里，开源框架的品牌还值多少钱？

## 来源

1. https://adamwathan.me/tailwindcss-from-side-project-byproduct-to-multi-mullion-dollar-business/ （2020-08-02）
2. https://adamwathan.me/2018-year-in-review/ （2018-12）
3. https://marketingexamples.com/landing-page/pricing （Refactoring UI 定价复盘）
4. https://x.com/adamwathan/status/1289702466754211842 （2020-08-01）
5. https://adamwathan.me/journal/2020/12/29/2020-year-in-review/ （2020-12-29）
6. https://www.indiehackers.com/post/im-adam-wathan-i-created-tailwind-css-and-built-a-multi-million-dollar-business-around-it-ama-3c0732f724 （2022-09-13 AMA）
7. https://adamwathan.me/journal/2019/12/06/2019-year-in-review/ （2019-12-06）
8. https://tailwindcss.com/blog/tailwindcss-v4 （2025-01-22）
9. https://tailwindcss.com/blog/tailwind-plus （2025-03-04）
10. https://devclass.com/2026/01/08/tailwind-labs-lays-off-75-percent-of-its-engineers-thanks-to-brutal-impact-of-ai/ （2026-01-08）
11. https://socket.dev/blog/tailwind-css-announces-layoffs （2026-01）
12. https://podwise.ai/episodes/6735732 （Adam's Morning Walk：《We had six months left》，2026-01-07）
13. https://x.com/PhilippSpiess/status/2008852246847754469 （2026-01）
14. https://x.com/reinink/status/2009305569291849885 （2026-01）
15. https://www.startupsfortherestofus.com/episodes/episode-825-talking-tailwind-css-and-founder-fitness-with-adam-wathan （2026-03-24）
16. https://saas.transistor.fm/episodes/adam-wathan-on-hiring-for-a-small-startup-tailwind-css （Build Your SaaS，2024-06-04）
17. https://podcast.tuple.app/episodes/adam-wathan/transcript （2024）
18. https://x.com/adamwathan/status/2009340684210159812 （2026-01）
19. https://ppc.land/tailwind-css-lays-off-75-of-engineering-team-as-ai-impacts-revenue/ （2026-01）
20. https://news.ycombinator.com/item?id=46527950 （HN 讨论，社区归因）
