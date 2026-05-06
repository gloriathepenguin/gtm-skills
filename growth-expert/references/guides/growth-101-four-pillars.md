# 出海增长 101：四柱体系入门指南

> 适合：完全没做过海外增长的创始人/PM，或只懂其中一个渠道的专项同学  
> 框架来源：Frank（500万用户AI产品海外增长负责人）四柱体系

---

## 第零章：先搞清楚三个词的关系

很多人混淆 SEM、SEO、付费广告，先对齐概念：

```
数字营销
├── 付费流量（花钱买，停止付费立即消失）
│   ├── SEM（Google/Bing 搜索广告）← 用户主动搜索时出现
│   ├── 社媒广告（FB/IG/TikTok）← 打断用户刷内容时出现
│   └── 展示广告（GDN/程序化）← 用户浏览其他网站时出现
├── 自然搜索流量（不花钱买位置，慢但长期免费）
│   └── SEO（搜索引擎优化）← 靠内容质量获得 Google/Bing 排名
└── AI 引用流量（新兴，基于内容被 AI 引用）
    └── GEO（AI 搜索优化）← 被 ChatGPT/Perplexity/AI Overview 引用
```

**SEM 是付费流量的子集**：特指在搜索结果页买关键词广告（Google Ads PPC）。很多人说"做 SEM"默认就是指 Google 搜索广告。

**SEO 和 GEO 都是自然流量，但来源不同**：SEO 面向 Google 算法，GEO 面向 AI 模型的知识库和引用逻辑。SEO 做好的内容天然会被 AI 引用，所以 GEO 是 SEO 的延伸，而不是全新独立的渠道。

---

## 第零章补充：App 产品的流量体系（与 Web 完全不同）

> 上面的框架默认面向 Web/SaaS 产品。如果你的产品是 iOS/Android App，流量逻辑完全不同，需要单独理解。

### App 的流量来源

```
App 流量
├── 付费获量（UA，User Acquisition）
│   ├── Apple Search Ads（ASA）← 只在 App Store 搜索结果页
│   ├── Google UAC（Universal App Campaign）← 打包投放，不能单选 Play Store
│   └── 社媒广告（FB/TikTok/Pangle 等）← 跳转到应用商店下载
└── 自然获量
    ├── ASO（App Store Optimization）← App 内的 SEO，靠关键词排名
    └── 口碑/品牌词搜索
```

---

### Apple Search Ads（ASA）vs Google UAC：两种完全不同的逻辑

#### Apple Search Ads（苹果搜索广告）

用户在 **App Store 搜索框**输入关键词时，顶部出现的广告位。逻辑和 Google SEM 几乎一样：

- **你指定关键词竞价**：选好词、出价、控制预算
- **高购买意图**：用户正在主动找 App，转化率高
- **数据相对透明**：能看到每个词的展示量、点击率、安装成本

#### Google UAC（通用应用广告系列）

Google Ads 里的 App 广告类型，投放位置由 Google 自动决定：

- **你不能指定关键词**：只提供素材（文字/图片/视频）+ 预算，Google 自动匹配用户
- **投放位置打包**：Play Store 搜索 + Google 搜索 + YouTube + GDN 展示网络，**无法单独只买 Play Store 搜索位**
- **黑盒程度高**：不知道哪个位置带来了哪个用户

**关键差异**：iOS 买量可以精确到"我要买搜索'fitness tracker'这个词的用户"；Android 买量只能说"我要买'下载健康 App 意向高'的用户，具体在哪里展示你定"。

**UAC 三阶段运营逻辑（量 → 质 → 钱）**：

| 阶段 | 目标 | 出价方式 | 适用时机 |
|------|------|---------|---------|
| **UAC 1.0** | 最大化安装量 | Target CPI | 冷启动，快速积累用户规模 |
| **UAC 2.0** | 优化应用内行为（注册/购买等） | Target CPA | 有一定安装数据后（50+ 转化/月）|
| **UAC 3.0** | 最大化收益，吸引高 LTV 用户 | Target ROAS | 产品成熟，有稳定付费数据 |

