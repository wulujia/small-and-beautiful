# iA Writer（Oliver Reichenstein）

> 给写作者（而非程序员）的无干扰纯文本写作工具，用"减法 + 字体排印"在文字工具红海里切出高端买断位 ｜ ia.net ｜ Oliver Reichenstein（哲学系出身，巴塞尔/巴黎读哲学，后成为设计师）[1][19] ｜ 公司 2005 年创于东京，产品 2010 年上线 [1][19] ｜ 团队规模官方未公布，外部数据估计各办公室不足 10 人、全球合计约 10–20 人，分驻苏黎世（产品团队）与东京（设计团队）[19][26] ｜ 类型：买断制独立软件 + 设计咨询双轨 ｜ 营收未公开；2012 年自称"App Store 效率类目最赚钱应用之一，持续一年半"[6]

## 缝隙切入点

iA 是一家 2005 年创于东京的设计公司（Information Architects），给媒体集团做信息架构和 UX 咨询，客户包括 Ringier、Freitag、ZEIT ONLINE [19][25]。iA Writer 是设计公司把自己的方法论做成产品的典型：缝隙不是"又一个文本编辑器"，而是 Reichenstein 的一个判断——"The main problem with current text editors is that they were written by programmers."（现有文本编辑器的主要问题是它们都是程序员写的）[6]。市面上的编辑器为代码优化，写作者要的是另一种东西：专注、好的排版、不被格式和设置打扰。iA 的定位语是手术刀式的："A professional writing tool is like a scalpel, not like a Swiss army knife."（专业写作工具像手术刀，不像瑞士军刀）[6]。

产品哲学一句话：“The more you think about how you use your writing tool, the less energy you have to think about your writing.”（你越琢磨工具怎么用，留给写作本身的精力就越少）[4]。所以 iA Writer 没有设置项、没有主题、没有格式面板——beauty 全部押在文本排印本身 [2][4]。

## 时机

2010 年 9 月 22 日 iA Writer 在 iPad 首发 [1][2]——那是 iPad 上市的第一年，主流叙事说 iPad 是"消费设备、不适合创作"，iA 反向押注：一块只显示一个应用的屏幕恰恰是最好的无干扰写作环境。新平台没有存量竞争、没有交互惯性，Focus Mode 这种激进设计只有在全新设备上才容易被接受。2011 年 1 月 Mac App Store 开张，5 月 iA Writer for Mac 上架，吃到桌面分发渠道的早期红利 [5]。同期 Markdown 从程序员圈向写作者圈扩散，iA Writer 的 Auto-Markdown 把它变成"写作者也能用"的格式，后来 Markdown 之父 John Gruber 称 iA Writer 是他"favorite iOS app for writing in Markdown"[1]。

## 差异化

以少胜多、且每个"少"都有发明含量：

- **Focus Mode**（2010 年首发功能）：淡出当前三行以外的一切，后来演化为句子/段落聚焦 [2]。
- **Reading Time**：不显示字数而显示"读完需要几分钟"——现在全网通用的 reading time 指标，最早出现在 iA Writer 上 [2]。
- **写作专用字体**：首发用 Bold Monday 专为 iPad 定制的等宽字体 Nitti Light，连智能引号都听 Erik Spiekermann 的建议故意关掉 [2]；后来自研 iA Writer Mono/Duo/Quattro（基于 IBM Plex 改造的 duospace 字体），并以 SIL OFL 协议在 GitHub 开源 [1][24]。"typography 就是文本的 usability"[2]。
- **Syntax Highlight（词性高亮）**：用 NLP 给名词、动词、形容词、副词、连词标不同颜色，帮写作者发现形容词滥用、弱动词、被动语态——把编辑功力做进编辑器 [27]。
- **Authorship（2023 年 12 月，iA Writer 7）**：不做 AI 生成，反着来——粘贴进来的 AI 文本显示为灰色，你亲手改写一处，那处才变黑。工具不做警察，只让作者对"哪些字是我写的"保持自觉 [1][17][22]。Authorship 的标注规范以开源 Markdown Annotations 发布 [22]。该版本入围 2025 Apple Design Awards（交互类）[1]。

差异化的黑历史也值得记：2013 年 12 月 iA 发布收费新品 Writer Pro（19.99 美元），主打 Syntax Control，并宣布该功能"专利申请中"、扬言要积极维权——而这个功能大量依赖 Apple 系统自带的语言学 API。开发者社区（含 HN）强烈反弹，DHH 公开批评，几天后 iA 撤回专利申请，公开发推："Thank you @dhh for clearing our minds."[7][8][9] 小公司想用专利守护设计创新，几天内被社区舆论纠正——此后 iA 的护城河转向了相反方向：开源字体、开源规范。

