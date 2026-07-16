# LobeChat（LobeHub）

> 给想自己掌控 AI 的人一个"比官方更好看"的开源 ChatGPT，再长成 Agent 运营平台 ｜ lobehub.com ｜ 创始人：空谷 Arvin Xu（另有联合创始人，GitHub: canisminor1990）｜ 2023 ｜ 团队公开可见 ≤10 人 ｜ 开源 + SaaS 订阅（LobeHub Cloud）｜ 营收：仅 2024-08 公开过 $1000+ MRR（58 个付费用户），此后未披露

## 缝隙切入点

起点是创始人自己的痛。空谷："其实我做 LobeChat 的一个原因就是第一个用的 ChatGPT 账号被封……当我意识到这个号里那些非常有价值的对话永远也找不回来的那一刻，我才发现 Local First 有多重要" [13]。2023 年 5 月 21 日建仓 lobe-chat [1]，切的缝隙是：数据在自己手里、填自己的 API key、一键免费部署的"私有 ChatGPT"——但和满地的 ChatGPT-web 套壳不同，它把"modern-design（现代设计）"直接写进仓库简介 [1]。组织名的野心藏在名字里：Lobe 是脑叶，Hub 是枢纽，"我们希望在应用端（UI 界面层）成为各种 LLM 的连结枢纽。我们在 LobeChat 中做的很多看似吃力不讨好的工作，都是围绕这个意图展开的" [14]。

## 时机

- Star 曲线的起飞不在建仓时，而在 2023 年底到 2024 年初：2023-09-24 仅 433 star → 2023-12-10 为 4,377 → 2024-03-01 冲到 21,153 [6]。恰逢多模型时代开启（Gemini / Ollama / 开源模型井喷），"多供应商 + 自部署"从极客玩具变成刚需。
- 之后靠大功能持续拉升：知识库发布一周后破 40K（2024-09，四个月涨 1 万）[15]；2024-12-30 为 50,391；2025-07-01 为 62,981 [6]；2026-07-16 达 79,893 star / 15,596 fork [1]。
- 2024 年中上线 Cloud，接住"不想折腾 API key"的外溢人群 [2]；2025 年底赶在 Agent 浪潮转型（见"转型"）。

## 差异化

设计驱动是基因不是口号：空谷的自我身份是"Design Engineer"，Ant Design 核心成员、前蚂蚁集团，浙江大学工业设计工程硕士 [17]；团队博客作者 René Wang 的头衔同样是 Design Engineer [10]。技术栈自建了与 antd 配套的整套设计资产（Lobe UI、antd-style）[24]。空谷对自家产品的清醒定位："在开源版里 LobeChat 的整个产品体验能排到第一梯队，但我们的 Cloud 在成熟的商业产品 ChatGPT/Claude/Poe 这些老大哥面前还是个弟弟" [2]。另外两个差异化选择：拒绝国内号商流行的"OneAPI + 一堆 WebUI"拼装模式，坚持自研 Stripe 接入和完整闭环体验 [2]；把贡献者体验当产品设计——新增一个模型 Provider 的 PR 指南"100 行童叟无欺" [18]。

## 第一批用户/冷启动

纯 GitHub 冷启动：开源仓库 + 一键 Vercel 部署，没有投放。Cloud 公测第一个月 7k+ 注册用户主要来自开源社区"注册 Cloud 也就是来捧捧场"，付费转化率不到 1% [2]。空谷的判断很直白："我们选择开源之时，就觉得会去 GitHub 上找开源方案的人，大概率都是白嫖怪（包括我们自己也是）……为 Cloud 付费的用户也基本不来自开源社区，用户是完全不同的两个群体" [2]——这成了他敢把核心功能持续开源的依据。

## 收入与定价

- **第一个里程碑**（2024-08-16，公测一个月）：$1000+ MRR，总营收约 $4k+（3 万人民币），付费用户 58 人。空谷原话："达成 $1000 MRR 订阅的用户数，只需要 58 人。我在回顾看到这个数据时，突然真切地感觉到宏大叙事的薄纱被刺破了……只需要能获得一千到两千名愿意为我们持续付费订阅的用户，就可以让我们这个团队长久稳定地运作下去" [2]。
- **成本结构**：AI API 成本占一半以上（"感觉是在给大模型厂商打工"），基础设施每月大几百刀，第一个月基本只是打平略盈 [2]。
- **定价踩坑**：照抄主流的固定用量订阅制，结果重度用户几天耗尽额度、多轮对话 token 累积让用户"体感被骗"；随即改为"较低的基础订阅费 + 按需购买用量"，并主动为受影响用户重置额度 [2]。
- 2024-11-03 宣布到达第二个收入里程碑，但拒绝披露数字（"免得看着像在贩卖焦虑"）[3]。
- **现行定价**（2026-07 检索）：Free 每月 50 万 credits；Starter $9.9/月、Premium $19.9/月、Ultimate $39.9/月（年付价，月付分别为 $12.9/$24.9/$49.9），另有可加购的 credit 包和私有部署的企业版；credits 按模型 token 换算 [5]。
- 无公开融资记录（Tracxn，2026）[16]；商业主体为 LobeHub LLC [7]。

