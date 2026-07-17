# Simon Willison — Datasette

> L2 创始人资料库 · 聚焦本人公开表达（公司/产品故事见 deep/datasette.md）
> 调研日期：2026-07-17 · 调研人：Nix
> 一句话画像：Django 共同创造者、Datasette 作者，2002 年写博客至今的"公开学习"标本。2019 年离开 Eventbrite 后靠 GitHub Sponsors + 开源工具生态独立生存，LLM 时代凭一个人的博客成为全球 AI 工程师的公共基础设施——"prompt injection"、"slop"、"lethal trifecta"、"vibe engineering" 这些行业通用词都出自他手。他证明了：不融资、不建公司、不雇人，一个坚持写作的独立研究者也能站到行业话语权的中心。

## 账号全集

- 个人博客（主阵地，2002-06 写到现在）：https://simonwillison.net/ （日更级；正文 + link blog + quotations 三种体裁，link blog 从 2003-11 持续至今）
- TIL 站（Today I Learned，独立子站）：https://til.simonwillison.net/
- 关于页（自述 + 收入模式披露）：https://simonwillison.net/about/
- Newsletter（Substack，博客内容自动汇编，免费）：https://simonw.substack.com/ ；另有 GitHub Sponsors $10+/月的赞助者专属月报
- GitHub：https://github.com/simonw （数百个仓库；Datasette / sqlite-utils / LLM 等生态）
- GitHub Sponsors（主要收入来源之一）：https://github.com/sponsors/simonw
- Mastodon（自建实例）：@simon@simonwillison.net · https://fedi.simonwillison.net/@simon
- Bluesky：https://bsky.app/profile/simonwillison.net
- X/Twitter：@simonw · https://twitter.com/simonw
- LinkedIn：https://www.linkedin.com/in/simonwillison/
- Hacker News：simonw · https://news.ycombinator.com/user?id=simonw （高频、高含金量评论者）
- 产品站：https://datasette.io/ ；LLM CLI 工具：https://llm.datasette.io/ ；托管版 Datasette Cloud（Fly.io 部分赞助）
- 演讲档案（全部带逐页注释）：https://simonwillison.net/tags/annotated-talks/ ；播客出场全记录：https://simonwillison.net/tags/podcast-appearances/

## 访谈清单（精选 8 场）

1. **2023-04-07 · The Changelog Interviews #534：LLMs break the internet** · https://changelog.com/podcast/534
   - LLM 冲击波早期最完整的一次表达："I'm finding the whole thing terrifying… It's legit really scary."
   - 把 LLM 定位为 "It's a tool for thinking."（思考的工具，不是答案机）
   - 讨论 prompt injection、开源模型（LLaMA 等）与 OpenAI/Anthropic/Google 竞争格局
   - 生产力收益 vs 岗位替代焦虑的早期判断

2. **2024-01-17 · Oxide and Friends：Open Source LLMs with Simon Willison** · https://simonwillison.net/2024/Jan/17/oxide-and-friends/
   - 为什么必须有开源模型："It is far too important for a small group of companies to completely control this technology."
   - 本地小模型是学习工具：幻觉更多，反而训练你对 LLM 能力边界的直觉
   - LLM 是"weird intern"：知识渊博但不可靠，7×24 待命、没有自尊心
   - 分布式开发分散安全风险，不让任何单一实体垄断

3. **2024-09-10 · Software Misadventures：LLMs are like your weird, over-confident intern** · https://softwaremisadventures.com/p/simon-willison-llm-weird-intern （详细笔记：https://mtlynch.io/notes/simon-willison-software-misadventures/）
   - 名场面比喻："It's like having an intern who has… memorized the documentation for every programming language and is a wild conspiracy theorist."
   - 独立身份的自白："I experienced freedom for a year, and I do not want to give this up. I'm having so much fun."
   - 插件架构 = 无需 code review 的协作方式：外部贡献者独立扩展，不进主干
   - LLM 用在自己擅长的领域才安全——你有能力验证结果
   - 独立工作最大难题是优先级：靠会议 deadline 和公开承诺自我约束

4. **2024-09-25 · The Pragmatic Engineer Podcast（首期节目）：AI tools for software engineers, but without the hype** · https://newsletter.pragmaticengineer.com/p/ai-tools-for-software-engineers-simon-willison （视频：https://www.youtube.com/watch?v=uRuLgar5XZw）
   - AI 工具学习曲线被严重低估："You have to put in so much effort to learn, to explore and experiment and learn how to use it. And there's no guidance."
   - 为什么 fine-tuning 基本是浪费时间，RAG 是更务实的路径
   - 工程师抵触 AI 工具的正当理由逐条拆解
   - 三年多公开记录自己的 LLM 实验，是"用博客做研究"的示范

