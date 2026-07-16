# Mike Perham（Sidekiq）约访

- 最佳渠道：邮件 mike@perham.net（公开在 mikeperham.com/about，他明确说"不回非客户私信"指的是技术支持，采访请求是例外——他常年接受播客/文字访谈）
- 次选渠道：Mastodon @getajobmike@ruby.social（他 2022 年后弃用 X，Ruby 社区活跃）；Bluesky @mike.contribsys.com；GitHub @mperham
- 触达难度评估：低-中。他做过大量访谈（Indie Hackers、Software Sessions、Startups For the Rest of Us、saas.group、alphalist 等），对 bootstrapper/独立开发者受众友好，且长期公开经营数据——"给中文开发者讲 Sidekiq 背后的生意"是他没覆盖过的受众，命中率高。风险点：他惜时（成功的定义就是少工作），书面回答可能比通话更容易拿到。
- 个性化钩子：① 十周年帖里的数字（$13.5M 累计销售、1,850 客户、"1 employee (me!)"）；② "credit card only, no exceptions" 这类为保持一人运营而设计的商业政策；③ 他自认的 day-one 大错（没从第一天做订阅）；④ 他 2022 年公开提出的交接问题（Ruby Central）；⑤ 他"开源基建应该像公路自来水一样公共供养"的观点——可以聊中国语境下的对照。

## 草稿

Subject: Interview request — Chinese book on small, profitable software companies

Hi Mike,

I'm Luca, a founder in Singapore — I run Zsxq (a paid-communities platform with millions of users in China) and write at wlj.me. I'm writing a Chinese-language book on small & profitable products (my first book is already with a publisher) and building a public case library alongside it.

Sidekiq is the case I keep returning to: $13.5M in cumulative sales by its 10th birthday, one employee, and business policies deliberately engineered so it stays that way — "credit card only, no exceptions" included. Chinese developers know Sidekiq the software; almost none know the business behind it.

Could I ask for a 30-minute call, or written answers to five questions? I'd focus on where you draw the free/Pro/Enterprise line, your pricing evolution since the $500 one-time days, and the succession question you raised in 2022.

Thanks for considering,
Luca (wlj.me)

## 想问的问题

1. 免费/付费的边界是怎么试出来的？有没有功能差点放进免费版最后决定收费（或相反）？"可靠性归付费"是事先原则还是事后总结？
   EN: How did you find the free/paid boundary? Was there a feature that almost went into OSS but ended up paid (or vice versa)? Was "reliability is a paid feature" a principle upfront or a pattern you noticed later?
2. 从 $500 买断到 $995/年 + Enterprise 滑动计费，每次涨价怎么定的？哪次涨价的实际结果和预期差别最大？
   EN: From the $500 one-time license to $995/yr plus Enterprise's sliding scale — how did you decide each price change, and which one surprised you most in terms of churn or pushback?
3. 14 年里最接近改变主意的一刻：最高的收购出价或最动心的雇人冲动是哪次？为什么最终没做？
   EN: In 14 years, what was the closest you came to changing your mind — the biggest acquisition offer or the strongest temptation to hire? Why didn't you?
4. Solid Queue 成为 Rails 8 默认后，免费→Pro 的转化有可测变化吗？你的应对是技术的（性能）还是商业的（定价/功能）？
   EN: Since Solid Queue became the Rails 8 default, have you seen measurable changes in the free-to-Pro funnel? Is your response technical (performance) or commercial (pricing/features)?
5. 2022 年你说不会以 owner 身份见到 2030。交接计划现在到哪一步？一门一个人的千万美元生意，该怎么设计它的身后事？
   EN: In 2022 you said you likely won't see 2030 as owner. Where does the succession plan stand now, and how do you design an "afterlife" for a one-person eight-figure business — contracts, trademarks, gem servers, and the knowledge that lives only in your head?