有足够的上阶段数据才能升级——跳过直接上 ROAS，算法没有信号可学，跑不动。

→ UAC 详细操作见 [channels/google-ads.md](../channels/google-ads.md)

---

### 为什么 AppTweak 的 Search Ads Intelligence 值钱

App Store Search Ads 是个**黑盒竞价市场**——苹果不公开谁在投哪些词、用什么素材、投了多久。

AppTweak 通过抓取数据，让你在黑盒里获得竞品情报：

| 能看到什么 | 实际用途 |
|-----------|---------|
| 竞品在投哪些关键词 | 快速找到你漏掉的高价值词，不用从零摸索 |
| 竞品的广告素材截图 | 直接看对方用什么标题/截图组合，跳过 A/B 测试摸索期 |
| 竞品的投放时间线 | 判断某个词是否有人在持续烧钱（值不值得入场竞价） |
| 同一关键词下的竞争格局 | 评估 CPT（每次点击费用）区间，判断预算够不够打 |

**对代运营的实际价值**：客户来了不知道该买哪些词、用什么素材，以前要跑 2-4 周才有数据。有 AppTweak 可以直接对标竞品已验证过的打法，冷启动速度快很多。

**什么时候 AppTweak 的溢价不值**：客户没有在跑 App Store Search Ads，也没有计划跑。这种情况下 Search Ads Intelligence 功能完全用不上，同类工具里 Appfigures（$9/月）或 ASOMobile（$47/月）性价比更高。

---

### App 买量的归因问题：为什么需要 MMP

App 产品面临一个特殊问题：广告在 Google/Meta/TikTok 投放，安装发生在 App Store/Play Store，行为数据在 App 内——三段跨平台，各广告平台只能自报数据，结果出现"数字打架"：Google 报 1000 次安装 + Meta 报 800 次安装，加起来远超实际安装量，因为同一用户被两个平台同时认领。

**MMP（Mobile Measurement Partner，移动归因平台）**的作用就是统一裁判：每次安装到底算哪个渠道的。

主流选择：**AppsFlyer**（最主流）、Adjust、Branch。

运营规则：
- 预算决策以 MMP 数据为准（SSOT），不看平台自报数字
- UAC 2.0/3.0 的应用内事件（购买、注册）必须通过 MMP 正确回传给 Google，算法才能优化

→ MMP 和归因详细说明见 [topics/tracking-attribution.md](../topics/tracking-attribution.md)

### ASO vs SEO：相似但不同

| 维度 | SEO（网站） | ASO（App Store） |
|------|------------|----------------|
| 平台 | Google/Bing | App Store / Google Play |
| 排名因素 | 外链、内容质量、页面结构 | 关键词密度、下载量、评分/评论、更新频率 |
| 工具 | Ahrefs、SEMrush | AppTweak、ASOMobile、Appfigures |
| 验证路径 | 先用 SEM 跑词，再做 SEO | 先用 ASA 验证词，再优化 ASO |
| 见效时间 | 3-6 个月 | 2-4 周（竞争没那么激烈） |

**对代运营的启示**：如果客户同时有 Web 端和 App 端，SEO 和 ASO 要分开策略，工具也要分开——没有一个工具能同时做好两件事。

---

## 第一章：为什么顺序很重要

大多数团队同时开启所有渠道，结果四个都没跑通。

正确的逻辑是：**用有限的钱，先找到"谁愿意付钱"这个答案**，然后再扩大规模。

四个渠道有明确的先后逻辑：

```
[SEM 验证] → [SEO 建资产] → [GEO 副产品] → [社媒放大品牌]
     ↑_______________________________________________|
                     数据和内容流转形成闭环
```

---

## 第二章：四根柱子详解

### 柱一：SEM — 你的付费验证实验室