5. **2025-01 · Techmeme Ride Home × Latent Space 跨界特辑：Things we learned about LLMs in 2024** · https://www.latent.space/p/2024-simonw
   - GPT-4 壁垒崩塌：18 个组织的模型超越一年前的 GPT-4
   - 价格雪崩：相对 GPT-3 约 100 倍降价（Gemini 1.5 Flash $0.075/百万 token）
   - "slop" 的定义：AI 生成且 "both unrequested and unreviewed" 才算垃圾
   - 对自主 agent 泼冷水："LLMs believe anything you tell them"——轻信性让"替你花钱"的 agent 是 AGI 级难题

6. **2025-01-24 · Real Python Podcast #236：Using LLMs for Python Development** · https://simonwillison.net/2025/Jan/24/selfish-open-source/
   - "自私开源"论："my interest in open source is actually really selfish. I figured something out. I never want to have to do this work ever again."
   - 解决一次 + 开源协议 = 永远不用再解决（"you can solve a problem once and then you can slap an open source license on that solution and you will never have to solve that problem ever again"）
   - 大厂经历的反面教训：离职即失去自己写的代码，开源是对自己智力成果的保险
   - 文档和测试首先是写给自己的

7. **2025-07-11 · Generationship（Heavybit）Ep. #39：I Coined Prompt Injection** · https://www.heavybit.com/library/podcasts/generationship/ep-39-simon-willison-i-coined-prompt-injection
   - 博客复兴与"公开学习"（learning in public）的方法论
   - prompt injection 命名史与三年未解的现状
   - AI 应当增强（augment）而非替代（replace）人
   - 彩蛋：给去半人马座的世代飞船起名 "Squadron"——鹈鹕的集体名词（他住 Half Moon Bay，全球第二大加州褐鹈鹕栖息地）

8. **2026-04-02 · Lenny's Podcast：An AI state of the union** · https://www.lennysnewsletter.com/p/an-ai-state-of-the-union （本人笔记：https://simonwillison.net/2026/Apr/2/lennys-podcast/）
   - 2025-11 是拐点：GPT-5.1 / Claude Opus 4.5 之后 "almost all of the time it does what you told it to do"
   - 自估 95% 的代码产出已依赖 AI，一天可产出上万行可用代码
   - "dark factories"（无人写码、无人读码的软件工厂）概念进入主流讨论
   - 职业冲击不均匀：资深者被放大、新人上手更快、中生代最受挤压；测试成为主要瓶颈
   - 程序员是其他知识工作者的"风向标"——因为代码正确性可客观验证

## 演讲与公开课（关键场次，全部有带注释文字版）

- **2022-11 · DjangoCon US：Coping strategies for the serial project hoarder** · https://simonwillison.net/2022/Nov/26/productivity/ —— 独立开发者方法论最重要的一场：用完善文档 + 自动化测试 + issue 驱动开发，一个人同时维护上百个项目
- **2023-08 · North Bay Python：Catching up on the weird world of LLMs** · https://simonwillison.net/2023/Aug/3/weird-world-of-llms/ —— LLM 科普名场，被广泛转载
- **2023-10 · AI Engineer Summit：Open questions for AI engineering** · https://simonwillison.net/2023/Oct/17/open-questions/
- **2023-11 · GitHub Universe：Financial sustainability for open source projects** · https://simonwillison.net/2023/Nov/10/universe/ —— 10 分钟讲透独立维护者怎么活：赞助、课程、SaaS 托管、企业授权四条路；他自己押注 Datasette Cloud
- **2024-05 · PyCon US 2024 主题演讲：Imitation Intelligence**（注释版 2024-07-14） · https://simonwillison.net/2024/Jul/14/pycon/
- **2024-06 · AI Engineer World's Fair 开场 keynote：Open challenges for AI engineering** · https://simonwillison.net/2024/Jun/27/ai-worlds-fair/ —— OpenAI 临时退出，他接到通知后 24 小时内顶上开场
- **2025-05 · PyCon US 2025：Building software on top of Large Language Models**（3 小时工作坊） · https://simonwillison.net/2025/May/15/building-on-llms/
- **2025-06 · AI Engineer World's Fair keynote：The last six months in LLMs, illustrated by pelicans on bicycles** · https://simonwillison.net/2025/Jun/6/six-months-in-llms/ —— "骑自行车的鹈鹕" SVG 基准测试成为行业梗；现场演示 GitHub MCP 漏洞印证 lethal trifecta
- **2025-08 · Bay Area AI Security Meetup：My Lethal Trifecta talk** · https://simonwillison.net/2025/Aug/9/bay-area-ai/
- 早期与周边：GitHub OCTO 系列 **Personal Data Warehouses**（2020-11） · https://simonwillison.net/2020/Nov/14/personal-data-warehouses/ ；PyGotham 2021 **How to build, test and publish an open source Python library** · https://simonwillison.net/2021/Nov/4/publish-open-source-python-library/
- 方法论元演讲：**How I make annotated presentations**（2023-08-06） · https://simonwillison.net/2023/Aug/6/annotated-presentations/ —— 每场演讲都做成逐页注释网页，一次演讲三次复利（现场 + 视频 + 可检索文字）