## 内容与增长

- **透明复盘本身就是获客内容**：两条商业化复盘 thread 被大 V 宝玉整篇转述扩散 [4]，"小而美也能实现商业可持续、58 人达成 $1000 MRR"成了中文独立开发者圈的经典案例。
- **增长引擎是功能发布，不是营销**："每一个大功能都能带来一些新的用户群体：8 月上新的知识库，9 月上的 Artifacts，都带来了很大一波增量用户。而由于 10 月没有做新功能……增速可以看到明显放缓了"，由此定下"一个月一个大 feature"的迭代节奏 [3]。
- 每周发布公开日志 Lobe Open Log（LOL），"做了什么、坏了什么、想法变了什么"全公开 [10]。
- 2026-05 Product Hunt 当日第一（Product of the Day），靠存量用户投出来的 [10]。
- 一个反差数字：GitHub 近 80k star，但 X 官号 2026 年 6 月才突破 5,000 粉 [12]——增长发生在代码分发渠道，不在社交媒体。
- 企业侧：2024-07 与 Master Concept 达成战略合作进入企业级市场 [20]。

## 社区

79,893 star / 15,596 fork（2026-07-16）[1]，是同赛道 star 最高的开源项目之一。社区运营的几个硬动作：把加 Provider 的贡献门槛压到 100 行代码 [18]；核心功能持续开源反哺——知识库全量开源，Cloud 独占的搜索插件也承诺后续开源 [2]；事故极端透明——2026-05 供应链攻击导致仓库所有 issue 被关闭、2026-07 官方 X 账号被 OAuth 钓鱼劫持，两次都发长文复盘 [10][21]。

## 留存

- 漏斗数据（各时点）：Cloud 上线三个月累计 2.4 万注册，Clerk 实际计费的活跃 MAU 约 3,000 [3]；首月 7k+ 注册对应 60+ 付费 [2]。
- 留存承诺是"前沿模型 day-one 可用"："The day a frontier model lands, you should be able to use it here——not next sprint, not next month" [11]。
- 对产品设计缺陷造成的用量损失主动兜底（重置额度），"这些额外的用量损失理应由我们承担" [2]。

## 转型

三段式：开源 Chat UI（2023）→ Cloud SaaS（2024）→ Agent 运营平台（2025-2026）。

- **许可证随商业化演进**：MIT → Apache 2.0（2024-03-28）[8] → 1.0 起改为 LobeHub Community License（2024-06-17，Apache 2.0 基础上加一条：直接商用可以，基于源码做衍生分发需购买商业授权）[7]。
- **Cloud**：2024 年年中公测，与开源版"递进"——开源管产品力，Cloud 管增值服务和运营 [2]。
- **CAO 大转向**：2025 年底 LobeHub 以"agent teammates"重新发布；2026-05-18 发布 LobeHub 2.2，定位改为"你的首席 Agent 运营官（Chief Agent Operator）"，并把这个 80k star 的仓库直接从 lobe-chat 改名为 lobehub [9][1]。转型触发点是用户反馈的原话："I already have Claude Code, Codex, Manus, OpenClaw. I don't need a smarter agent. I need someone to run them."（我不需要更聪明的 agent，我需要有人替我运营它们）[9]。CAO 从 27.3 万+ Skills / 5.1 万+ MCP servers 里组队，云端并行跑 Claude Code/Codex/OpenClaw，通过 Slack/Discord/Telegram/微信/飞书/iMessage 等 IM 网关汇报 [9][11]。

## 如何保持小

- **没有投资款可烧，就把成本当产品做**："作为一个小团队，也没有可以烧的投资款，因此我们在初期就做了非常多有关成本结构的测算……如果哪天流量突然爆炸式增长 10 倍，现有基础设施不做任何变动仍然可以接住，并且能将利润一并扩大 10 倍" [3]。
- 抠成本的具体功夫：同等流量下 preview 站点月开销约 $30（对比同行的 Vercel 天价账单）[2]；发现 Clerk 只对"二次登录"用户计费——2.4 万注册实际只按 3,000 MAU 收费，注册→活跃→付费漏斗数据白送 [3]。
- **规模观**：不追百万月活，"一千到两千名持续付费用户"就是团队的够活线 [2]。
- 团队公开可见 ≤10 人：GitHub 组织公开成员 7 人（不含 bot）[22]，2026 年 6 月新成员入职还值得在周报里单独官宣 [11]。
- 用自家 agent 加杠杆：靠 Agent Operation Tracing 让 harness 自我改进，自动发现 20+ bug，agent 任务成功率从 75% 提到 95% [23]。

## 开放问题（值得当面问创始人的）