**核心定位**：不是获客工具，是验证工具

#### Google Ads 能优化哪些指标？

| 优化目标 | 适合阶段 | 适合公司类型 | 注意事项 |
|---------|---------|------------|---------|
| **注册量 / Lead** | 早期，需要快速积累用户数据 | B2C 免费增值、消费类 | ⚠️ 注册不等于付费，数据可能误导后续决策 |
| **付费转化** | 有付费产品 + 有一定转化数据后 | SaaS、电商、订阅制 | ✅ AI 产品应从第一天就以此为目标 |
| **表单提交 / 演示预约** | B2B 企业级 | 高客单价、销售驱动 | 销售跟进质量决定最终结果 |
| **页面访问量** | 品牌初期曝光 | 知名度接近零时 | 不要长期停留这个目标 |

**Frank 的核心建议**：
> AI 产品的用户越多成本越高（推理费用）。如果优化注册量，每个不付费的用户都在消耗你的 API 成本。**AI 产品从第一天起就必须优化付费转化，而不是注册量。**

传统 SaaS 可以"先拉量再转化"，AI 产品不行。

#### SEM 和 GDN（展示广告）有什么区别？

很多人把 Google Ads 和 GDN 混为一谈，其实是两种完全不同的广告：

| 维度 | SEM（搜索广告） | GDN（展示广告） |
|------|--------------|--------------|
| 出现时机 | 用户主动搜索关键词时 | 用户浏览其他网站 / App 时 |
| 用户意图 | 高——正在找解决方案 | 低——未必有需求 |
| 转化率 | 高 | 低 |
| 适合阶段 | 从第一天开始 | 有一定流量后做再营销 |

**对早期团队的建议**：把预算集中在搜索广告。GDN 覆盖广但意图弱，早期没有足够的再营销数据，大概率是低效曝光。等转化漏斗跑通之后，再用 GDN 追踪未转化的用户（再营销）。

→ GDN 详细用法见 [channels/google-ads.md](../channels/google-ads.md)

---

#### SEM 第一个月该怎么跑？

1. **从品牌词开始**（自己公司名 + 产品名）：转化率最高，成本最低，先跑通数据
2. **加竞品词**（用户在搜你竞品时截流）：成本较高但意图明确
3. **最后才做非品牌词**（行业通用词）：竞争激烈，需要有足够数据支撑

```
第1-2周：品牌词 → 验证基础转化漏斗是否跑通
第3-4周：加入竞品词 → 测试不同意图用户的转化差异
第2个月起：小预算测试非品牌词 → 找"金矿词"
```

#### 什么是"金矿词"？

搜索这个词的用户，**注册后真的付了钱**。

如何找：在 Google Ads 后台，把转化目标设为"付费"，跑 2-4 周，找出付费转化率最高的关键词。这些词就是你后续所有决策的数据基础。

---

### 柱二：SEO — 用 SEM 数据选词，不是用感觉

**核心定位**：建长期流量资产，但选词必须基于 SEM 验证结果

#### SEO 为什么慢？

Google 要评估你的内容是否值得信任，需要时间：
- 新网站：3-6 个月才开始有排名
- 竞争激烈的词：可能需要 1-2 年
- 没有外链（Backlink）支撑：基本排不上去

#### SEO 关键词三种类型

| 类型 | 示例 | 搜索意图 | 转化率 | 难度 |
|------|------|---------|-------|------|
| **品牌词** | "Notion AI" | 已知道你 | 极高 | 低（自己品牌） |
| **产品类词** | "AI note taking app" | 在比较方案 | 高 | 中-高 |
| **信息词** | "how to organize notes with AI" | 在学习 | 低-中 | 低-中 |

**正确策略（来自 Frank + Jared Liu）**：
1. 用 SEM 跑出高付费转化的产品类词 → 这些词值得花 3-6 个月做 SEO
2. 信息词辅助建立权威（Domain Rating），但主战场是产品词

