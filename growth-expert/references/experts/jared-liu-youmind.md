# 宗源（Jared Liu）— YouMind 增长工程师

## 来源

- **姓名**：宗源（Jared Liu）
- **公司**：YouMind（AI 学习和创作平台，前语雀创始人玉伯创立）
- **角色**：增长工程师（Growth Engineer）
- **背景**：前端工程师转型，曾在网易/阿里做前端，后独立开发、创业，转型增长
- **成果**：近3个月贡献 YouMind 50%+ 全站流量；Product Hunt 日榜第一（Tidyread）、年榜第六
- **文章**：前端已死？重生之在 YouMind 做增长工程师
- **作者**：不孤独的二向箔（宗源本人）
- **日期**：2026-03-30
- **原文**：https://mp.weixin.qq.com/s/LBFRHtkhqOffepCaNKD60A

---

## 核心主张

1. **增长工程师 = 用技术手段做 AARRR**，聚焦拉新和激活，以数据为基础，内容是炮引子或验证器

2. **集合站是每家创业公司都值得做的增长引擎**：核心密码是"免费而丰富的高价值资源"，能引发 KOL/KOC 自发传播。注册转化率可达 20%（Wordware 受众错位只有 3–4%，对比鲜明）

3. **受众匹配 > 流量规模**：Wordware 810万UV但注册转化率 3–4%，YouMind 提示词站注册转化率 20%，区别在于来的人是不是你的目标用户

4. **Agent 自动化是增长的核心杠杆**：用 OpenClaw 在睡觉时跑增长任务，"未来在睡觉时做增长将成为常态"

5. **先做增长实验，再投入资源**：哥飞原则——40% 需求挖掘 + 20% 开发 + 40% 宣传推广

---

## 集合站策略（核心方法）

### 五个成功要素

| 要素 | 具体做法 |
|------|---------|
| **快** | 不必发布当天上线，但头一周必须发 |
| **多语言** | 做 16 个语言，大量不同语种 KOL 自发传播（土耳其 KOC 单帖曝光 80w） |
| **持续更新** | 自动化流程每天抓 X 数据筛选几十条，累积到 1.2w 提示词，成全球最大 |
| **高质量** | 数量和质量平衡，反复优化过滤规则，移除低质/截断/擦边内容 |
| **UI 有特色** | 不套组件库，选有辨识度的风格（宗源用新粗野风，大红色落地页抓眼球）|

### 集合站 + GitHub 仓库双飞轮

- 集合站给 GitHub 仓库引 Stars → Stars 超 200 被博主抓到 trending → 博主自发推广仓库
- GitHub 反向给集合站输送流量（占集合站总流量 12%+）
- **超过 200 Stars 就能带来 DR 96 的 Do-follow 外链**（GitHub 本身 DR 96–97）

### 低成本测款

用 YouMind Dynamic Webpage 快速验证需求：抓70个素材存到 Board → 生成临时落地页 → 推广观察流量 → 流量好再做正式页面，不好直接放弃。

---

## SEO 策略

### 核心指标：Domain Rating (DR)

- DR = Ahrefs 定义的域名权威度（0–100）
- DR 50+ 后，发布的博文才容易在非品牌词排名靠前
- 早期策略：先蹭**模型词**（Sora、Seedance、Nano Banana）提升 DR，再去竞争信息词

### 外链建设三层级

**第一层：买外链**
- theresanaiforthat.com（几十刀，全球最大 AI 工具导航站，一个外链）
- submitdirs.com（AITDK 作者 blank 的批量目录提交服务，分 3 个月逐步提交，能提升 10 个点 DR）

**第二层：自建资产**
- 集合站本身：YouMind 提示词集合站已带来数千个外链
- GitHub 仓库：超 200 Stars → DR 96 的 Do-follow 外链；YouMind-OpenLab 旗下 13 个仓库，总 Stars 超 11.8K

**第三层：注册转化**
- 粗暴：页面顶部 + 底部多放 CTA（天工 AI 做法）
- 精细：One-Tap Login（右上角自动弹 Google 授权），可提升 3–8% 注册转化率

### 关键词策略

- **不要在 DR 低时直接竞争大词**（如 youtube transcript）：举全站之力的竞品会吊打你单一内页
- **应该找新词、长尾词、一搜还没工具页的词**
- 加 `?gl=xx` 参数切地区，很多工具站不做多语言优化，有机会

---

## Chrome 插件增长

### 搜索词优化（影响因素）

标题 > 转化率（搜索→安装相关性）> 评分（含数量）> 描述 > 词频

### 埋词策略

**品牌词**（蹭竞品）：
- 最想蹭的词放**标题**（权重最高）
- 在不同语言的描述里分散埋词，避免 Google 惩罚
- **先申请 featured badge，通过后再做埋词**（埋词可能影响 featured 审核）
- 注意：蹭词有投诉风险，蹭过 MyMind 被投诉后搜不到了

**信息词**：
- 主打词埋标题（如 "AI Web Clipper"、"Youtube Notes"）
- 其他词分散在多语言描述里，用精准本地化表达

### Chrome Featured Badge

