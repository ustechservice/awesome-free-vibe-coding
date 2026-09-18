# awesome-free-vibe-coding [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> **Verified free tiers for vibe coding** — real limits, TOS gotchas, student-offer tracking, and the open source that replaces your SaaS stack. Receipts required.

**Tool count: see [`tools.json`](tools.json)** — the headline number here always equals `jq length tools.json`. No "550+" marketing math.

Maintained by [DarkDataLabs](https://darkdatalabs.com) / US_Tech. Extracted from a live operation, not scraped from a blog.

![Tools](https://img.shields.io/badge/tools-42-00acb8?style=flat-square)
![Primary verified](https://img.shields.io/badge/%F0%9F%A7%BE_primary--verified-4-00acb8?style=flat-square)
![Corroborated](https://img.shields.io/badge/%E2%9C%85_corroborated-33-2ea44f?style=flat-square)
![Extinct tracked](https://img.shields.io/badge/extinct_tracked-15-555?style=flat-square)
![SaaS displaced](https://img.shields.io/badge/SaaS_displaced-%24321%E2%80%93%241%2C088%2Fmo-orange?style=flat-square)

**Verification status:** last pass Aug 2026 (batch 1: Bolt, v0, Lovable, Codespaces) - monthly cadence - remaining queue tracked in [issue #1](https://github.com/ustechservice/awesome-free-vibe-coding/issues/1). Every limit links to a pricing-page receipt or carries an honest ⏳.

**What qualifies (the whole bar, three lines):**
- Permanently free tier - trials and "free with paid plan" features do not count
- Receipts required - pricing pages and official docs only; announcement posts are not sources
- Deaths are documented, not deleted - extinct tiers move to the [extinct list](GRAVEYARD.md) with dates

**New to vibe coding?** Skip the taxonomy - go straight to the [⚡ $0 Quickstart](#-quickstart-the-0-stack) and ship something tonight.

### At a glance

| Tool | Best for | Free tier in one line |
|---|---|---|
| [Cline](https://cline.bot) | Open-source coding agent | Free forever, BYOK, runs in VS Code |
| [Google AI Studio](https://aistudio.google.com) | Free frontier-model API | Gemini key in 90 seconds, no card |
| [Bolt](https://bolt.new) | Build in the browser | 300K tokens/day, 1M/mo 🧾 |
| [Cloudflare](https://pages.cloudflare.com) | Deploy for $0 | Pages unlimited static, Workers 100K req/day |
| [Oracle OCI](https://oracle.com/cloud/free) | Always-free VMs | ARM A1 instances, no expiry 🧾 |
| [Twenty](https://twenty.com) | Replace your CRM bill | Self-hosted, open source, $0 forever |

---

## Why this exists

Free-tier lists rot. In 2026 alone: a major listicle crowned Amazon Q Developer "best free tier" in April — Amazon closed it to new signups on **May 15**. Phind shut down in January a month after raising $10M. Google cut Gemini API free limits 50–80% in December 2025. Cursor's famous free student year closed in June. Every unmaintained list still recommends at least one dead product.

This repo fights rot with three rules:

1. **Receipts required.** Every limit links to a pricing/docs page. Announcement blog posts don't count as sources (they're where stale data comes from).
2. **Honest accounting.** We report *documented recurring* limits, not theoretical rate-limit ceilings or one-time signup credits inflated into headline numbers.
3. **Dated verification.** Every row carries a `last-verified` date. Stale rows get flagged, dead tools go to the [Graveyard](GRAVEYARD.md).

## State of Free — 2026

Since early 2026, OpenAI, Anthropic, and Google have restricted flagship reasoning models to paid tiers; free tiers now get lighter models (GPT-5.5 Instant-class, Claude Haiku/Sonnet-class, Gemini Flash-class). Hyperscaler *always-free services* remain the most durable free compute; VC-subsidized startup free tiers and promo programs are the most volatile — several died mid-2026. Plan accordingly: build on OSS + BYOK where possible, treat hosted free tiers as scaffolding.

## ⚡ Quickstart — the $0 stack in 3 steps

```bash
# 1. Install a free, open-source coding agent in VS Code
code --install-extension saoudrizwan.claude-dev   # Cline

# 2. Get a free API key (no card): https://aistudio.google.com/apikey
#    Point Cline at it: Settings → API Provider → Google Gemini → paste key

# 3. Deploy what you build, free:
npm create cloudflare@latest    # → Cloudflare Pages/Workers, 100K req/day
```

Working agent, free frontier-adjacent model, free hosting — $0, no card, ~5 minutes. Full rotation strategy in [The $0 Pipeline](#the-0-pipeline-rotation-playbook).

## Legend

| Badge | Meaning |
|---|---|
| 🧾 | Primary-source verified (pricing/docs page) |
| ✅ | Corroborated by 2+ independent sources |
| ⏳ | Single-sourced or stale — needs verification (PRs welcome) |
| 🟢 / 🟡 / 🟠 / 🔴 | Generosity: Truly Free / Generous / Moderate / Limited |
| 🏛️ / 🎢 | Durability: hyperscaler-subsidized / VC-subsidized-volatile |
| 🌍 | Regional availability restrictions apply |
| ⚠️ | TOS gotcha — read the fine print column |

Boolean facets per tool (in `tools.json`): `card_required` · `commercial_use_ok` · `trains_on_your_code`

---

## Tier 0 — Fully Free / Open Source

Pay $0 for the tool forever. Bring your own model (free or paid).

| Tool | Type | License | Notes | Verified |
|---|---|---|---|---|
| [Cline](https://github.com/cline/cline) | VS Code agent | Apache-2.0 | 🟢 The BYOK reference standard | ✅ |
| [Roo Code](https://github.com/RooVetGit/Roo-Code) | VS Code agent | Apache-2.0 | 🟢 Cline fork, power-user features | ✅ |
| [Kilo Code](https://github.com/Kilo-Org/kilocode) | VS Code agent | Apache-2.0 | 🟢 Free for individuals, routes to free models | ⏳ |
| [OpenCode](https://github.com/sst/opencode) | Terminal agent | MIT | 🟢 Provider-agnostic CLI agent | ✅ |
| [Aider](https://github.com/Aider-AI/aider) | Terminal agent | Apache-2.0 | 🟢 Git-native pair programmer | ✅ |
| [Continue](https://github.com/continuedev/continue) | IDE extension | Apache-2.0 | 🟢 VS Code + JetBrains | ✅ |
| [bolt.diy](https://github.com/stackblitz-labs/bolt.diy) | Local app builder | MIT | 🟢 OSS Bolt, any model | ✅ |
| [Dyad](https://github.com/dyad-sh/dyad) | Local app builder | Apache-2.0 | 🟢 Local, free, lovable-style | ⏳ |
| [Goose](https://github.com/block/goose) | Terminal agent | Apache-2.0 | 🟢 Block's extensible agent | ✅ |
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) | Autonomous agent | MIT | 🟢 Full dev agent platform | ⏳ |
| [Plandex](https://github.com/plandex-ai/plandex) | Terminal agent | MIT | 🟢 2M-token context engine | ⏳ |
| [Tabby](https://github.com/TabbyML/tabby) | Self-hosted completion | Apache-2.0 | 🟢 Own your Copilot | ⏳ |
| [Twinny](https://github.com/twinnydotdev/twinny) | VS Code + local models | MIT | 🟢 Ollama-native completions | ⏳ |
| [PearAI](https://github.com/trypear/pearai-app) / [Void](https://github.com/voideditor/void) | OSS IDEs | Apache-2.0 | 🟢 Cursor alternatives | ⏳ |
| [GPT Engineer](https://github.com/gpt-engineer-org/gpt-engineer) | CLI scaffolder | MIT | 🟢 Spec → codebase | ⏳ |
| [PR-Agent](https://github.com/The-PR-Agent/pr-agent) | PR review agent | OSS | 🟢 Self-host answer to paid review bots (upstream of Qodo) | ✅ |

**Local models:** [Ollama](https://ollama.com) + open weights (Qwen-Coder, DeepSeek-Coder, IBM Granite (Apache-2.0), Llama, Mistral) = zero token cost if your hardware can carry it.

## Tier 1 — Free API Backends (BYOK fuel)

Pair these with Tier 0 tools for a genuinely $0 pipeline. **Deep reference:** [OmniRoute's 98-provider free-tier audit](https://github.com/diegosouzapw/OmniRoute/wiki/Free-Tiers) — per-provider ToS analysis and confidence ratings; we don't duplicate it, we summarize the coding-relevant cuts.

| Provider | Documented free limit | Gotchas | Verified |
|---|---|---|---|
| [Google AI Studio](https://aistudio.google.com) | Gemini Flash free API; limits cut 50–80% Dec 2025 — check current RPD | ⚠️ Free tier may train on data; limits volatile | ✅ |
| [Mistral La Plateforme](https://console.mistral.ai) | ~1B tokens/mo Experiment tier | ⚠️ Personal-use-only ToS | ✅ |
| [NVIDIA NIM](https://build.nvidia.com) | Permanent free key, 70–100+ models | Rate-limited | ✅ |
| [Groq](https://groq.com) | Free tier, very fast inference | ⚠️ No resale/proxy per ToS | ✅ |
| [Cerebras](https://cloud.cerebras.ai) | ~1M tokens/day free | | ✅ |
| [OpenRouter](https://openrouter.ai) | :free models: 50 req/day, 20 req/min | 💰 One-time $10 credit purchase = 1,000 req/day forever (lifetime unlock, survives $0 balance). ⚠️ Failed requests count against quota | 🧾 |
| [GitHub Models](https://github.com/marketplace/models) | Free playground + API to frontier models | Rate-limited by tier | ⏳ |
| [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/) | 10K neurons/day | 🏛️ | ✅ |
| [GLM / Zhipu](https://open.bigmodel.cn) | GLM-4-Flash free API | 🌍 | ⏳ |
| [LongCat](https://longcat.chat/platform/docs/) | 5M tokens/day (Flash-Chat); Flash-Lite API currently unlimited, 50M/day free tier announced Feb 2026 | 🌍 | ⏳ |
| [Tencent Hunyuan-lite](https://cloud.tencent.com/product/hunyuan) / [iFlytek Spark Lite](https://xinghuo.xfyun.cn/sparkapi) | Permanently free | 🌍 | ✅ |
| [watsonx.ai Lite](https://www.ibm.com/products/watsonx-ai) | Free Lite instance; 1 RU = 1,000 tokens | ⚠️ One Lite instance per account; tuning/GPU excluded; no auto-charge | 🧾 |
| [Cohere](https://cohere.com) | 1,000 API calls/mo trial key | ⚠️ **Production use prohibited in ToS** | ✅ |
| [Anthropic](https://console.anthropic.com) | Limited free trial credits (since Mar 2026) | One-time, not recurring | ⏳ |
| [OpenAI](https://platform.openai.com) | $5 new-account credit | ⚠️ Expires after 3 months | ✅ |

⚠️ **Community norm: don't abuse these.** Proxying, key-pooling, and resale get tiers killed for everyone — 19+ providers already have explicit personal-use/anti-proxy clauses.

### 💰 The cheap permanent unlocks

A pattern most lists miss: several providers run **cumulative-spend tier ladders** - your *lifetime* deposits, not your balance, set your rate limits. One small top-up permanently promotes the account. The cheapest upgrades in AI:

| Provider | The unlock | Status |
|---|---|---|
| [OpenRouter](https://openrouter.ai) | One-time $10 credit purchase: 50 -> 1,000 free-model req/day, forever. Survives a $0 balance | 🧾 |
| [OpenAI API](https://platform.openai.com/docs/guides/rate-limits) | First ~$5 lifetime spend promotes to Tier 1 limits; further tiers by cumulative spend | ⏳ verify thresholds |
| [Anthropic API](https://docs.claude.com) | Deposit-based tier ladder - first deposit permanently lifts rate limits | ⏳ verify thresholds |
| [Gemini API](https://ai.google.dev/gemini-api/docs/rate-limits) | Adjacent pattern: *enabling billing* (no spend) promotes free-tier limits to Tier 1 | ⏳ verify |
| [Together AI](https://www.together.ai) / [Fireworks](https://fireworks.ai) | Build-tier ladders keyed to cumulative spend | ⏳ verify |

Rule of thumb: if you're hitting rate limits on a free tier, check whether the provider's limits are keyed to lifetime spend before you architect around the ceiling - the fix may cost $5, once.

## Foundation Models & Chat Platforms

Vibe coding in a chat/canvas UI — no IDE required.

| Platform | Free coding surface | Notes | Verified |
|---|---|---|---|
| ChatGPT (Canvas) | Free tier, lighter models | 🌍 geo-blocked in some regions | ✅ |
| Claude (Artifacts) | Free tier, Haiku/Sonnet-class | 🌍 | ✅ |
| Gemini | Free chat + Canvas | | ✅ |
| Grok | Free tier on X | | ⏳ |
| Mistral Le Chat | Free, generous | | ✅ |
| DeepSeek | Free chat, strong coder | 🌍 available where US models aren't | ✅ |
| Qwen Chat | Free, Qwen-Coder access | 🌍 | ✅ |
| Kimi | Free chat + kimi-cli | 🌍 | ⏳ |
| HuggingChat | Free open-model chat | | ⏳ |

## Hyperscalers

The durable free compute. 🏛️ = subsidized by cloud revenue, not VC burn — but note AWS proved trial *structures* can still change (Jul 2025).

### Microsoft / GitHub
- **Copilot Free** — 2,000 completions + 50 chat/mo (≈26 hrs of full-time completion use). ⚠️ Free tier sends code-snippet telemetry; paid can opt out. ✅
- **GitHub Codespaces** — ~120 core-hours/mo free cloud dev env ⏳ · **GitHub Models** free playground ⏳

### Google
- **Gemini Code Assist** — free for individuals since Mar 2026: **180K completions/mo (~6K/day), 240 chat/day**, no card. ⚠️ Trains on your code by default — opt out in settings. ✅
- **Gemini CLI** — 1,000 req/day via OAuth; ⚠️ free OAuth tier deprecated Jun 18, 2026 for non-enterprise — verify current status. ✅
- **Firebase Studio / Antigravity / Jules / Colab** — all with free tiers ⏳

### Amazon
- **Amazon Q Developer** — ⚰️ closed to new signups May 15, 2026 ([Graveyard](GRAVEYARD.md)). Existing users grandfathered.
- **Kiro** — free tier ~50 credits/mo ⏳
- **AWS Free Tier (post-Jul 2025)** — new accounts: $100 signup credit + $100 via 5 onboarding tasks; Free Plan auto-closes at 6 months or credit exhaustion (⚠️ 90-day grace, then data deleted). Pre-Jul-2025 accounts grandfathered on legacy 12-month tier. 30+ always-free services (Lambda 1M req/mo, DynamoDB 25GB) remain. ✅

### IBM
- **IBM Cloud Lite** — 40+ always-free products that never expire and **cannot be charged**; $200/30-day new-account credit. 🧾
- **watsonx.ai Lite** — free Granite + foundation-model inference (see Tier 1). 🧾
- **LinuxONE free virtual servers** — ⚠️ s390x architecture, not x86: many Docker images/binaries won't run without s390x builds. 🧾

### Oracle
- **OCI Always Free** — Ampere A1 ARM compute (commonly cited 4 OCPUs + 24GB — verify on detail page), AMD micro instances, 200GB-class block volume, Autonomous DBs, HeatWave, load balancer, even email delivery. The beefiest free VM in the industry. 🧾
- ⚠️ Gotchas (all from Oracle's own FAQ): idle 30+ days = eligible for reclamation (keep-alive cron is standard practice); credit card required (no prepaid/virtual); one account per person; region choice is permanent and popular regions run out of A1 capacity; $300 credit but only 30 days to use it. 🧾

### Cloudflare
- **Workers** 100K req/day · **Pages** free hosting · **Workers AI** 10K neurons/day · **D1 / KV / R2** free tiers · OSS [vibesdk](https://github.com/cloudflare/vibesdk). ✅

---

## Tier 2 — Usable Hosted Free Tiers

| Tool | Free tier | Effective lifespan / burn | Verified |
|---|---|---|---|
| [Bolt](https://bolt.new) | 300K tokens/day, 1M/mo, free hosting | ⚠️ Syncs whole project per message — 50-file app ≈ 200K tokens/prompt; daily tokens don't roll over | 🧾 |
| [Cursor](https://cursor.com) Hobby | Limited agent requests + tab completion (in-house model) | Frontier models need Pro $20/mo | ✅ |
| [Trae](https://trae.ai) | Free access to frontier models | ⚠️ ByteDance — evaluate data routing for client/compliance work | ✅ |
| [Windsurf / Devin Desktop](https://windsurf.com) | ~25 credits/mo | 🎢 pricing changed 3× in a year | ✅ |
| [Supermaven](https://supermaven.com) | 500 completions/day, fastest latency | Completion-only, no chat | ⏳ |
| [Zed](https://zed.dev) | Free editor + AI free allowance | | ⏳ |
| [Google Antigravity](https://antigravity.google) | Free cross-platform agentic IDE | | ⏳ |

## Tier 3 — Demo-Grade Free Tiers

Enough to evaluate, not enough to build on.

| Tool | Free tier | Verified |
|---|---|---|
| [v0](https://v0.dev) | $5 in monthly credits (resets each cycle); Premium $20/mo, Team $30/user | ✅ |
| [Lovable](https://lovable.dev) | 30 credits/mo (5/day cap), then from $25/mo | ✅ |
| [Rocket](https://rocket.new) | 20 free credits; Stripe billing, auth, multi-tenant built in; paid from $25/mo | ⏳ |
| [Base44](https://base44.com) | 25 message credits/mo (Wix-owned), Starter $16/mo | ✅ |
| [Replit](https://replit.com) | Starter tier, credits burn fast. ⚠️ "Free Mode" (Aug 19, 2026) is NOT a free tier — unmetered routine work *for paid subscribers* ($20/mo Core+, GPT-5.6, limits reset every 5 hrs); the actual free plan is unchanged | ✅ |
| [Tencent Cloud Studio](https://cloudstudio.net) | ~1,000 points/mo 🌍 | ⏳ |
| [Baidu Comate](https://comate.baidu.com) | ~500 agent dialogues/mo 🌍 | ⏳ |

## Student & Edu Offers

Status board — half the famous offers died in 2026. ✅ active · ⏸️ paused · ⚰️ ended

| Offer | Status | Detail |
|---|---|---|
| GitHub Student Developer Pack | ✅ | Non-Copilot benefits intact |
| JetBrains free for students | ✅ | Full IDE suite |
| AWS Educate | ✅ | Individual credits |
| Gemini student discount | ✅ | $9.99/mo (50% off) ×12mo via SheerID — the free 12-month promo ⚰️ Jan 2026 |
| GitHub Copilot Pro (students) | ⏸️ | New signups paused Apr 20, 2026; existing users keep it. ⚠️ Conflicting reports — verify before relying on it |
| Cursor free student year | ⚰️ | Closed to new signups Jun 25, 2026; event-based promos expected fall 2026 |
| Windsurf student offer | ⚰️ | Ended with Jun 2026 Devin Desktop rebrand |

**OSS maintainer offers (adjacent):** Anthropic's Claude for Open Source (6 months of Max free for qualifying maintainers) · CodeRabbit, Sweep, Sourcery, Ellipsis free for public/OSS repos.

## Free Deploy & Backend

A vibe-coded app is worthless if hosting costs money. The shortlist that matters:

| Service | Always-free | Gotchas | Verified |
|---|---|---|---|
| Cloudflare Workers/Pages | 100K req/day + free hosting | | ✅ |
| GCP Cloud Run | 2M requests/mo | 🧾 primary-verified | 🧾 |
| GCP e2-micro VM | 1 instance/mo | ⚠️ US free-tier regions only — verify | 🧾 |
| Oracle A1 ARM VM | Biggest free compute anywhere | ⚠️ idle reclamation, capacity roulette | 🧾 |
| Vercel Hobby | Free Next.js hosting | ⚠️ Non-commercial ToS on Hobby | ⏳ |
| Netlify Free | Static + functions | | ⏳ |
| GitHub Pages | Static hosting | | ✅ |
| Supabase Free | Postgres + auth + storage | ⚠️ Pauses after 1 week inactivity | ⏳ |
| Neon Free | Serverless Postgres | | ⏳ |
| **Startup credits** | GCP up to $200K ($350K AI startups) · AWS Activate · Azure founders · IBM $200 | Application required | 🧾 |

For the long tail of infra free tiers → [free-for.dev](https://free-for.dev).

## Free Business Stack

Per category: best hosted, best self-host, and the boring default. New entries must argue out an incumbent.

**Forms:** 🥇 [Tally](https://tally.so) (unlimited forms + responses, no card) · 🟢 [Formbricks](https://formbricks.com) (AGPL, Docker one-liner — what we run in production) · [OpnForm](https://opnform.com) (AGPL, Typeform-style UX) · Google Forms (immortal default)

**Scheduling:** 🥇 [Cal.com](https://cal.com) (free individual plan *and* AGPL self-host — only entry with both) · [Calendly](https://calendly.com) free (1 event type) · Zoho Bookings free (1 user)

## The Subscription Killers

Open-source software that replaces a SaaS bill. Check GitHub before you buy — own the pipeline, rent only the irreplaceable. License matters (AGPL vs fair-code vs MIT changes what you can do commercially) and so does footprint — a Pi-class Go binary and a 3GB container stack are different commitments.

| OSS | Replaces | Cost avoided (USD/mo) | License | ~RAM |
|---|---|---|---|---|
| [Twenty](https://github.com/twentyhq/twenty) | Salesforce / HubSpot CRM | $25–100/seat | AGPL-3.0 | 2GB |
| [n8n](https://github.com/n8n-io/n8n) | Zapier | $30–100 | Fair-code ⚠️ | 768MB |
| [Formbricks](https://github.com/formbricks/formbricks) / [OpnForm](https://github.com/JhumanJ/OpnForm) | Typeform | $29 | AGPL-3.0 | ~1GB |
| [Cal.com](https://github.com/calcom/cal.com) | Calendly | $12 | AGPL-3.0 | 1–2GB |
| [Plausible](https://github.com/plausible/analytics) / [Umami](https://github.com/umami-software/umami) | Paid analytics | $9–19 | AGPL-3.0 / MIT | 2GB / 384MB |
| [Chatwoot](https://github.com/chatwoot/chatwoot) | Intercom / Zendesk | $39–100/seat | MIT | 2GB |
| [Listmonk](https://github.com/knadh/listmonk) | Mailchimp | $20–100 | AGPL-3.0 | 96MB 🥧 |
| [Documenso](https://github.com/documenso/documenso) | DocuSign | $15–25 | AGPL-3.0 | 1GB |
| [Invoice Ninja](https://github.com/invoiceninja/invoiceninja) | FreshBooks | $19–30 | Elastic 2.0 ⚠️ | 768MB |
| [NocoDB](https://github.com/nocodb/nocodb) | Airtable | $20/seat | AGPL-3.0 | 512MB |
| [Supabase](https://github.com/supabase/supabase) / [PocketBase](https://github.com/pocketbase/pocketbase) | Firebase paid | $25–50 | Apache-2.0 / MIT | 3GB / 64MB 🥧 |
| [Uptime Kuma](https://github.com/louislam/uptime-kuma) | Pingdom | $15 | MIT | 256MB |
| [Metabase](https://github.com/metabase/metabase) | Tableau / Looker | $75–500 | AGPL-3.0 | 2GB |

🥧 = Pi-class (runs on a Raspberry Pi or the smallest free VM) · ⚠️ = not OSI-approved open source — fine to self-host for your own use, restrictions apply to reselling it as a service · RAM figures are rough self-host baselines, not benchmarks.

**Total displaced: $321–1,088/mo** — computed from `tools.json` (single-seat, low-end paid plans; paired alternatives counted once). Long tail → [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted).

## Supporting Stack

**Cloud sandboxes:** StackBlitz · CodeSandbox free · Glitch ⏳
**Notebooks/GPU:** Colab free · Kaggle (~30 GPU hrs/wk) · Lightning AI (free GPU hrs/mo) · Deepnote · Hex ⏳
**Assets/audio (for game/app vibe coding):** free tiers of Suno, ElevenLabs; open 3D gen (Trellis, Hunyuan3D) ⏳
**Context tools:** uithub · Context7 · RepoPrompt ⏳

## Meta-Tools

- [NextReset](https://nextreset.ai/) — free Codex reset-history and official AI-service incident resource. Personal timers stay in the browser; it does not read account usage. Verified 2026-09-18.
- [onWatch](https://github.com/onwatch) — quota tracking across providers ⏳ · vibe-kanban · Task Master
- [OmniRoute](https://github.com/diegosouzapw/OmniRoute) — free-tier aggregation gateway. ⚠️ Routing providers through proxies violates several providers' ToS — read their own wiki's warnings first.
- [freellmapi](https://github.com/tashfeenahmed/freellmapi) — OpenAI-compatible proxy stacking 28 providers' free tiers behind one `/v1` endpoint. ⚠️ Twice-flagged: the "~4B tokens/month" headline is theoretical-ceiling math (documented recurring across the ecosystem is closer to ~2B — see honest accounting, rule 2), and proxy-stacking free tiers sits in the ToS gray-to-red zone for many of the 28 providers. Popular (17k+ ⭐), so listed — with eyes open.

## The $0 Pipeline (Rotation Playbook)

Idea → deployed, no card required:

1. **Scaffold** the UI in a hosted builder's free tier (Bolt / v0) — burn their tokens on boilerplate
2. **Export** and switch to Tier 0 + BYOK (Cline or Roo + Gemini Flash via AI Studio, or Mistral's free tier) for real iteration
3. **Heavy lifting** on free GPU (Kaggle / Colab) when you need training or batch work
4. **Deploy** to Cloudflare Pages/Workers or GCP Cloud Run; database on Supabase/Neon free
5. **Back office** free: Tally forms, Cal.com scheduling, n8n automation, Twenty CRM
6. **Rotate** when a tier tightens — this repo's [CHANGELOG](CHANGELOG.md) tracks the tightenings

## Related Directories & Guides

- [free-for.dev](https://free-for.dev) — the genre's founding document (SaaS/infra free tiers)
- [awesome-vibe-coding](https://github.com/filipecalegario/awesome-vibe-coding) — the canonical tool taxonomy (CC0)
- [EnzeD/vibe-coding](https://github.com/EnzeD/vibe-coding) — methodology & memory-bank workflow
- [easy-vibe](https://github.com/datawhalechina/easy-vibe) — full vibe-coding course, 10 languages
- [OmniRoute Free-Tiers wiki](https://github.com/diegosouzapw/OmniRoute/wiki/Free-Tiers) — 98-provider API audit
- [ShaikhWarsi/free-ai-tools](https://github.com/ShaikhWarsi/free-ai-tools) — broad free AI tools list
- [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) — 100+ runnable agent/RAG templates: *what to build*; this repo is *what to build it with for $0* — our [Tier 1 backends](#tier-1--free-api-backends-byok-fuel) power those templates free
- [stack-on-a-budget](https://github.com/255kb/stack-on-a-budget) · [heroku-free-alternatives](https://github.com/meanands/heroku-free-alternatives) — adjacent free-tier lists
- [ClawLabsAI/free-ai-models](https://github.com/ClawLabsAI/free-ai-models) — auto-generated daily free-model tracker (OpenRouter API). Good for model IDs; rate limits thin, ZeroLimitAI-affiliated
- [12britz/awesome-free-models](https://github.com/12britz/awesome-free-models) — broad models/local-inference list (CC0). Wide but shallow — no tier limits; verify pricing here
- [CYBIRD-D/FREE-LLM-API-Provider](https://github.com/CYBIRD-D/FREE-LLM-API-Provider) — free LLM APIs with CN-platform coverage Western lists miss
- [eudk/awesome-edu-deals](https://github.com/eudk/awesome-edu-deals) — broad student/edu software deals (no status tracking — see our [student board](#student--edu-offers) for AI-coding offers)
- [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) · freetiers.com · freestuff.dev · tolop.vercel.app

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md). Short version: pricing-page receipts required, announcement posts don't count, permanent free ≠ trial, and the headline count must equal `tools.json` length.

## License

[CC BY 4.0](LICENSE) — share and adapt freely, attribution to DarkDataLabs required.

---

⭐ **Star this repo to catch free-tier changes before they bite you** — the [CHANGELOG](CHANGELOG.md) tracks every tightening, and the [Graveyard](GRAVEYARD.md) grows every year.