## 第一批用户/冷启动

冷启动引擎是**博客积累的十年设计圈声望**。Reichenstein 2006 年 10 月发表《Web Design is 95% Typography》，引发全球设计圈论战、数百篇转载、多语种翻译，奠定了 ia.net 的行业地位 [20][21]。2010 年产品发布时，ia.net 本身就是发布渠道。

名人自来水完成引爆：Stephen Fry 2010 年被问"iPad 上离不开的四个应用"，答案里有 iA Writer——"Astonishingly simple. Everything goes away except for the writing experience."[23] Erik Spiekermann 称其为"The best app on my iPad"[2]，Fast Company 写"Writer has out-innovated Apple"[2]。Tim O'Reilly、畅销书作家 Augusten Burroughs 都是公开用户 [6]。

早期数字：2010 年 12 月，日销 300–500 份、日入 1,200–2,000 美元，iA 发文炫耀"一个 4 人设计公司的小应用，在美区 App Store 挣得和 Adobe 撑腰的 WIRED 杂志应用差不多"[3]。到 2011 年 6 月，iPad 版累计 8 万购买者；Mac 版（17.99 美元）上线两周卖出近 5,000 份 [4][5]。2012 年 7 月累计销量近 40 万份，"效率类目最赚钱应用之一，持续了一年半"[6]。iA 自己的总结不是营销驱动，而是"解决写作者的真实痛点 + 口碑"[6]。

## 收入与定价

iA Writer 的定价史是一部"对抗 App Store 重力"的编年史：

- **2010–2011，低价泥潭**：iPad 版在 App Store 低价竞争下一度只卖 0.99 美元；Reichenstein 发文反击"比披萨便宜的软件不叫贵"，提出定价公理："the right price for a product is the highest price you can ask for, but with one condition: that your customers remain happy after they buy it."[4]
- **2011，桌面溢价**：Mac 版定价 17.99 美元，刻意站上极简写作应用的中高价位 [4][5]。
- **2013**：Writer Pro 以 19.99 美元发布（后因专利风波口碑受挫）[7][8]。
- **2017，分水岭**：最直接的竞品 Ulysses 于 2017 年 8 月 10 日全面转订阅（4.99 美元/月），创始人 Max Seelemann 称这是"the hardest decision in our whole time as professional software developers"，内部争论了两年多 [10]。iA 走了相反的路。
- **2020，公开抵制 + 受控实验**：iA 发长文《Subscription or no Subscription?》，反驳"订阅是软件生存唯一出路"的行业叙事：用户感知不到持续开发成本、强转订阅制造怨恨、个人用户已有订阅疲劳；并点破 Apple 的结构性诱导（订阅抽成 15% vs 买断 30%）："我们想象了在生产力工具上开口要订阅的场景，兴奋感一周周往下掉。"[12] 但抵制不是教条——他们在新上线的 Android 版做了双轨实验：30 美元买断 或 5 美元/年订阅，用户各选一半，但买断带来的收入"substantially higher"；免费用户付费转化率 10%，超预期 [12]。结论：给用户选择权，两个价格互为锚点。
- **2023，新产品上的"妥协"**：第二款产品 iA Presenter 定价前先向社区公开问卷"你觉得该收多少钱"，结果用户报价普遍比 iA 自己预想的高；最终 Presenter 同时提供订阅与买断（买断价高于年费订阅），定价对标"一个月一个巨无霸"——"iA Presenter is one Big Mac per month, just a bit healthier."，学生免费 [13]。对订阅制的妥协发生在新产品上，而不是 iA Writer 上。
- **现状（2026）**：iA Writer 仍是纯买断：Mac 49.99 / iOS+iPadOS 49.99 / Windows 29.99 美元，官网明确写"Subscriptions to Writer are not available for iPad, iPhone, Mac, and Windows"；7 天免费试用，教育优惠 20%[14]。价格 15 年间从 0.99 涨到 49.99——用涨价而不是订阅来解决买断制的可持续性问题；iA Writer 7 作为大版本仍是免费更新 [14][18]。

## 内容与增长

ia.net 博客是 iA 二十年唯一稳定的增长引擎，套路是"用高质量长文立论 → 论点本身成为传播事件 → 产品是论点的实体化"：