#### 什么是 DR（Domain Rating）？

DR 是 Ahrefs 等工具对域名整体权威性的评分（0-100）。

| DR 分段 | 意味着 | 大概需要 |
|--------|-------|---------|
| 0-20 | 新站，几乎没有外链 | 6个月内正常 |
| 20-40 | 有一定积累，部分词能排进第一页 | 1-2年 |
| 40-60 | 有竞争力 | 2-3年持续建设 |
| 60+ | 行业权威级别 | 长期投入 |

快速提高 DR 的方法（来自 Jared Liu）：
- GitHub 开源项目 200+ Stars → 能获得 DR96 的 dofollow 外链
- Product Hunt 上线 → 高 DR 媒体自然报道
- 集合站/对比站收录 → 低成本批量外链

---

### 柱三：GEO — SEO 的免费副产品

**核心定位**：让你的内容出现在 ChatGPT / Perplexity / Google AI Overview 的回答里

#### 为什么现在要关注 GEO？

用户的信息获取方式正在转变：
- 过去：Google 搜索 → 点击结果 → 浏览网站
- 现在：直接问 ChatGPT / Perplexity → 得到答案（可能附带引用）

如果 AI 在回答"最好的 AI 笔记工具是什么"时不提你，你就在这个渠道上隐身了。

#### GEO 和 SEO 的关系

| SEO 做了 | GEO 的效果 |
|---------|-----------|
| 有结构化内容（对比文章、使用指南） | AI 会直接引用 |
| 有真实用户案例 | AI 回答时会举例 |
| 没有内容 | AI 根本不知道你存在 |

**结论**：先把 SEO 做好，GEO 自然跟上。不需要单独投入。

#### Lena Waters（Notion CMO）的补充视角

> "Think about how much time we've spent debating the top nav. That's applied human psychology. Agents don't care."

传统网站是为人类设计的（导航、视觉层次、情感化设计）。AI Agent 只解析内容结构。  
实践建议：确保你的核心产品信息以干净的文字形式存在，而不只是埋在精美的网页设计里。

---

### 柱四：社媒 — KPI 是品牌词搜索量，不是粉丝数

**核心定位**：通过社媒内容驱动用户主动 Google 你的品牌

#### 为什么粉丝数是错误的 KPI？

- 粉丝数 ≠ 付费用户数，两者相关性极低
- 10 万粉丝但没人去搜你品牌词 = 你只是个内容账号
- 1 万粉丝但每次发帖后品牌词搜索量涨 20% = 你在真正建立品牌

#### 正确 KPI：品牌词搜索量（Brand Search Volume）

如何追踪：Google Search Console → 过滤你的品牌词 → 看每次发帖前后的点击量变化

品牌词搜索用户的特点：
- 主动找你 = 已经有一定信任
- 付费转化率通常比广告词用户高 2-5 倍
- 这些用户来了之后，SEM 的广告质量得分也会提升（降低 CPC）

#### 不同社媒平台的作用

| 平台 | 适合 | 内容形式 |
|------|------|---------|
| Twitter/X | 技术产品、开发者工具 | 产品更新、使用技巧、思考输出 |
| LinkedIn | B2B、企业级 | 案例故事、数据洞察、行业观点 |
| YouTube | 任何需要演示的产品 | 教程、对比测评（参考 Ben Lang 的 Notion 策略） |
| TikTok/Instagram | C端消费品、创意工具 | 快速展示结果、钩子型短视频 |

**Ben Lang（Notion 早期增长）的关键发现**：
- YouTube 全视频教程 >> 60 秒贴片广告（CPA 低 2-5 倍）
- 创作者**真实使用**你的产品远比"念台词"效果好
- YouTube 视频是**常青资产**：发布 6 个月后仍在带来新注册

---

## 第三章：闭环是如何运转的

一个完整的例子：

