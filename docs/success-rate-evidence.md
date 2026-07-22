# SMS 接码平台成功率与来源关系证据矩阵

核验日期：**2026-07-17**（America/Los_Angeles）。本矩阵只评价公开成功率或性能数字的可复核程度，不把平台价格、库存、退款和功能声明自动当作性能证据。产品事实以 [`sms-platform-source-ledger.md`](./sms-platform-source-ledger.md) 为准。

## 证据等级与使用规则

| 等级 | 本项目定义 |
|---|---|
| A | 独立原始测试，公开数据与条件，可复现 |
| B | 独立测试，方法透明但样本有限 |
| C | 关联方测试，并明确披露商业关系 |
| D | 厂商自测、厂商比较稿或营销宣传 |
| E | 无法追溯的转载、匿名个案或无可核验出处的说法 |

正文只能按矩阵“允许措辞”列引用。**同一证据主体的多个页面不能累计成多份独立证据；本轮没有发现可评为 A 或 B 的公开成功率证据。**

## 来源关系与证据主体去重

| 证据主体 | 页面与直接关系证据 | 关系结论 | 去重与等级处理 |
|---|---|---|---|
| **S1：Serhat Doğan / VerifySMS / TwoLine 关联主体** | [VerifySMS 状态报告](https://verifysms.app/state-of-sms-verification-2026/)署名 Serhat Dogan，并写明“Founder, VerifySMS”“I run VerifySMS”；[TwoLine 测试](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/)写明作者创办 TwoLine、同时参与 VerifySMS 团队，两者是 sister brands；[DEV.to 转载](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7)写明原载 VerifySMS，作者披露“I’m the developer behind VerifySMS”。 | VerifySMS 官网比较是平台自测/厂商比较；TwoLine 对 VerifySMS 及其他平台的比较是已披露关联方测试；DEV.to 不是独立第三方。 | 整体只计 **1 个商业关联证据主体**。VerifySMS 官网和 DEV.to 数字为 D；TwoLine 披露关联关系的测试为 C；TwoLine 对自身的数字从严为 D。 |
| **S2：VirtualSMS / Daniel Mercer** | [比较文章](https://virtualsms.io/blog/best-sms-verification-services-2026)发布在 VirtualSMS 官网；[作者页](https://virtualsms.io/authors/daniel-mercer)将 Daniel Mercer 标为“Verification & Deliverability, VirtualSMS”；[关于页](https://virtualsms.io/about)称成功率排序来自平台 live order logs。 | 自有平台作者使用未公开的内部订单日志比较自己与竞品。 | 只计 **1 个厂商自述主体**，D；没有逐笔日志或可下载数据。 |
| **S3：VoidMob Team** | [比较文章](https://voidmob.com/blog/best-non-voip-sms-verification-services-2026)署名“VoidMob Team”；[关于页](https://voidmob.com/about)重复同一成功率卖点。 | 自有团队在自有域名发布自家成功率。 | 只计 **1 个厂商自述主体**，D；没有测试方法、样本或逐笔数据。 |
| **S4：SMSPVA** | [SMSPVA 官网](https://smspva.com/)在 FAQ 中声称“Real SIM numbers have a 99% delivery success rate”。 | SMSPVA 在自家平台宣传自家真实 SIM 号码。 | 只计 **1 个厂商营销主张主体**，D；未披露样本、测试条件、方法或逐笔数据。 |

## 成功率与性能数字矩阵

### S1-A：VerifySMS 官网 12 家比较（厂商自测，D）

发布页：[Best SMS Verification Services 2026: 12 Providers Honestly Compared](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/)，标注 Updated April 2026。Quick answer 同页称“8 leading providers / 200+ verification scenarios”，方法段却称 6 周、12 家、总计 240 次、每家 20 次，目标为 WhatsApp、Telegram、Discord、Google、Instagram；页面未解释 8/12 与 200+/240 的口径变化，也未公开逐笔记录、每个平台分配、号码/国家明细、时间戳或 CSV。

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| VerifySMS.app | WhatsApp **96%**；表中平均到码 10–30 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 方法段称每家总计 20；WhatsApp 只是子集且分母未披露；Quick answer另称8家/200+ scenarios | 5 个服务；国家未披露 | 6 周；更新于 2026-04 | 自家平台自测并导流自家产品 | 无逐笔数据 | 同页8 vs 12、200+ vs 240；在每家总样本≤20且结果为二元成功/失败的前提下，96%无法由公开整数分母精确复算，除非存在未披露分母、加权或取整；另与 DEV.to 78%/66%、TwoLine 10/10、二次稿29/30冲突 | D | **平台声称**其测试中 WhatsApp 为96%；同页样本口径冲突，且公开整数分母无法精确复算 |
| 5sim | WhatsApp **65–88%**；15–40 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；区间对应的国家池和分母未披露 | WhatsApp；国家池未列 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | 同作者 DEV.to 为 72% WhatsApp、61% overall；TwoLine 为 6/10 US、8/10 非 US | D | **该测试报告称** 5sim 的 WhatsApp 结果随国家池为 65–88%；不可外推 |
| HeroSMS | WhatsApp **72%**；20–60 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较；文中另披露曾是其供应侧客户 | 无逐笔数据 | 正文称 3/20 失败对应总通过 85%，与表中 WhatsApp 72%不是同一口径且未拆分 | D | **该测试报告称** HeroSMS 的 WhatsApp 为 72%；总样本与平台子样本口径未披露 |
| SMS-Man | WhatsApp **74%**；30–90 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | 同作者 DEV.to 为 65% WhatsApp、55% overall；TwoLine 为 5/10 US、7/10 非 US | D | **该测试报告称** SMS-Man 的 WhatsApp 为 74%；不可视为独立基准 |
| GrizzlySMS | WhatsApp **78%**；20–50 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | 正文另称整体测试成功率 78%，表却标为 WhatsApp 78%，两种口径被写成同一数字 | D | **该测试报告称** GrizzlySMS 为 78%，但原文的 overall/WhatsApp 口径不清 |
| Quackr | WhatsApp **60%**；30–120 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；免费/付费样本未拆分 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | TwoLine 称付费 5/10、免费近 0/10 | D | **该测试报告称** Quackr 的 WhatsApp 为 60%；免费与付费层未拆分 |
| TextVerified | WhatsApp **82%**；30–90 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | DEV.to 为 92% WhatsApp、89% overall；TwoLine 为 10/10；二次稿为 90% WhatsApp | D | **该测试报告称** TextVerified 的 WhatsApp 为 82%；其他关联页面数字冲突 |
| Receive-SMSS | WhatsApp **35%**；1–5 分钟 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；公共号 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | DEV.to 的 Receive-SMS 为 5% WhatsApp、6% overall | D | **该测试报告称**该公共号码站 WhatsApp 为 35%；不可概括所有免费站 |
| AnonymSMS | 跨 5 服务 **28%** | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20 | 5 个服务；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | 表把 28% 放在 WhatsApp Success 列，正文称 across five platforms，口径冲突 | D | **该测试报告称** AnonymSMS 为 28%，但 WhatsApp/整体口径不清 |
| SMSPool | WhatsApp **71%**；20–90 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | DEV.to 为 80% WhatsApp、68% overall；TwoLine 为 9/10 US | D | **该测试报告称** SMSPool 的 WhatsApp 为 71%；不可视为独立基准 |
| OnlineSim | WhatsApp **69%**；30–90 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | 未发现同条件可复核数据 | D | **该测试报告称** OnlineSim 的 WhatsApp 为 69%；未发现可复核数据 |
| JuicySMS | WhatsApp **73%**；25–60 秒 | [原文](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/) | VerifySMS | 每家总计 20；WhatsApp 分母未披露 | WhatsApp；国家未披露 | 同上 | 竞品由 VerifySMS 厂商比较 | 无逐笔数据 | 正文称整体测试成功率 73%，表却标为 WhatsApp 73%，口径不清 | D | **该测试报告称** JuicySMS 为 73%，但 overall/WhatsApp 口径不清 |

### S1-B：VerifySMS 状态报告（明言未做成功率测试）

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| 8 家平台（状态报告；不是成功率结果） | 2026-04 版本明确称**没有运行自有验证码测试**；一处称未来做“80 scenarios”，另一处写 8 家 × 4 国 × 每组合 10 次 = 320 attempts并发布 CSV | [原文](https://verifysms.app/state-of-sms-verification-2026/) | Serhat Dogan / VerifySMS | 当期 0；未来“80 scenarios”与320 attempts的术语/分母关系未解释 | 计划 USA/UK/Indonesia/India | 发布 2026-04-08 | VerifySMS 创始人自家方法声明 | 截至核验日页面仍只写未来发布；站内及公开搜索未找到承诺的 CSV/GitHub 数据集 | 80 scenarios不能自行等同320 attempts；同域名 2026-04 比较页又称200+ scenarios/240次实测，两页未说明项目关系 | D | **平台声称**该状态报告当期未做成功率实测；未来80 scenarios与320 attempts口径不明 |

### S1-C：DEV.to 转载（VerifySMS 开发者自测，D）

原文标题称测试 8 家；方法称每家 10 WhatsApp + 10 Telegram + 10 Instagram + 5 Google + 5 其他，共 40 次，使用 US/UK/Indonesia，时间为 2026 年 1–3 月。结果表只列 6 家（其中“Receive-SMS”又被正文说成 3 个免费服务），没有逐笔数据。DEV.to 明示原载 VerifySMS，作者也披露自己是 VerifySMS 开发者。

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| VerifySMS.app | WhatsApp **78%**、Telegram **90%**、Instagram **55%**、Google **40%**、overall **66%**；34 秒 | [原文](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7) | Serhat Doğan | 声称每家 40，其中 WhatsApp/Telegram/Instagram 各 10、Google 5 | US/UK/Indonesia；另有 5 个随机服务 | 2026-01 至 2026-03 | 作者为 VerifySMS 开发者；原载 VerifySMS | 无逐笔数据 | 10 次 WhatsApp 不可能产生 78%；10 次 Instagram 不可能产生 55%；5 次 Google 可产生 40%，但 overall 66%不是 40 次样本的 2.5% 步进；另与 96%及 10/10 冲突 | D | **平台声称**其关联作者测试得到上述数字；所述分母与百分比数学不一致 |
| 5sim | WhatsApp **72%**、Telegram **88%**、Instagram **48%**、Google **35%**、overall **61%**；41 秒 | [原文](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7) | Serhat Doğan | 声称每家 40 | 同上 | 同上 | VerifySMS 开发者比较竞品 | 无逐笔数据 | 72/88/48 均不能由各 10 次产生，35%不能由 5 次产生，61%不能由 40 次产生；与 65–88%和 TwoLine 6/10、8/10 冲突 | D | **该测试报告称** 5sim 有上述结果；分母不支持这些百分比 |
| SMS-Man | WhatsApp **65%**、Telegram **82%**、Instagram **42%**、Google **30%**、overall **55%**；52 秒 | [原文](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7) | Serhat Doğan | 声称每家 40 | 同上 | 同上 | VerifySMS 开发者比较竞品 | 无逐笔数据 | 除 55% overall 外，多数平台百分比不能由对应 10/5 次整数分母产生；与 74%和 TwoLine 5/10、7/10 冲突 | D | **该测试报告称** SMS-Man 有上述结果；平台子样本数学不一致 |
| SMSPool | WhatsApp **80%**、Telegram **85%**、Instagram **60%**、Google **45%**、overall **68%**；28 秒 | [原文](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7) | Serhat Doğan | 声称每家 40 | 同上 | 同上 | VerifySMS 开发者比较竞品 | 无逐笔数据 | Telegram 85%不能由 10 次产生，Google 45%不能由 5 次产生，overall 68%不能由 40 次产生；与 71%和 9/10 冲突 | D | **该测试报告称** SMSPool 有上述结果；分母不支持部分百分比 |
| TextVerified | WhatsApp **92%**、Telegram **95%**、Instagram **88%**、Google **80%**、overall **89%**；15 秒 | [原文](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7) | Serhat Doğan | 声称每家 40 | 同上 | 同上 | VerifySMS 开发者比较竞品 | 无逐笔数据 | 前三项不能由各 10 次产生，overall 89%不能由 40 次产生；另与 82%、TwoLine 10/10及二次稿 90%冲突 | D | **该测试报告称** TextVerified 有上述结果；分母不支持这些精度 |
| Receive-SMS / 3 个免费站 | WhatsApp **5%**、Telegram **15%**、Instagram **2%**、Google **0%**、overall **6%** | [原文](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7) | Serhat Doğan | 表看似 1 家 40 次；正文又称测试 3 个免费服务 | 同上；公共号码 | 同上 | VerifySMS 开发者比较免费竞品 | 无逐笔数据；未列 3 个站的分别结果 | 5/15/2 均不能由各 10 次产生，6%不能由 40 次产生；与 VerifySMS 比较页 Receive-SMSS 35%冲突 | D | **该测试报告称**其免费站样本有上述结果；具体站点、分母和合并方式未披露 |

### S1-D：TwoLine 关联方测试（整体 C；TwoLine 自身从严 D）

原文方法称 2026-04-02 至 2026-04-30，12 家各 10 次，共 n=120，另有 TwoLine/Hushed 基线 n=20；6 类服务、Pixel 7 和 iPhone 14。作者披露自己创办 TwoLine，并参与 VerifySMS 团队。没有逐笔记录或数据文件。

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| VerifySMS.app | **10/10** across 6 platforms | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 10 | US；WhatsApp、Telegram、Discord、Tinder、Bumble、marketplace | 2026-04-02 至 04-04 | 作者参与 VerifySMS 团队，已披露 | 无逐笔数据 | 与同作者/团队 96%、78%、66%及二次稿 29/30 冲突 | C | **关联方测试显示** VerifySMS 为 10/10；样本很小且没有逐笔数据 |
| TwoLine | US **10/10**、UK/NL **8/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 页面同时呈现两个 n=10；方法称每家 n=10，另有基线 n=20但未分配 | US/UK/NL；6 类服务 | 2026-04-05 至 04-08 | 作者称“I built TwoLine” | 无逐笔数据 | 若两组均为 10 次，则单平台合计 20，与每家 n=10 不兼容；基线 n=20是否覆盖此差额未说明 | D | **平台声称**其测试为 US 10/10、非 US 8/10；样本口径不清 |
| TextVerified | **10/10** across 6 platforms | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 10 | US；6 类服务 | 2026-04-09 至 04-12 | 作者与 VerifySMS/TwoLine 有商业关系，非 TextVerified 所属方 | 无逐笔数据 | 与 VerifySMS 厂商稿 82%、DEV.to 92%/89%及二次稿 90%冲突 | C | **关联方测试显示** TextVerified 为 10/10；不可当作精确长期成功率 |
| SMSPool | **9/10** US | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 10 | US；6 类服务 | 2026-04-13 至 04-16 | 已披露关联方测试 | 无逐笔数据 | 与 71%及 DEV.to 80%/68%冲突 | C | **关联方测试显示** SMSPool 为 9/10；样本仅 10 次 |
| Hushed | US **7/10**、Canada **6/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 页面呈现两组 n=10 | US/Canada；6 类服务 | 2026-04-17 至 04-20 | 已披露关联方测试 | 无逐笔数据 | 方法的额外基线 n=20点名 TwoLine/Hushed，但未说明 Hushed 两组是否含在 n=120或基线 | C | **关联方测试显示** Hushed 两国结果分别为 7/10、6/10；总体样本归属不清 |
| Burner | US **6/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 10 | US；6 类服务 | 2026-04-21 至 04-22 | 已披露关联方测试 | 无逐笔数据 | 未发现同条件可复核数据 | C | **关联方测试显示** Burner 为 6/10；样本仅 10 次 |
| Sideline | US **7/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 10 | US；6 类服务 | 2026-04-23 至 04-24 | 已披露关联方测试 | 无逐笔数据 | 未发现同条件可复核数据 | C | **关联方测试显示** Sideline 为 7/10；样本仅 10 次 |
| 5sim | US **6/10**、非 US **8/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 页面呈现两组 n=10；方法称每家 n=10 | US 与 RU/UA/IN/PL；6 类服务 | 2026-04-25 至 04-26 | 已披露关联方测试 | 无逐笔数据 | 两组共 20 次与每家 n=10不兼容；且与 65–88%及 DEV.to 72%/61%冲突 | C | **关联方测试显示** 5sim 为 US 6/10、非 US 8/10；样本总数冲突 |
| SMS-Man | US **5/10**、非 US **7/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 页面呈现两组 n=10；方法称每家 n=10 | US 与 RU/UA/PL；6 类服务 | 2026-04-27 | 已披露关联方测试 | 无逐笔数据 | 两组共 20 次与每家 n=10不兼容；且与 74%及 DEV.to 65%/55%冲突 | C | **关联方测试显示** SMS-Man 为 US 5/10、非 US 7/10；样本总数冲突 |
| Google Voice | US **4/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 10 | US；6 类服务 | 2026-04-28 | 已披露关联方测试 | 无逐笔数据 | 未发现同条件可复核数据 | C | **关联方测试显示** Google Voice 为 4/10；样本仅 10 次 |
| TextNow Free | **1/10** | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 10 | US/Canada；6 类服务 | 2026-04-29 | 已披露关联方测试 | 无逐笔数据 | 未发现同条件可复核数据 | C | **关联方测试显示** TextNow 免费层为 1/10；样本仅 10 次 |
| Quackr | 付费 **5/10**；免费层“接近 **0/10**” | [原文](https://twoline.io/blog/we-tested-12-sms-verification-services-2026/) | Serhat Doğan / TwoLine | 付费层 10；免费层分母未披露 | US/Canada/UK；6 类服务 | 2026-04-30 | 已披露关联方测试 | 无逐笔数据 | 免费层若另有样本，会进一步超过方法的每家 n=10；与 VerifySMS 厂商稿 60%冲突 | C | **关联方测试显示** Quackr 付费层为 5/10；免费层分母未披露 |

### S2：VirtualSMS 自述（D）

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| VirtualSMS | “consistently high”送达；关于页称 WhatsApp 约 **95%** vs VoIP route 约 **40%**，严格平台 **95%+** | [比较稿](https://virtualsms.io/blog/best-sms-verification-services-2026)；[关于页](https://virtualsms.io/about) | Daniel Mercer / VirtualSMS Team | 未披露 | 自称 145+ 国、2500+ 服务；关于页举 WhatsApp/严格平台 | 比较稿更新 2026-03-14；关于页更新 2026-04-22 | VirtualSMS 自家作者/团队 | 称来自 live order logs，但未公开分母、逐笔日志或下载数据 | 上传二次稿写“~100%”；原始页未给 100%，且关于页不同位置写约95%和95%+ | D | **平台声称**真实 SIM 订单送达率持续较高，并举出约 95%/95%+；未发现可复核数据 |
| 廉价/VoIP 服务（泛称） | 免费或廉价 VoIP 在 WhatsApp/Telegram “失败 **35–55%**”；另用 **45%** 成功率做成本示例 | [原文](https://virtualsms.io/blog/best-sms-verification-services-2026) | VirtualSMS | 未披露；45%明确是计算示例 | WhatsApp/Telegram；具体平台和国家未列 | 更新 2026-03-14 | VirtualSMS 用于对比自家 real-SIM 产品 | 无原始数据；45%是情景假设，不是观测值 | 没有列明评论平台、帖子、样本或计算过程 | D | **平台声称**廉价/VoIP 服务可能有 35–55%失败；45%仅是平台给出的成本示例 |

### S3：VoidMob 自述（D）

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| VoidMob | 支持平台成功率 **95%+**；通常 1–3 分钟 | [比较稿](https://voidmob.com/blog/best-non-voip-sms-verification-services-2026)；[关于页](https://voidmob.com/about) | VoidMob Team | 未披露 | 自称 US 号码、500+ 平台 | 发布 2026-02-24，更新 2026-06-11 | VoidMob 自家团队和自家产品页 | 无方法、样本或逐笔数据 | 没有同条件外部数据；关于页重复同一 95%+，不构成第二证据 | D | **平台声称**支持平台成功率 95%+；未发现可复核数据 |
| 非 VoIP 服务（泛称） | 严格平台 **90–99%** 成功率 | [原文](https://voidmob.com/blog/best-non-voip-sms-verification-services-2026) | VoidMob Team | 未披露 | 严格平台；未列国家/服务组合 | 更新 2026-06-11 | 厂商比较稿，用于支持自家 non-VoIP 产品 | 无方法、分母或逐笔数据 | 与自家 95%+是不同泛化口径；不可相互验证 | D | **平台声称**非 VoIP 号码在严格平台可达 90–99%；未发现可复核数据 |
| SMSPool | **99% uptime**（VoidMob 对 SMSPool claim 的二手转述） | [原文](https://voidmob.com/blog/best-non-voip-sms-verification-services-2026) | VoidMob Team | 未披露 | 平台可用性，非验证码成功率 | 更新 2026-06-11 | 竞品声明被 VoidMob 厂商比较稿二手转述 | 未链接 SMSPool 状态页时间序列 | 不是测试报告结果，且不能与验证码成功率混用 | D | **未发现可复核数据**；VoidMob 厂商比较稿转述 SMSPool 宣传99% uptime，且 uptime 不是验证码成功率 |

### S4：SMSPVA 厂商主张（D）

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| SMSPVA | 真实 SIM 号码 **99% delivery success rate** | [SMSPVA 官网](https://smspva.com/) | SMSPVA | 未披露 | 仅限定真实 SIM 号码；国家、服务、运营商与线路组合未披露 | 未披露；页面于 2026-07-17 核验 | 自家平台宣传自家产品 | 无测试方法、分母或逐笔数据 | 未发现同条件可复核数据 | D | **平台声称**真实 SIM 号码 delivery success rate 为 99%；未发现可复核方法，不用于推荐或与其他数字横比 |

### 上传二次稿中不可追溯或被改写的数字（E）

| 平台 | 公开数字/结论 | 发布页面 | 发布者 | 样本量 | 国家/服务 | 测试时间 | 与平台关系 | 原始数据 | 冲突数据 | 等级 | 允许措辞 |
|---|---|---|---|---:|---|---|---|---|---|---|---|
| VerifySMS.app | **29/30（96.7%）**，并写成“12 平台 × 3 次 × 8 服务 = 240 次独立测试” | [`upload/2026年十大接码平台深度评测.md`](../upload/2026年十大接码平台深度评测.md) | 未注明二次稿作者 | 声称 30/平台；公式实际为 288，不是 240 | 8 服务；国家未列 | 未列 | 将 S1 关联主体误写成独立来源 | 未找到任何重点原文给出 29/30或逐笔数据 | VerifySMS 原文称每家20次；29/30超过该分母；96%与29/30也不是同一精度 | E | **未发现可复核数据**；不得引用 29/30或称其为独立测试 |
| VirtualSMS | WhatsApp/Telegram **~100%** | [上传二次稿](../upload/2026年十大接码平台深度评测.md) | 未注明二次稿作者 | 未披露 | WhatsApp/Telegram | 未列 | 把 VirtualSMS 自述改写为近100% | 无 | 原始自述是“consistently high”、约95%或95%+，不是100% | E | **未发现可复核数据**；不得写~100% |
| TextVerified | WhatsApp **90%**、Google **80%**，称“独立测试” | [上传二次稿](../upload/2026年十大接码平台深度评测.md) | 未注明二次稿作者 | 未披露 | US；WhatsApp/Google | 未列 | 来自 S1 关联主体的数字拼接，不独立 | 无 | DEV.to 为92%/80%，VerifySMS比较页为82%，TwoLine为10/10；没有重点原文给出90% WhatsApp | E | **未发现可复核数据**；不得称90%/80%为独立测试 |
| 免费公共号码站（泛称） | WhatsApp **5–35%** | [上传二次稿](../upload/2026年十大接码平台深度评测.md) | 未注明二次稿作者 | 未披露 | WhatsApp；站点未列 | 未列 | 将 S1 多页不同对象合并 | 无 | 5%来自 DEV.to 的 Receive-SMS，35%来自 VerifySMS 比较页的 Receive-SMSS；不是同一测试、同一时间或同一站点 | E | **未发现可复核数据**；不得把5–35%写成统一公共号码成功率 |

## 冲突登记与正文处理

| 冲突 | 直接来源与事实 | 处理结论 | 正文允许措辞 |
|---|---|---|---|
| **VerifySMS 比较页8/12、200+/240及二次转述矛盾** | [VerifySMS 比较页](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/)Quick answer称8家/200+ scenarios，标题和方法段称12家、每家20次、总计240次；上传稿又改写为12×3×8=240，但乘积是288。 | 并列保留同页口径，不把scenario自行等同attempt；不采用二次公式。来源仍按厂商比较稿D，而非因方法矛盾改判E。 | **该测试报告称**8家/200+ scenarios及12家/240 attempts两种口径；页面未解释差异。 |
| **29/30 与每家20次不兼容** | 29/30只出现在上传稿；重点原文和公开搜索均未找到。原始比较页的每家总样本只有20。 | 29/30与96.7 percent为E，不得引用；不自行把96 percent反推成29/30。 | **未发现可复核数据**。 |
| **96 / 78 / 66 percent / 10/10 冲突** | VerifySMS自家比较为96 percent WhatsApp；但每家总样本≤20且WhatsApp为子集，在二元结果前提下无法由公开整数分母精确复算，除非有未披露分母、加权或取整；同作者DEV.to为78 percent WhatsApp、66 percent overall；TwoLine关联方为10/10 across six platforms。 | 并列呈现，不平均、不选一个当“真实成功率”；数学缺陷写入冲突栏，不改变其D/D/C来源关系等级。 | **平台声称**96 percent但公开分母无法精确复算；**该测试报告称**78/66 percent；**关联方测试显示**10/10。 |
| **状态报告80 scenarios与320 attempts** | [VerifySMS状态报告](https://verifysms.app/state-of-sms-verification-2026/)一处预告“80 scenarios”，方法计划又写8家×4国×10次=320 attempts。 | scenario与attempt可能是不同单位；页面未定义，不能自行等同或反推分母。 | **平台声称**未来测试含80 scenarios及320 attempts；两者关系未解释。 |
| **DEV.to 样本整数矛盾** | 方法称单平台10/10/10/5次，但报告78、72、65、88、55 percent等无法由对应整数分母产生；40次 overall 应以2.5 percent步进，66、61、68、89、6 percent也不满足。标题称8家，表仅6行；8×40=320，表内6×40=240。 | 全部按D并加数学警告；不能用作精确率或成本计算。 | **该测试报告称**……，但所述分母与百分比数学不一致。 |
| **TwoLine n=120 与双地区分母冲突** | 方法称12家每家n=10、总计120，另有TwoLine/Hushed baseline n=20；结果却给TwoLine、Hushed、5sim、SMS-Man各两组n=10，至少要求额外40次，且Quackr免费层分母未列。 | 整体仍是披露关系的C，但样本总数不可完全复算；TwoLine自身为D。 | **关联方测试显示**……，但样本总数与分组口径不清。 |
| **SMS-Activate 停运日期冲突** | [DEV.to](https://dev.to/serhat_doan_33c17e2855a0/sms-activate-is-gone-what-developers-need-to-know-about-migrating-32k7)写2025-12-22；[VerifySMS状态报告](https://verifysms.app/state-of-sms-verification-2026/)写2025-12-29；[VerifySMS比较页](https://verifysms.app/blog/best-sms-verification-services-2026-mega-comparison/)写2026-03；[VerifySMS首页](https://verifysms.app/)写2026-03-26；VirtualSMS页面又写2025-12。官方事实账本只确认截至2026-07-17原官网无法正常呈现原服务。 | 只能作为来源冲突，不确认具体日期或原因。 | 截至2026-07-17，SMS-Activate原官方网站无法正常呈现原有服务，可写“停运”，**不写具体日期或原因**。 |
| **5sim 自动/手动退款冲突** | [5sim官方Rules](https://5sim.net/rules)称取消订单或部分情形约5分钟未到码可退款，用户软件错误和封号不退；VerifySMS比较页称timer未使用自动退；VerifySMS状态报告和DEV.to称manual/support ticket。 | 以官方规则描述适用条件；外部“自动/手动”冲突只作来源冲突，不扩展为确认事实。 | **平台声称**取消订单或部分未到码情形可退回；关联比较稿对自动或手动流程描述冲突。 |
| **VerifySMS 国家覆盖冲突** | [官网](https://verifysms.app/)150+；[App Store](https://apps.apple.com/us/app/verify-sms-virtual-number/id6759080670)直开内容为200+；[Google Play](https://play.google.com/store/apps/details?id=app.verifysms.android)官方页面索引内容为120+，但本轮直开失败；状态报告还写200+。 | 不择一认定，只写多种官方口径并列；Google Play索引只支持官方产品版本冲突，不是独立性能证据。 | **平台声称**范围在不同官方入口分别为120+、150+或200+国家；Google Play为官方页面索引核验。 |
| **VerifySMS App 状态冲突** | 官网称iPhone/iPad和Android；App Store直开写Only for iPhone；Google Play官方页面索引显示Android上架，但本轮直开失败。DEV.to早期文又称无Android。 | 可确认iPhone商店页；Android仅按Google Play官方页面索引表述；iPad兼容不确认；旧文只作时间版本冲突，均不构成性能证据。 | **平台声称**有iOS和Android版本；App Store当前标注仅iPhone，Google Play仅经官方页面索引核验。 |
| **VerifySMS API 状态冲突** | 2026-04状态报告表格写API Yes；同月DEV.to写No developer API yet；截至官方事实账本核验日未发现公开API/MCP。 | 不写“API已上线”或“开发中预计日期”；只写未发现公开API/MCP。 | **未发现可复核数据**证明VerifySMS.app已有公开API/MCP。 |
| **VirtualSMS 成功率与退款时限版本冲突** | 比较稿写20分钟自动退款；关于页一处写2分钟，后部又写20分钟；成功率写“consistently high”、约95 percent、95 percent以上。 | 成功率仅作D级厂商声明；退款按官方事实账本的20分钟主产品口径，并保留页面内部冲突。 | **平台声称**送达率较高并可自动退款；具体成功率无可复核数据，页面退款时限存在版本冲突。 |

## 可直接用于正文的方法声明

> 本文没有购买并逐一测试这些平台。公开成功率主要来自 VerifySMS/TwoLine 关联团队及 VirtualSMS、VoidMob、SMSPVA 厂商自述；未发现公开、可复现的独立原始测试，因此没有 A 级证据；也未发现独立且方法透明的小样本测试，因此没有 B 级证据。同一作者或商业团队的多个页面按一个证据主体处理，冲突数字并列呈现，不取平均，也不把厂商自测写成本文实测。

## 核验范围与无法确认项

- 已直接打开六个重点页面、VerifySMS/TwoLine/VirtualSMS/VoidMob 作者或关于页、SMSPVA 官网、5sim Rules、VerifySMS 官网和 App Store；SMSPVA 的 99% 仅按厂商主张列 D。Google Play直开失败，120+国家与Android上架状态仅由同一官方页面的搜索索引内容核验，且不作为独立性能证据。
- 搜索了 VerifySMS 承诺的 Q2 原始 CSV/GitHub 数据集以及“29/30”“96.7%”原始出处；截至核验日未找到。
- 未找到任何重点来源公开号码级/订单级逐笔记录、失败截图集合、时间戳清单或可下载 CSV，因此没有可复现的独立原始测试（A）；同时也没有发现独立且方法透明的小样本测试（B）。
- 页面会更新；日期、App、国家数、API和退款规则应继续以官方事实账本的核验日口径为准。