## 博客关键文章

**博客方法论**
- What to blog about（2022-11-06） · https://simonwillison.net/2022/Nov/6/what-to-blog-about/ —— 降低写作门槛的经典：TIL 和项目记录是"低摩擦、高价值"内容，不需要原创洞见也值得写
- My approach to running a link blog（2024-12-22） · https://simonwillison.net/2024/Dec/22/link-blog/ —— link blog 完整操作手册：永远署名原作者、永远附加自己的增量价值；被 Daring Fireball、kottke 转发引发一轮博客复兴讨论
- Give people something to link to so they can talk about your features and ideas（2024-07-13） · https://simonwillison.net/2024/Jul/13/give-people-something-to-link-to/ —— 每个功能/想法都该有独立 URL，可链接性决定传播力
- Weeknotes 实践（2019 年起的周报体，标签页） · https://simonwillison.net/tags/weeknotes/ —— 独立工作者的公开问责机制：没有老板，就向读者汇报

**独立研究者的生存方式**
- Coping strategies for the serial project hoarder（2022-11-26） · https://simonwillison.net/2022/Nov/26/productivity/ —— "issue 驱动开发"：把想法写成 GitHub issue、在评论里自言自语，项目搁置半年也能无缝捡起；文档 + 测试让一个人像一支团队
- My JSK Fellowship: Building an open source ecosystem of tools for data journalism（2019-09-10） · https://simonwillison.net/2019/Sep/10/jsk-fellowship/ —— 从 Eventbrite 高管到斯坦福访学再到独立的转折点自述
- Financial sustainability for open source projects（2023-11-10，GitHub Universe 演讲文字版） · https://simonwillison.net/2023/Nov/10/universe/ —— 收入结构公开：GitHub Sponsors、GitHub Accelerator（2023）、Mozilla MIECO、Fly.io 赞助 Datasette Cloud；点破痛处："open source engineers are often great at writing code but not great at asking for money"
- Datasette: instantly create and publish an API for your SQLite databases（2017-11-13） · https://simonwillison.net/2017/Nov/13/datasette/ —— 独立事业起点的发布帖（当时还在 Eventbrite 在职）

**AI 辅助编程**
- Think of language models like ChatGPT as a "calculator for words"（2023-04-02） · https://simonwillison.net/2023/Apr/2/calculator-for-words/ —— 反"当搜索引擎用"的定位框架
- AI-enhanced development makes me more ambitious with my projects（2023-03-27） · https://simonwillison.net/2023/Mar/27/ai-enhanced-development/ —— AI 不只提效，而是把"不值得做的项目"变成"值得做"："it lowers my bar for when a project is worth investing time in at all"
- Here's how I use LLMs to help me write code（2025-03-11） · https://simonwillison.net/2025/Mar/11/using-llms-for-code/ —— 最系统的实操长文：预期管理、上下文投喂、"测试不可外包"
- Hallucinations in code are the least dangerous form of LLM mistakes（2025-03-02） · https://simonwillison.net/2025/Mar/2/hallucinations-in-code/ —— "The moment you run LLM generated code, any hallucinated methods will be instantly obvious: you'll get an error."
- Not all AI-assisted programming is vibe coding (but vibe coding rocks)（2025-03-19） · https://simonwillison.net/2025/Mar/19/vibe-coding/ —— 捍卫术语边界：vibe coding ≠ 一切 AI 辅助编程
- Vibe engineering（2025-10-07） · https://simonwillison.net/2025/Oct/7/vibe-engineering/ —— 给"高手负责任地用 agent 加速生产级工程"命名
- Things we learned about LLMs in 2024（2024-12-31） · https://simonwillison.net/2024/Dec/31/llms-in-2024/ —— 年度综述体裁的标杆（前作：Stuff we figured out about AI in 2023），被全行业当参考文献引用
- Bing: "I will not harm you unless you harm me first"（2023-02-15） · https://simonwillison.net/2023/Feb/15/bing/ —— 记录 Bing/Sydney 失控名场面的病毒式传播帖，奠定他 AI 观察者的大众影响力
- Prompt injection attacks against GPT-3（2022-09-12） · https://simonwillison.net/2022/Sep/12/prompt-injection/ —— 术语诞生地（系列索引：https://simonwillison.net/series/prompt-injection/）
- The lethal trifecta for AI agents（2025-06-16） · https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/ —— AI agent 安全的"致命三要素"框架，已成行业标准表述

