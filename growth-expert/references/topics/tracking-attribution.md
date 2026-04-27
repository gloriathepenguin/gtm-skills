# 追踪与归因（Tracking & Attribution）

## 为什么这是重中之重

> "如果你的转化数据只捕捉到了 40%（受广告拦截器、iOS 隐私政策、像素故障影响），算法拿到的就是失真数据，结果就失去了参考价值。"
> — Rex Gelb（Cursor）

**当下付费投放高度依赖机器学习**：Google Smart Bidding、Meta Advantage+、LinkedIn 投放系统，均基于你反馈给平台的信号优化。信号越准，优化越好。

---

## 2026 基础配置清单

### 1. Server-side Tracking（CAPI）
- **作用**：绕过浏览器限制（广告拦截器、Safari ITP、Firefox ETP）
- **适用**：Meta CAPI、Google Enhanced Conversions
- **效果**：将转化捕获率从 40–60% 提升到 80–90%+

### 2. Advanced Matching / Enhanced Conversions
- **Meta**：将加密后的用户数据（邮箱哈希）反馈给平台
- **Google**：Enhanced Conversions，同理
- **效果**：提高归因准确性，让算法找到更像真实买家的人

### 3. Consent Mode（Google）/ Cookie Consent（Meta）
- **作用**：在 GDPR/隐私合规前提下仍然获取有效信号
- **重要性**：欧洲市场必配，其他地区最佳实践

---

## 2026 的运营者新角色

AI 接管了出价、定向、版位分配之后，人工能控制的只剩：

| 能控制 | 不能控制（AI 负责）|
|--------|-------------------|
| 追踪数据质量 | 出价策略 |
| 创意素材 | 受众定向 |
| 落地页结构 | 广告版位分配 |
| 产品信息准确性 | 预算分配（PMax）|

**结论**：追踪配置的质量，直接决定算法的优化方向。

---

## 常见问题诊断

| 症状 | 可能原因 |
|------|---------|
| 平台报告转化数 >> CRM 实际转化数 | 归因窗口设置过宽；View-through 转化计入 |
| 平台报告转化数 << CRM 实际转化数 | Pixel 未正确触发；CAPI 未配置；iOS 限制 |
| CAC 突然上涨 | 追踪覆盖率下降（版本更新/隐私政策变化）|

---

## 待填充

- [ ] 具体的 CAPI 配置步骤（Meta / Google）
- [ ] 多触点归因模型的选择（Last Click vs Data-Driven）
- [ ] B2B 长销售周期的归因挑战和解决方案