```
① SEM 跑了 1 个月，发现 "AI meeting notes" 这个词付费转化率是平均的 3 倍
   ↓
② SEO 围绕 "AI meeting notes" 写深度内容（对比文、使用指南、案例）
   ↓  
③ GEO：Perplexity 在回答 "best AI meeting tool" 时开始引用你的对比文章
   ↓
④ 社媒发布 "我用 AI 做会议记录 30 天的真实体验" → 品牌词搜索量上涨
   ↓
⑤ 品牌词搜索量提升 → SEO 排名提升 + SEM 广告质量得分提升（CPC 下降）
   ↓（回到起点，下一轮验证新词）
```

每个环节都在喂数据给下一个环节，而不是各自为政。

---

## 第四章：不同阶段该做什么（ARR 驱动的渠道选择）

> 框架来源：Holly Chen（ExponentialX，前 Slack / Miro / Loom）
>
> 核心原则：**渠道选择由 ARR 阶段决定，而非产品类型**。"我是 PLG 产品所以不做 Sales"是错误的——不同阶段有效的组合完全不同。

### $0 → $1M ARR — 找到可重复路径

| 分类 | 有效渠道 | 不该碰 |
|------|---------|-------|
| 优先做 | Product-led 自助注册、创始人直销、社区/口碑 | 大规模付费投放（PMF 未稳，烧钱） |
| 不该碰 | — | Content Marketing（6-12 个月才出效果）、Partnership（谈判消耗大，规模小无筹码） |

**判断信号**：创始人不亲自参与每个 deal，能否完成销售？不能 → 还没到扩渠道的时候。

**PMF 粗略标准（Rex Gelb，Cursor）**：Week-4 留存率 > 20%

---

### $1M → $5M ARR — 建立初始增长引擎

| 路径 | 有效渠道 |
|------|---------|
| **PLG 路径** | SEO + 内容（用 SEM 验证词后开始建资产）、产品内 viral loop（邀请/协作触发分享）、KOL/Influencer（参考 Ben Lang 的 Notion 模型） |
| **Sales-led 路径** | 有 intent 信号支撑的 Outbound（非随机 cold email）、小规模 Field Marketing 活动（找高意向人群） |
| **两者共同** | Referral 项目（此阶段用户基数够，激励分享 ROI 合理） |

---

### $5M → $20M ARR — 专注转化，不要全铺

> "At this stage, the question isn't PLG or SLG. It's what's your conversion motion from free to paid, and from paid to enterprise."
> — Holly Chen

重点转向：
- **PQL 系统**（Product Qualified Lead）：用产品行为数据识别哪些免费用户有付费信号，触发 Sales 介入
- **B2B Influencer Marketing**：LinkedIn / Twitter 精准受众，ROI 优于广泛投放
- SEM 扩量（此时已有足够转化数据支撑 AI 出价优化）

⚠️ **这个阶段的常见陷阱**：以为可以持续靠自然增长，实际 CAC 开始爬升；SEO 内容规模化后质量下降，排名不稳定。

---

### $20M ARR+ — PLG 和 SLG 必然收敛

> "Every successful PLG company above $20M ARR starts looking like a SLG company. The question is whether you plan for that or stumble into it."
> — Holly Chen

几乎所有高增长 SaaS 在这个阶段都会：
- 成立专门的 Enterprise Sales 团队
- 建立 Customer Success 职能（防 churn + 扩展）
- 开始做大客户 Executive Relationship

**PLG 的优势在此阶段体现为**：企业内已有自下而上的用户基础（warm leads），谈判时有"先用后买"的产品验证。

→ 完整的 PLG→Enterprise 转型路径，见 [guides/plg-to-enterprise.md](plg-to-enterprise.md)

---

## 第五章：AI 产品特别说明

> 来源：Elena Verna（Lovable CPO，前 Miro / Dropbox）+ Frank（500 万用户 AI 产品）+ Phil Carter（Elemental Growth，前 Quizlet）