- 2006《Web Design is 95% Typography》定义了 typography-first 运动，也预定义了四年后 iA Writer 的产品逻辑 [20][21]。
- 2010 年起产品发布文（Writer for iPad）本身就是设计宣言，媒体直接引用 [2]。
- 2010 年 12 月《iPad App Sales Numbers》公开自家日营收数据打脸出版业 iPad 幻想，再次成为行业讨论素材 [3]。
- 2023 年 AI 浪潮中，iA 先连发三篇 AI 与写作的立场长文，铺垫半年后才发 iA Writer 7 的 Authorship 功能，媒体（The Verge 等）"almost everyone got it right"——先输出思想再发产品，让媒体替你解释产品 [17][18]。
- 渠道迁移同样有观点驱动：2023 年公开退出 Twitter，转向 Newsletter、Mastodon、YouTube、LinkedIn；iA Presenter 的 Newsletter 六个月做到 5 万订阅 [18]。

## 社区

- **Windows 版众筹（2018）**：iA 第一次 Kickstarter，823 名支持者筹得 CHF 23,575（目标 2 万，118%）——与其说融资，不如说是用真金白银验证 Windows 需求 [11]。
- **把定价决策交给社区**：iA Presenter 定价前公开做了多轮"你会收多少钱"问卷（还带了个小向导），并把结果和推理全文公开 [13][28]。
- **开源作为社区资产**：三套自研写作字体全部开源（GitHub, SIL OFL）[24]；Authorship 的 Markdown Annotations 规范开源，Reichenstein 明确说希望"people to use this and do their own thing with that"[22]。
- Presenter 内测有 2,000+ 人报名 [18]。

## 转型

- **单品 → 三产品（2023）**：iA Writer（写）、iA Presenter（讲，2023 年 6 月正式发布）、iA Notebook（第一个实体产品：纸质笔记本，与瑞士/日本工匠合作十年、100+ 原型，写字后水印线条淡出；获 Red Dot 2025 Best of the Best 和 iF Gold 2026）[18][19]。轨迹不是"做大单品"，而是围绕"写作与表达"横向长出小产品。
- **撤出 Android（2024）**：Google 修改 Drive API 政策，先要求写作应用只配"只读"权限，后要求每年通过 CASA 安全审计（需雇 KPMG 级第三方，成本约等于 Android 版一到两个月收入、且年年交）；叠加碎片化适配和远高于其他平台的盗版率，iA 发文《Our Android App is Frozen in Carbonite》宣布下架 Play Store，老用户保留使用权 [15][16]。小团队对平台风险的处置方式：算清账、公开退出、不恋战。
- **AI 时代的再定位**：不做生成、做"作者身份追踪"（Authorship），把无干扰写作工具重新定位成"AI 时代守护人类作者性的工具"[1][17][22]。Reichenstein 对 AI 的态度是工具论："It's helpful for preparation, it's helpful for testing what you want to say."，但代笔而不自知是伦理问题——"If there's any humanity left in you, you feel really bad about it."[22]

## 如何保持小

- **二十年零融资**：官网直接把"20 Years of Independence"当卖点——不拿投资、不比稿（no pitching）、不外包（no outsourcing），设计业务只接少量客户 [19]。
- **双轨互养的结构**：苏黎世是产品团队（Information Architects AG），东京是设计团队（株式会社）[19]。咨询业务提供现金流和一线问题输入（"Maker's Knowledge"：只有亲手做才真正理解 [19]），产品把方法论变成复利资产；两边共用同一套关于排版与阅读的知识。
- **每个办公室不足 10 人**（外部估计），支持团队按日本工作时间运转 [19][26]。
- **克制作为工艺纪律**：功能不达内部标准就压着不发（隐藏的反向链接、没发布的图表功能），Reichenstein 自称这是一种"Protestant"式的克制 [22]。产品十几年不加设置项、不加主题。
- **买断制反过来约束规模**：没有经常性收入就没有养大团队的诱惑；用涨价（49.99 美元）而非扩张来维持利润 [12][14]。
- 2025 年，公司 20 年、iA Writer 15 年，仍然是同一个创始人、同一个博客、同一个买断模式 [29]。

## 开放问题（值得当面问创始人的）

1. 今天 iA 的营收里，产品和设计咨询各占多少？哪一年产品收入第一次超过咨询？有没有想过彻底砍掉咨询业务，为什么留着？
2. Android 双轨实验证明"买断收入远高于订阅"，但这个选择权模型至今没落地到 iOS/Mac——是 Apple 的规则障碍，还是你们自己不想做了？拒绝订阅这些年，粗略算过少赚多少吗？
3. iA Writer 7 作为大版本仍免费更新，49.99 美元买断要养一个 15 年的产品——大版本收费的触发条件到底是什么？现金流最紧张的是哪一年？
4. Writer Pro 专利风波从宣布到撤回只有几天：内部当时怎么吵的？为什么是 DHH 那句话起了作用？这件事之后你们把字体和 Authorship 规范都开源了，是不是同一个教训的两面？
5. AI 让"生成文字"边际成本归零，无干扰写作的缝隙十年后还在吗——Authorship 是一次防御，还是你们看到的下一条缝隙？