1. Cloud 现在的 MRR 和付费用户数到什么量级了？2024 年说的"一两千付费用户够活线"过线了吗？团队现在到底几个人、怎么分工？
2. 把 80k star 的 lobe-chat 仓库直接改名转向 CAO——这个决定怎么拍板的？社区和团队内部最大的反对声音是什么？流失了多少"只要一个好看 Chat UI"的老用户？
3. MIT → Apache 2.0 → LobeHub Community License 三步收紧，每一步社区的真实反弹有多大？如果重来，会一开始就上商业限制条款吗？
4. 你说过付费用户基本不来自开源社区（"白嫖怪"理论）——那开源对这门生意的真实价值到底是什么：获客、信任资产、招聘名片，还是护城河？能量化吗？
5. 至今查不到公开融资记录——是主动不拿，还是没合适的？AI API 成本占一半的订阅生意，你怎么想它的天花板和终局？

## 来源

1. GitHub 仓库 lobehub/lobehub 及 API 数据（created_at 2023-05-21；79,893 star / 15,596 fork，检索于 2026-07-16）：https://github.com/lobehub/lobehub
2. 空谷 Arvin Xu，Cloud 公测一个月复盘 thread（2024-08-16）：https://x.com/arvin17x/status/1824474643983634683 （全文镜像：https://twitter-thread.com/t/1824474643983634683）
3. 空谷 Arvin Xu，Cloud 公测三个月复盘 thread（2024-11-03）：https://x.com/arvin17x/status/1853106500694323433 （全文镜像：https://twitter-thread.com/t/1853106500694323433）
4. 宝玉（@dotey）对复盘的总结转述（2024-11）：https://x.com/dotey/status/1853242109626622090
5. LobeHub Pricing 页面（检索于 2026-07-16）：https://lobehub.com/pricing
6. Wayback Machine 上 github.com/lobehub/lobe-chat 各快照的精确 star 数（2023-09-24 / 2023-12-10 / 2024-03-01 / 2024-12-30 / 2025-07-01）：https://web.archive.org/web/*/github.com/lobehub/lobe-chat
7. LobeHub Community License 原文：https://github.com/lobehub/lobehub/blob/main/LICENSE
8. LobeHub 博客《Announcing Our Transition to Apache License 2.0》（2024-03-28）：https://lobehub.com/blog/category/company
9. GitHub Discussion #14935《LobeHub 2.2 — Your Chief Agent Operator》（2026-05-18）：https://github.com/lobehub/lobehub/discussions/14935
10. LobeHub 博客 LOL #10（2026-05-22，CAO 上线 / PH Product of the Day / 供应链事故）：https://lobehub.com/blog/lol-10
11. LobeHub 博客 LOL #11（2026-06-05，新成员 Max / day-one 模型承诺 / IM 网关）：https://lobehub.com/blog/lol-11
12. LobeHub 博客 LOL #12（2026-06-11，X 粉丝破 5,000）：https://lobehub.com/blog/lol-12
13. 空谷 Arvin Xu 谈做 LobeChat 的起因（ChatGPT 账号被封 / Local First，2024-03）：https://x.com/arvin17x/status/1768590012583702773
14. 空谷 Arvin Xu 谈 LobeHub 名字由来（2024-08）：https://x.com/arvin17x/status/1819221250113503410
15. 空谷 Arvin Xu：知识库发布一周、40K star 达成（2024-09）：https://x.com/arvin17x/status/1832090218612359378
16. Tracxn LobeHub 公司档案（2026，无融资记录）：https://tracxn.com/d/companies/lobehub/__7JoT8WeCTLUVA_UKEBnCcX-7bDLqMnxxfonwK-MAxhE
17. Arvin Xu 个人档案（Design Engineer / Ant Design 核心成员 / 前蚂蚁集团；浙大工业设计工程硕士见 RocketReach）：https://peerlist.io/arvinxx 、https://rocketreach.co/arvin-xu-email_138449852
18. 空谷 Arvin Xu：新增 Provider 的 PR 指南"100 行童叟无欺"（2024-07）：https://x.com/arvin17x/status/1808099765923827912
19. LobeHub 博客 LOL #14（2026-06-26，创始人们登台 AWS Summit China 2026）：https://lobehub.com/blog/lol-14
20. LobeHub 博客：与 Master Concept 战略合作（2024-07-16）：https://lobehub.com/blog/category/company
21. LobeHub 博客《How an OAuth Phish Hijacked Our X Account》（2026-07-10）：https://lobehub.com/blog
22. GitHub API：lobehub 组织公开成员列表（检索于 2026-07-16）：https://api.github.com/orgs/lobehub/public_members
23. LobeHub 博客《Build a Harness That Builds Itself》（2026-05-27）：https://lobehub.com/blog
24. 空谷 Arvin Xu：LobeChat 1.0 技术栈（2024-06）：https://x.com/arvin17x/status/1803761433714507850