### 增长三层拆分（Phil Carter）

在讲具体战术之前，先用这个框架对齐增长的三个环节：

```
Value Creation（价值创造）— 产品是否真正造出了用户想要的价值？
    ↓
Value Delivery（价值传递）— 分发、营销、触达，本身就是增长模型的一部分
    ↓
Value Capture（价值变现）— Paywall、定价、套餐包装
```

核心原则：如果 Value Creation 的承诺不清晰，后面所有优化都只是在放大噪音。

---

### 1. PMF Treadmill — PMF 不是终点，是跑步机（Elena Verna）

传统观念：找到 PMF → 踩油门增长 → 持续扩大规模

AI 产品现实：
> "PMF is not a destination. It's a treadmill. The moment you think you've found it, the ground shifts again."
> — Elena Verna

AI 能力每 3-6 个月发生一次量级跳跃，用户预期随之重置：
- 今天让用户惊叫"wow"的功能，6 个月后成为基础预期
- 再 6 个月后变成负担（"为什么还要我做这一步？"）
- 同样的留存率，6 个月前是及格，现在可能不合格

**实践含义**：不能一次 PMF 验证完就全速推进。每季度重新校验核心用户行为信号，留存基准线在持续上移。

### 2. First Session 是最关键的转化战场（Elena Verna + Phil Carter）

传统 PLG Onboarding 逻辑：设计 7 步引导漏斗 → 带用户到 aha moment

AI 产品现实：
> "The value delivery in AI products is so immediate that the traditional 'aha moment' has collapsed into the first interaction."
> — Elena Verna

**RevenueCat 行业数据（Phil Carter）**：消费订阅产品中，试用发生在 day zero 的比例已超过 **80%**，部分品类接近 90%。必须在前 **30-60 秒**让用户感受到价值，否则基本不会再转化。

竞品 AI 能直接完成用户想做的事，任何"引导期"都是流失点。

**实践含义**：第一个 prompt / 操作就必须 deliver value。传统的注册后邮件序列、分步引导、功能解锁设计在 AI 产品里 ROI 极低。

### 3. Value-to-Noise Ratio：功能多 ≠ 价值大（Phil Carter）

AI 让功能做得很快，团队容易陷入"发得越多价值越大"的误区。

**正确指标**：用户能多快撞见真正有用的那部分价值——而不是功能总数。

**优秀团队的做法**：
- 持续 shipping 的同时，盯 feature usage、长期留存、订阅留存之间的关联
- 找出 **hero features**（真正驱动留存的功能），砍掉不再产生价值的噪音

> "与其只看功能堆了多少，不如看你的价值噪音比。" — Phil Carter

### 4. AI 成本结构决定增长目标（Frank + Phil Carter）

> "如果你的增长策略只管把用户灌进来，不管灌进来的人愿不愿意付费，你不是在增长——你是在加速亏损。" — Frank

每个注册但不付费的用户 = 持续消耗 token + 零收入。Google Ads 从第一天起必须优化**付费转化**，而非注册量。

**Phil Carter 的延伸**：AI 有真实算力成本，30 天免费试用可能适得其反——吸引一批高消耗用户用完即走。趋势是**缩短试用 + 多层订阅 + 用量上限 + 额外 credits**，越来越像 B2B 分层收费。

### 5. 模型选择是增长决策，不只是工程决策（Phil Carter）

> "产品体验不只取决于模型输出的质量，也取决于它输出得有多快、代价有多高。"

**Gamma 案例**：6 个月内实现盈利，原因之一是没有把"最强模型"当成唯一答案——质量够用 + 速度快 + 成本低的模型，用户体验反而更好。

- 高溢价、性能第一的产品 → 上最强模型
- 大众化产品 → 先找到"质量够用、速度更快、单位经济更健康"的组合

---

## 第六章：最常见的四个错误

1. **优化注册量，不优化付费转化**  
   → 跑出来的"最优关键词"背后全是薅羊毛用户，后续 SEO 方向全错

