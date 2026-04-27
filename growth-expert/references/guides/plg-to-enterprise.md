# PLG→Enterprise 转型路径

> 适合：已有一定 PLG 用户基础（$1M+ ARR），正在考虑或刚开始做企业销售的创始人/增长负责人  
> 框架来源：Holly Chen（ExponentialX）、Morgane Palomares（前 Vercel）、Lena Waters（Notion CMO）

---

## 核心前提：PLG 和 Enterprise 不是对立关系

市场上最常见的误区：
- "我们是 PLG 产品，不应该做 Sales"
- "做 Enterprise 就要放弃 PLG 的自然增长"

**正确理解（Lena Waters，Notion）**：
> PLG 是企业销售的 warm lead 生产机器，不是竞争者。个人用户 PLG 进入 → 在组织内传播 → 触发企业采购，是同一个用户旅程的不同阶段。

**底层逻辑**：没有 PLG 基础的企业销售，是陌生拜访；有 PLG 基础的企业销售，是已经在用你产品的人主动升级。两者的转化率和销售效率差距可以是 10 倍以上。

---

## 何时开始 Enterprise Motion？

**信号一：自发的团队采购**

有人在信用卡上给整个团队付费，但你没有对应的团队计划或企业合同。这是最强的信号：用户在用实际行动告诉你他们愿意付更多。

**信号二：IT / 采购部门主动联系**

有人发邮件问 SSO、SOC 2、数据处理协议。这说明产品已经在企业内部扩散到了触发安全审查的程度。

**信号三：组织内渗透深度**

同一个公司域名下有 5+ 个活跃用户，且来自不同部门（不是同一个人拉来的朋友）。

---

## 第一步：建立 PQL 系统（Product Qualified Lead）

**什么是 PQL**：不靠人工判断，用产品行为数据自动识别哪些免费用户有企业付费潜力。

### 高价值信号（按转化率排序）

| 信号 | 含义 | 优先级 |
|------|------|-------|
| 团队成员数 >5 且均活跃 | 组织渗透，不是个人爱好 | ★★★★★ |
| 用量触达免费计划上限 | 愿意付费的意愿已验证 | ★★★★★ |
| 职位发布中有你的产品名 | 招人来维护，深度依赖 | ★★★★ |
| 公司融资 / IPO 新闻 | 购买力激增 | ★★★★ |
| 邮箱域名匹配目标企业规模 | 企业账户，非个人 | ★★★ |

### 工具链（Morgane Palomares，Vercel）

```
产品使用数据（内部）
    +
Koala（行为 + 意图信号聚合）
    +
Clay（数据丰富 + 自动化触达）
    +
Common Room（社区信号：GitHub Stars、Twitter 提及）
    ↓
Sales / Product Advocate 收到优先级排序的行动清单
```

---

## 第二步：用 Product Advocates，不是 SDR

开发者工具和生产力工具面临的核心矛盾：用户极度反感销售感，但你需要企业合同。

**Morgane Palomares（Vercel）的解法**：用 Product Advocates 替代传统 SDR。

| 维度 | 传统 SDR | Product Advocate |
|------|---------|-----------------|
| 背景 | 销售出身 | 技术出身（Bootcamp、CS） |
| 工作内容 | Cold email、电话 | 技术辅助、用例扩展 |
| 触发时机 | 漏斗进入时 | PQL 信号出现时 |
| 目标 | 预约 demo | 帮用户成功 → 自然升级 |
| 用户接受度 | 被视为骚扰 | 被视为有价值的联系 |

**双目标设计**：Product Advocate 的考核同时包含：
1. Self-serve 收入（帮 Pro 用户扩展使用）
2. Enterprise pipeline（识别有企业采购潜力的账户）

这打破了 PLG 团队和 Sales 团队的内耗——两者服务同一批用户，目标对齐。

---

## 第三步：企业采购需要的基础设施

PLG 用户不需要关心的东西，Enterprise 采购必须解决：

| 需求 | 说明 | 优先级 |
|------|------|-------|
| **SSO / SAML** | IT 部门必须要求，没有就进不了 | 第一批 |
| **SOC 2 Type II** | 大公司安全审查标准 | 第一批 |
| **数据处理协议（DPA）** | GDPR 合规要求 | 第一批 |
| **管理员控制台** | IT 能看到所有席位、权限管理 | 第二批 |
| **发票 / PO 采购** | 财务部不用信用卡 | 第二批 |
| **SLA / 正常运行时间承诺** | 关键业务场景需要 | 视情况 |

**时机建议**：不要等到所有功能都做完再开始企业销售。先做 SSO + DPA，这两项解决了 80% 的企业采购阻力。剩下的在第一批企业客户的需求中迭代。

---

## 第四步：企业阶段的 GTM 动作

### Show, Don't Tell（Lena Waters，Notion）

传统企业销售：PPT → Demo → POC → 漫长决策

Notion 的做法：**直接让潜在客户进入产品**，而非展示产品。

效果：大幅缩短 Discovery 时间，买家亲身体验替代销售说服。底层逻辑：工具类产品最好的推销就是使用本身。

### 温度 vs. 专业度（Warmth vs. Competency）

PLG 产品进入企业市场时面临的核心张力：
- 原有用户爱你是因为"温度"（简单、亲切、有人情味）
- 企业买家需要"专业度"信号（安全、合规、SLA）

**做法（Lena Waters）**：不是二选一，而是**在保持温度的前提下叠加专业度**。

失败案例：很多 PLG 公司进入企业市场后变得"冷冰冰"，失去了原有用户的喜爱，最终两端都没做好。

---

## 整体路径示意

```
PLG 用户增长（自助注册）
    ↓
PQL 信号识别（Koala + Clay + 内部数据）
    ↓
Product Advocate 介入（技术辅助，非销售 push）
    ↓
团队计划升级 → 自然扩展到部门
    ↓
IT 触达 / 安全审查 → 企业合同
    ↓
Customer Success 介入（防 churn + 扩展席位）
    ↓（循环：企业用户成为新的 PLG 传播节点）
```

---

## 常见误区

**误区一：等产品"完美"再做 Enterprise**

企业客户不需要完美产品，需要能解决真实问题 + 满足合规要求的产品。先卖，迭代在路上。

**误区二：PLG 和 Enterprise Sales 团队分开运营**

两个团队服务同一批用户，数据不通会造成内耗（Sales 觉得 PLG 抢了他们的客户，Growth 觉得 Sales 在打扰用户）。Product Advocates 双目标模型解决这个问题。

**误区三：以为大公司用户 = 自动升级到企业合同**

大公司员工用个人信用卡订阅 ≠ 企业采购。后者需要主动识别信号并介入。没有 PQL 系统，这些机会会大量流失。

---

## 延伸阅读（本 skill 内）

| 想深入了解 | 看这里 |
|-----------|-------|
| PLG vs SLG 渠道分阶段框架 | [experts/holly-chen-exponentialx.md](../experts/holly-chen-exponentialx.md) |
| Product Advocates 模型详解 | [experts/morgane-palomares-vercel.md](../experts/morgane-palomares-vercel.md) |
| Agentic GTM + Show don't tell | [experts/lena-waters-notion.md](../experts/lena-waters-notion.md) |
| PMF Treadmill（AI 产品特殊性）| [experts/elena-verna-lovable.md](../experts/elena-verna-lovable.md) |