- 建议尽早申请（Tidyread 在 1000 用户时就拿到了）
- 通过后流量扶持效果立竿见影
- 先 featured 再埋词，顺序不能反

---

## Product Hunt 打榜

### 核心现实

> "胜负取决于社媒互换票仓网络的规模，这已经不是一个靠产品质量取胜的游戏。"

- **票源渠道（从灰到白）**：印度/东南亚票仓服务 → 互换票/群（微信群、LinkedIn PH Groups）→ 头部 Hunter
- **自动化工具**：宗源写了脚本自动抓 PH 当日日榜产品的 members 的社媒账号，挨个 connect

### 三个推荐 Hunter

| Hunter | 特点 |
|--------|------|
| Chris Messina | #1 Hunter，亲口说只要他 hunt 100% 被 Featured；有选品标准，付费咨询 chrismessina.me/hunt-me |
| Ben Lang | 曾任 Notion Head of Community，已加入 Cursor，hunt 了 360+ 产品 |
| Ryan Hoover | PH 创始人（x.com/rrhoover）|

### 关键原则

- **没被 Featured = 立刻下架**（不被 featured 就拿不到排名/badge/外链，且让帮你冲票的人下次积极性下降）
- 打榜本身带来的 PH 流量其实很少，主要价值是**外链**

---

## AI 自动化增长工作流

### Nano Banana 2 自动截流案例

不知道发布时间，但提前准备：
1. OpenClaw 每 30 分钟到 Vertex AI 轮询是否有新模型
2. 发现新模型 → 提取 Model Name 和 ID → 尝试用新 ID 生图
3. 生图成功 → 批量给 100 个提示词生图 → CMS 自动发布落地页
4. 自动在 X 和 Google 检索文档和社区讨论 → 生成 SEO 博文

### 定时任务清单（每日）

| 任务 | 时间 | 说明 |
|------|------|------|
| youmind-daily-traffic-analysis | 00:00 | PostHog 流量 + 社媒溯源 + 报告推送 |
| twitter-daily-digest | 12:00 | 时间线 200 条 + 热门趋势，生成日报，精选存 memory |
| twitter-daily-post-analysis | 13:40 | 复盘推文表现，算法分析（静默运行）|
| gsc-server-connectivity-monitor | 09:00 | 检查 GSC 连接状态，异常才报警 |
| hot-topic-scan-morning | 07:00 | 扫描 Twitter/GitHub 热点，触发 SEO blog Skill 写作 |
| hot-topic-scan-afternoon | 15:00 | 同上（下午班）|
| bookmark-seo-blog-trigger | 01:34 | 分析 Twitter 书签，筛选 SEO 价值，触发写作 |
| competitor-blog-monitor | 06:31 | 监控竞品博文更新，触发 SEO blog Skill 写作 |

### 定时任务清单（每周）

| 任务 | 时间 | 说明 |
|------|------|------|
| competitor-kol-tracker | 周一 05:00 | 追踪竞品 YouTube 红人合作 |
| youmind-weekly-sentiment | 周一 06:00 | Twitter 舆情周报，发 Slack + Board |
| youtube-kol-scout | 周一/周四 07:30 | 从 X 热点挖关键词，搜 YouTube 小 KOL |
| blog-gsc-weekly-report | 周日 06:00 | Blog 7 天 GSC 流量周报 |
| skills-gsc-weekly-report | 周日 06:30 | /skills/ 页面 28 天 GSC 数据报告 |

---

## 福格行为模型应用

**行为 = 动机 + 提示 + 能力**

案例：发现点击下载按钮的用户注册转化率极高（动机强、能力低门槛），但按钮点击量很低 → 问题出在**提示不足** → 仅加了个红点提示 → 数据出现大转折且再没下降回去

---

## 失败案例（最有价值的部分）

### 1. 提示词对比站
- **设想**：支持盲测的模型对比集合站
- **失败原因**：不是"免费而丰富的高价值资源"，而是效果对比，用户不会想收藏，KOL 不愿传播
- **教训**：想不清楚核心传播动机就不要迭功能；盲测/AI吐槽是锦上添花，不是核心 MVP

### 2. YouTube Transcript SEO 页面
- **设想**：做 youtube transcript / youtube summary 大词的工具页
- **失败原因**：词竞争难度太大，有专门以此命名的域名整站来竞争；研发投入大，匿名模式适配复杂
- **教训**：DR 低时不要挑战大词；找新词/长尾词/一搜还没工具页承载的词；无法持续大流量的页面不必单独做匿名功能，注册转化率做好就够

---

## 反直觉观点

- **Product Hunt 已经不是靠产品质量取胜**，是票仓资源竞争
- **不被 Featured 立刻下架**，一次失败的 Launch 比没有 Launch 更糟糕
- **Chrome 插件先申请 Featured，通过后再埋词**（顺序反了就可能申请不到）
- **集合站注册转化率 20% 是正常水平**（关键是受众匹配）；810万UV但3–4%转化是受众错位
- **增长工程师会故意让体验不够顺畅**（比如"必须注册才能下载"），而产品工程师会把功能优化到极致