2. **SEO 选词靠感觉或抄竞品**  
   → 没有验证过这些词背后的用户是否付钱，投入 6 个月白做

3. **社媒只看粉丝和互动数**  
   → 做了一年，付费用户增长和社媒增长之间零相关

4. **四个渠道各找一家外包，数据互不相通**  
   → 广告代投不知道 SEO 在做什么词，SEO 不看广告转化数据

---

## 核心指标速查

| 指标 | 全称 | 含义 | 计算公式 | 典型场景 |
|------|------|------|---------|---------|
| **CPI** | Cost Per Install | 每次 App 安装成本 | 广告花费 ÷ 安装次数 | UAC 1.0，App 冷启动 |
| **CPA** | Cost Per Acquisition | 每次转化成本 | 广告花费 ÷ 转化次数 | UAC 2.0，优化应用内行为 |
| **ROAS** | Return on Ad Spend | 广告花费回报率 | 广告带来的收入 ÷ 广告花费 | UAC 3.0，优化收益 |
| **CAC** | Customer Acquisition Cost | 获客成本 | 总获客花费 ÷ 新客数量 | 比 CPA 范围更广，含所有获客渠道 |
| **LTV** | Lifetime Value | 用户生命周期价值 | 用户在整个生命周期内带来的总收入 | 判断 CAC 是否合理的参照 |
| **CTR** | Click-Through Rate | 点击率 | 点击次数 ÷ 展示次数 | 衡量广告素材吸引力 |
| **CPM** | Cost Per Mille | 千次展示成本 | 广告花费 ÷ 曝光量 × 1000 | 反映流量价格；高低不直接代表流量质量 |
| **oCPM** | Optimized Cost Per Mille | 优化千次展示出价 | 广告主填写期望转化成本 | Meta / 字节系主流出价方式，系统以转化为优化目标 |
| **eCPM** | Effective Cost Per Mille | 有效千次展示收益 | 出价 × 预估CTR × 预估CVR × 1000 | 平台内部排序依据；eCPM 高 → 拿到更多流量分配 |

> **三者关系**：广告主按 **oCPM** 出价 → 系统按 **eCPM** 排序 → 最终成本表现为 **CPM**。这也解释了为什么素材质量比出价本身更重要：同样出价，素材 CTR/CVR 更高的账户 eCPM 更高，自然拿到更多流量。详见 [meta-ads.md](../channels/meta-ads.md)。

**核心判断标准**：LTV > CAC × 3，业务才可持续。ROAS 4x 意味着花 1 块钱赚回 4 块钱。

---

## 快速自检表

在开始任何渠道前，先问自己：

- [ ] 我的 Google Ads 转化目标是付费，还是注册？
- [ ] 我知道哪 2-3 个关键词的付费转化率最高吗？
- [ ] 我的 SEO 内容选题有没有基于广告验证结果？
- [ ] 我知道我的产品在 ChatGPT 里被提到的频率吗？
- [ ] 我在追踪品牌词搜索量，还是只看社媒粉丝？
- [ ] 我的广告团队、SEO、社媒上周有没有开一次数据对齐会？

---

## 延伸阅读（本 skill 内）

| 想深入了解 | 看这里 |
|-----------|-------|
| SEM 分阶段预算策略 | [budget-allocation.md](../topics/budget-allocation.md) |
| Google/LinkedIn/Meta 平台细节 | [google-ads.md](../channels/google-ads.md)、[linkedin-ads.md](../channels/linkedin-ads.md) |
| SEO 外链和 DR 策略 | [seo-strategy.md](../topics/seo-strategy.md) |
| 创作者/KOL 增长实战 | [ben-lang-notion-cursor.md](../experts/ben-lang-notion-cursor.md) |
| AI 时代 GTM 全局观 | [lena-waters-notion.md](../experts/lena-waters-notion.md) |
