# GTM Skills

Real-world growth & GTM know-how from tech company practitioners, distilled into Claude Code skills.

Not generic frameworks — these are named people, real numbers, actual tactics from first-hand sources (interviews, articles, case studies).

## Install

```bash
npx skills add gloriathepenguin/gtm-skills
```

Or via Claude Code plugin manager:
```bash
/plugin marketplace add gloriathepenguin/gtm-skills
/plugin install growth-expert
```

## Skills

### [`growth-expert`](growth-expert/)

Covers: paid ads (Google/Meta/LinkedIn), channel selection strategy, PLG→Enterprise, SEO/GEO, organic viral growth, aggregation sites, ad creative strategy, and AI product growth specifics.

**12 experts across AI-native, PLG/dev tools, paid ads, and growth consulting:**

*AI-native products*
- **宗源 Jared Liu** (YouMind) — aggregation site flywheel, trending traffic interception, AI cron automation · [LinkedIn](https://cn.linkedin.com/in/jaredl233) · [X](https://x.com/jaredliu_bravo)
- **Frank** (500万用户AI产品) — four-pillar framework (SEM→SEO→GEO→social); paid conversion first · [LinkedIn](https://www.linkedin.com/in/yaoquan-fu-76878220b/) · WeChat: AI产品Frank
- **Austin Lau** (Anthropic) — *(coming soon)* · [LinkedIn](https://www.linkedin.com/in/austinlau1/) · [X](https://x.com/helloitsaustin) · [Source](https://www.passionfroot.me/blog/anthropics-austin-lau-on-building-your-growth-engine)

*Productivity / dev tools (PLG)*
- **Ben Lang** (Notion / Cursor) — full YouTube library + authentic creator use; evergreen signup flywheel · [LinkedIn](https://www.linkedin.com/in/benmlang/) · [X](https://x.com/benln) · [Source](https://ns.com/podcast/benlang)
- **Lena Waters** (Notion CMO) — show don't tell; PLG + Enterprise as one loop; agentic GTM · [LinkedIn](https://www.linkedin.com/in/lenawaters) · [X](https://x.com/lenawaters) · [Source](https://www.notion.com/blog/welcome-lena-waters-notions-new-chief-marketing-officer)
- **Karri Saarinen** (Linear) — $35K total marketing → $1.25B; Linear Method as ideology · [LinkedIn](https://www.linkedin.com/in/karrisaarinen/) · [X](https://x.com/karrisaarinen) · [Source](https://www.lennysnewsletter.com/p/inside-linear-building-with-taste)
- **Morgane Palomares** (ex-Vercel) — Product Advocates replacing SDRs; Koala + Clay + Common Room · [LinkedIn](https://www.linkedin.com/in/morganepalomares/) · [X](https://x.com/morgane_paloma) · [Source](https://medium.com/crv-insights/power-to-the-marketer-growth-marketing-lessons-from-vercels-vice-president-of-marketing-6191dcc29106)

*Paid ads*
- **Rex Gelb** (Cursor, paid media lead) — LinkedIn/Google/Meta playbook; PMF timing; 2026 AI bidding; three levers: creative / tracking / landing page · [LinkedIn](https://www.linkedin.com/in/rex-gelb-43445b1b/) · [X](https://x.com/rexg312)
- **Jon Loomer** (jonloomer.com) — Meta algorithm is literal; targeting obsession overrated; simplify structure; creative is the #1 lever · [LinkedIn](https://www.linkedin.com/in/jonloomer) · [X](https://x.com/jonloomer) · [Site](https://www.jonloomer.com)

*Growth consulting*
- **Elena Verna** (Lovable, ex-Miro/Dropbox) — 60-70% of traditional tactics are failing; PMF Treadmill; aha moment compressed to first interaction · [LinkedIn](https://www.linkedin.com/in/elenaverna/) · [X](https://x.com/ElenaVerna) · [Source](https://www.lennysnewsletter.com/p/the-new-ai-growth-playbook-for-2026-elena-verna)
- **Holly Chen** (ExponentialX, ex-Slack/Miro/Loom) — channel selection by ARR stage; PLG/SLG convergence at $20M+; B2B influencer marketing · [LinkedIn](https://www.linkedin.com/in/holly) · [X](https://x.com/hollychen) · [Source](https://www.branch.io/resources/podcast/growth-advisor-and-former-global-head-of-digital-marketing-slack-holly-chen/)
- **Phil Carter** (Elemental Growth, ex-Quizlet) — 3-layer growth framework (Creation/Delivery/Capture); first-session imperative (80% day-zero trials); value-to-noise ratio; viral artifacts; AEO · [LinkedIn](https://www.linkedin.com/in/phil-carter-growth/) · [X](https://x.com/philcarterr) · [Source](https://www.youtube.com/watch?v=UYIgu02h8cs)

## Reference Structure

The knowledge base is organized into four layers:

```
growth-expert/references/
├── experts/     # Primary source — one file per expert, with attribution
├── channels/    # Channel playbooks — cross-expert synthesis by platform
├── topics/      # Topic deep-dives — cross-expert synthesis by question
└── guides/      # Beginner guides — foundational concepts
```

**`experts/`** — First-hand distillations. Each file covers one expert's core claims, specific tactics, and counter-intuitive takes, with source links. Start here when you want to understand *who said what and why*.

**`channels/`** — Operational playbooks per platform. Aggregates multiple experts' views into a single reference you'd actually use when running that channel.

| File | What's inside |
|------|--------------|
| [`google-ads.md`](growth-expert/references/channels/google-ads.md) | Search → AI Max → PMax → Demand Gen → GDN; full-funnel framework; cold-start sequence; PMax exploration strategy; 45% cannibalization data |
| [`meta-ads.md`](growth-expert/references/channels/meta-ads.md) | Cold-start prerequisites; algorithm signal funnel; 11 creative formulas; Advantage+ series; Jon Loomer + Rex Gelb synthesis |
| [`linkedin-ads.md`](growth-expert/references/channels/linkedin-ads.md) | Lead Gen Forms vs website conversion; B2B targeting; Rex Gelb benchmarks |

**`topics/`** — Decision frameworks by question type. Use these when you have a specific strategic question, not a platform question.

| File | Question it answers |
|------|-------------------|
| [`channel-selection-strategy.md`](growth-expert/references/topics/channel-selection-strategy.md) | Google vs Meta — which to start with, and when to switch |
| [`pmf-timing.md`](growth-expert/references/topics/pmf-timing.md) | When should you start running paid ads? |
| [`budget-allocation.md`](growth-expert/references/topics/budget-allocation.md) | How to size budgets at each stage |
| [`tracking-attribution.md`](growth-expert/references/topics/tracking-attribution.md) | CAPI, server-side tracking, consent mode setup |
| [`ad-creative-strategy.md`](growth-expert/references/topics/ad-creative-strategy.md) | Cross-platform paid ad creative: Meta / LinkedIn / Google asset strategy and testing |
| [`seo-strategy.md`](growth-expert/references/topics/seo-strategy.md) | SEO, DR building, backlinks |
| [`organic-viral-growth.md`](growth-expert/references/topics/organic-viral-growth.md) | Aggregation sites, trending traffic interception, Product Hunt, social distribution |

**`guides/`** — Foundational concepts for getting oriented.

| File | What's inside |
|------|--------------|
| [`growth-101-four-pillars.md`](growth-expert/references/guides/growth-101-four-pillars.md) | SEM/SEO/GEO/social explained; Holly Chen's ARR-stage channel framework; AI product notes |
| [`plg-to-enterprise.md`](growth-expert/references/guides/plg-to-enterprise.md) | PQL system, Product Advocates model, enterprise infrastructure checklist |

---

## Contributing

Each time a good practitioner article drops, the workflow is:
1. Fetch with [agent-reach](https://github.com/Panniantong/agent-reach) (WeChat, podcasts, etc.)
2. Distill into `references/experts/<name>-<company>.md`
3. Update the relevant `channels/` and `topics/` cross-reference files
4. Update the expert index in `SKILL.md`