## 来源

- [1] Wikipedia: iA Writer — https://en.wikipedia.org/wiki/IA_Writer
- [2] iA: Writer for iPad（2010-09-22 发布文）— https://ia.net/topics/writer-for-ipad
- [3] iA: iPad App Sales Numbers – WIRED vs Writer（2010-12）— https://ia.net/topics/ipad-app-sales-numbers-wired-vs-writer
- [4] iA: On Prices and Features（2011-06-16）— https://ia.net/topics/ia-writer-on-prices-and-features
- [5] MacStories: iA Writer Launches on the Mac App Store（2011-05-27）— https://www.macstories.net/news/ia-writer-launches-on-the-mac-app-store/
- [6] iA 转载 Business Insider 访谈：“400,000 downloads with a super simple app”（2012-07-24）— https://ia.net/topics/400000-downloads-with-a-super-simple-app-business-insider
- [7] Outliner Software: The cautionary tale of iA Writer Pro — https://www.outlinersoftware.com/topics/viewt/5239/0/the-cautionary-tale-of-ia-writer-pro
- [8] candler blog: Don't Support Information Architects（2013-12-23）— https://www.candlerblog.com/2013/12/23/no-thanks-ia/
- [9] iPhoneBlog.de: iA Inc. zieht Patent-Idee von Writer Pro zurück（2013-12-27，含 “Thank you @dhh” 推文）— https://www.iphoneblog.de/2013/12/27/ia-inc-zieht-patent-idee-von-writer-pro-zurueck/
- [10] Max Seelemann (Ulysses): Why we're switching Ulysses to Subscription（2017-08-10）— https://medium.com/building-ulysses/why-were-switching-ulysses-to-subscription-47f80b07a9cd
- [11] Kickstarter: iA Writer – A focused writing app for Windows（2018-01/02，823 backers，CHF 23,575）— https://www.kickstarter.com/projects/reichenstein/a-focused-writing-app-for-windows ；数据另见 https://www.backerkit.com/projects/reichenstein/a-focused-writing-app-for-windows
- [12] iA: Subscription or no Subscription?（2020）— https://ia.net/topics/subscription-or-no-subscription
- [13] iA: Presenter Pricing (II)（2023-02-02）— https://ia.net/topics/how-much-would-you-charge-for-ia-presenter-part-2
- [14] iA Writer 官方定价页 — https://ia.net/writer/pricing
- [15] iA: Our Android App is Frozen in Carbonite（2024-09）— https://ia.net/topics/our-android-app-is-frozen-in-carbonite
- [16] Android Police: Popular writing app goes offline on Android after struggles with Google — https://www.androidpolice.com/popular-writing-app-goes-offline-on-android-after-struggles-with-google/
- [17] iA: Whoa, Feedback!（iA Writer 7 发布反馈，2023-12-08）— https://ia.net/topics/ia-writer-7-whoa-feedback
- [18] iA: The 2023 Recap — https://ia.net/topics/2023-new-year-recap
- [19] iA: About — https://ia.net/about
- [20] iA: Web Design is 95% Typography（2006-10-19）— https://ia.net/topics/the-web-is-all-about-typography-period
- [21] iA: Reactions to 95% Typography — https://ia.net/topics/webdesign-is-95-typography-partii
- [22] Andy Polaine, Power of Ten 播客: Oliver Reichenstein – Keeping it real when writing with AI — https://www.polaine.com/power-of-ten/oliver-reichenstein-keeping-it-real-when-writing-with-ai/
- [23] iA: Stephen Fry on iA Writer — https://ia.net/topics/stephen-fry-on-writer
- [24] GitHub: iaolo/iA-Fonts（开源写作字体，SIL OFL）— https://github.com/iaolo/iA-Fonts
- [25] Agency Spotter: Information Architects (iA) 客户列表 — https://www.agencyspotter.com/information-architects-ia
- [26] Apollo: Information Architects Tokyo 员工数据 — https://www.apollo.io/companies/Information-Architects-Tokyo/54a139ad69702dac84035900
- [27] iA Writer 支持文档: Syntax Highlight — https://ia.net/writer/support/editor/syntax-highlight
- [28] Oliver Reichenstein Mastodon（2022-11，定价问卷向导）— https://mastodon.social/@reichenstein/109394317466812013
- [29] Oliver Reichenstein Mastodon（2025，"Celebrating 20 years of iA and 15 years of iA Writer"）— https://mastodon.social/@reichenstein/114245794053262809