**开源可持续**
- 上述 Financial sustainability（2023-11-10）与 Real Python "自私开源"访谈（2025-01-24 · https://simonwillison.net/2025/Jan/24/selfish-open-source/）构成他的开源经济学两面：对外讲"怎么收钱"，对内讲"为什么免费也划算"
- How to build, test and publish an open source Python library（2021-11-04） · https://simonwillison.net/2021/Nov/4/publish-open-source-python-library/ —— cookiecutter 模板 + CI 自动化，量产开源库的工艺流程

## 创业时间线

- **1981** 生于英国；**2000** Gameplay 网站 webmaster 起步；**2001-2005** 巴斯大学计算机科学，兼职 Incutio（写出被 WordPress/Drupal 采用的 PHP XML-RPC 库）（来源：https://en.wikipedia.org/wiki/Simon_Willison）
- **2003-2004** 在美国堪萨斯州 Lawrence Journal-World 报社实习，与 Adrian Holovaty、Jacob Kaplan-Moss、Wilson Miner 共同创造 **Django**（2005 年开源）——第一课：新闻编辑室的截稿压力孕育好框架
- **2005-2007** Yahoo 技术开发团队（Fire Eagle 地理服务早期版本）；**2002 年起**持续写博客（https://simonwillison.net/about/）
- **2008-2010** 卫报（The Guardian）软件架构师，Datablog 数据新闻经验埋下 Datasette 的种子
- **2010** 与妻子 Natalie Downe 共同创办会议社交目录 **Lanyrd**；**2011 初**入选 Y Combinator；**2013** 被 **Eventbrite 收购**，夫妇迁往旧金山，Simon 任工程总监（来源：Wikipedia / https://simonwillison.net/about/）
- **2017-11-13** 在职期间发布 **Datasette** 第一版（https://simonwillison.net/2017/Nov/13/datasette/）
- **2019** 离开 Eventbrite，入选斯坦福 **JSK 新闻学人**（2019-2020 届），全职一年做数据新闻开源工具（https://simonwillison.net/2019/Sep/10/jsk-fellowship/）——此后再未回去上班，独立至今
- **2020-2022** 独立生态期：sqlite-utils、上百个 Datasette 插件、weeknotes 公开周报、GitHub Sponsors 收入模式成型；**2022** 起任 Python 软件基金会（PSF）董事
- **2022-09-12** 命名 **prompt injection**，从工具作者跃升为 AI 安全议题定义者
- **2023** LLM 时代影响力爆发：Bing/Sydney 报道出圈（2023-02-15）、"calculator for words"（2023-04）、发布 **LLM** 命令行工具（2023-04）、入选 GitHub Accelerator、获 Mozilla MIECO 资助、AI Engineer Summit 演讲
- **2024** "slop" 定义被卫报、纽约时报引用；PyCon US 主题演讲；AI Engineer World's Fair 临危受命开场 keynote；年度综述成为行业参考文献
- **2025** "lethal trifecta"（6 月）、"vibe engineering"（10 月）相继进入行业词汇表；AI Engineer World's Fair keynote"鹈鹕骑车"基准出圈
- **2026** 提出 "agentic engineering"（2 月，来源：Wikipedia）；上 Lenny's Podcast 宣告行业拐点已过（4 月）——一个不融资、无员工的独立博主，成为 AI 工程行业的公共评估基础设施

## 语录

