# Unity Prism — Ads Measurement Intelligence Platform

A signal intelligence platform for Unity Ads measurement — 25-layer funnel measurement intelligence, publisher signal health monitoring, revenue gap analysis, and AI-powered intelligence feed.

**Live demo:** [ai-products-builder.github.io/unity-prism](https://ai-products-builder.github.io/unity-prism)

---

## What it does

Unity Prism maps the complete Unity Ads signal chain — from Source App engine data at L0a through Vector AI bid optimization to Advertised App ROAS retraining at L27. It gives product and measurement teams a single view of where signal quality degrades and what to fix.

**Signal Funnel** — 25-layer interactive cone. Click any layer to inspect its key metric, formula, error codes, and PM action items. Layers are color-coded by Unity product owner (Engine, Analytics+Firebase, SDK, LevelPlay, Vector AI, MMP, Acquire).

**Signal Health Monitor** — Three-tier framework across 6 publishers. Tier 1: Integration Health (SDK version, identity coverage). Tier 2: Data Quality (MMP match rate, SKAN postback rate, Firebase/GA coverage, engine signal coverage L0a/L0b). Tier 3: Monetization Impact (D7 ROAS delta, Vector model confidence, D28 ROAS readiness).

**Revenue Gap Analyzer** — Filter by publisher × format × country. Shows root cause per funnel layer with specific error codes, diagnostic questions, and fix actions. 7-day gap shown vs top performer in same genre.

**Intelligence Feed** — Four tabs:
- *Insights* — Six chart cards with Claude-generated recommendations
- *Competitor* — Publisher benchmarking vs network median, format-adjusted
- *What-If* — Five sliders projecting revenue impact of signal improvements
- *Publisher Briefing* — Claude generates a structured PM briefing per publisher

---

## Stack

- Single-file HTML — no build step, no dependencies
- Chart.js 4.4.1 for data visualization
- Claude API for AI-powered recommendations and publisher briefings
- 1,008-record embedded dataset (Last 7 days, 6 publishers, 6 DSPs, 8 countries, 3 formats)
- Deployed on GitHub Pages

---

## Setup

### 1. Clone and deploy

```bash
git clone https://github.com/ai-products-builder/unity-prism.git
```

Push `index.html` to your `main` branch. Enable GitHub Pages under **Settings → Pages → Deploy from branch → main**.

---

## Data

The embedded dataset covers direct SDK traffic only. Key stats:

| Metric | Value |
|--------|-------|
| Total impressions | 1,153,336 |
| 7-day revenue | $14,656 |
| Avg eCPM | $10.20 |
| Vector AI D7 ROAS | 35.2% |
| External DSP avg D7 ROAS | 29.5% |
| Publishers | Rollic Games, Voodoo, Scopely, Jam City, Zynga, Miniclip |
| Formats | Rewarded, Interstitial, Banner |
| Countries | US, UK, JP, DE, FR, AU, BR, IN |

---

## Files

```
unity-prism/
├── index.html              # Complete application (single file)
├── data.json               # Full 1,008-record dataset
└── README.md
```

---

## License

© 2026 Preethi Sannathi — AI Builder. All rights reserved.