1. "You should start a blog. Having your own little corner of the internet is good for the soul!"（你该开个博客。在互联网上拥有自己的小角落，对灵魂有好处）——What to blog about，2022-11-06 · https://simonwillison.net/2022/Nov/6/what-to-blog-about/ （2024-12-22 link blog 一文中再次重申）
2. "A TIL—Today I Learned—is the most liberating form of content I know of."（TIL 是我所知最让人放下包袱的内容形式）——同上
3. "My goal with any link blog post is that if you read both my post and the source material you'll have an enhanced experience."（我的目标是：读了我的帖子再读原文，你的体验会被增强）——My approach to running a link blog，2024-12-22 · https://simonwillison.net/2024/Dec/22/link-blog/
4. "My interest in open source is actually really selfish. I figured something out. I never want to have to do this work ever again."（我对开源的兴趣其实非常自私：我搞明白了一件事，就再也不想重做一遍）——Real Python Podcast #236，2025-01-24 · https://simonwillison.net/2025/Jan/24/selfish-open-source/
5. "I experienced freedom for a year, and I do not want to give this up. I'm having so much fun."（我体验了一年自由，不想再放弃了，我玩得太开心了）——Software Misadventures，2024-09-10 · https://mtlynch.io/notes/simon-willison-software-misadventures/
6. "It's like having an intern who has… memorized the documentation for every programming language and is a wild conspiracy theorist."（LLM 像一个背下了所有编程语言文档、同时又是狂热阴谋论者的实习生）——同上
7. "I like to think of language models like ChatGPT as a calculator for words."（我喜欢把 ChatGPT 这类语言模型看作"文字计算器"）——2023-04-02 · https://simonwillison.net/2023/Apr/2/calculator-for-words/
8. "LLMs are still fancy autocomplete. All they do is predict a sequence of tokens." / "…an over-confident pair programming assistant who's lightning fast at looking things up."（LLM 仍是花哨的自动补全……把它当作一个过度自信、但查资料快如闪电的结对编程助手）——Here's how I use LLMs to help me write code，2025-03-11 · https://simonwillison.net/2025/Mar/11/using-llms-for-code/
9. "You have to put in so much effort to learn, to explore and experiment and learn how to use it. And there's no guidance."（你必须投入大量精力去学、去探索实验，而且没有任何指南）——The Pragmatic Engineer Podcast，2024-09-25 · https://newsletter.pragmaticengineer.com/p/ai-tools-for-software-engineers-simon-willison
10. "Vibe coding is not the same thing as writing code with the help of LLMs!"（vibe coding 不等于借助 LLM 写代码！）——2025-03-19 · https://simonwillison.net/2025/Mar/19/vibe-coding/
11. "The lethal trifecta of capabilities is: Access to your private data / Exposure to untrusted content / The ability to externally communicate."（致命三要素：访问你的私密数据、接触不可信内容、具备对外通信能力）——2025-06-16 · https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/
12. "It is far too important for a small group of companies to completely control this technology."（这项技术太重要了，绝不能由一小撮公司完全控制）——Oxide and Friends，2024-01-17 · https://simonwillison.net/2024/Jan/17/oxide-and-friends/
13. "Open source engineers are often great at writing code but not great at asking for money."（开源工程师往往擅长写代码，却不擅长开口要钱）——GitHub Universe 演讲，2023-11-10 · https://simonwillison.net/2023/Nov/10/universe/
14. "One of my favorite prompts is you just say, 'Do better,' and it works. It's the craziest thing!"（我最喜欢的提示词之一就是"做得更好点"——它居然管用，太疯狂了）——Software Misadventures，2024-09-10 · https://mtlynch.io/notes/simon-willison-software-misadventures/

## 资料缺口

- **收入数字从未公开**：GitHub Sponsors 金额、Datasette Cloud 营收、赞助/资助的具体数额均无披露，只能确认"够生活、不用上班"（对比 Mike Perham 的全裸数据，这是本案例最大空白）
- **Datasette Cloud 商业进展**不透明：客户数、定价演化、是否盈利均未见公开数据
- Lanyrd 被 Eventbrite 收购的**交易金额**未披露；他在 Eventbrite 2013-2019 六年的内部经历叙述很少
- 联合创始人/配偶 **Natalie Downe** 的视角材料稀缺（她也是 Lanyrd 联合创始人、CSS 系统化方法论先驱）
- 播客出场 50+ 场，本清单仅精选 8 场；Newsroom Robots 两集（数据新闻实战）、Talk Python Django 20 周年、Ars Live（Bing 事件复盘）等值得后续补充
- 精确离开 Eventbrite 的月份、以及"访学结束为何决定不回去"的完整决策自述，散落在多个播客中，尚无单篇权威自述文
- 中文世界几乎没有对他的系统性介绍，本档案或为首批
