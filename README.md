# Type Google Ads Skills

Open-source skill collection for building a Type sidekick that can monitor, analyze, and recommend improvements for Google Ads programs.

This repository is designed for Type's GitHub skill import flow. Paste the repository URL into the Type channel skill importer and select the skills you want to add.

## Skills

| Skill | What it does | Suggested cadence |
| --- | --- | --- |
| `skills/google-ads-command-center` | Orchestrates Ads analysis, routing, change control, source discovery, and reporting standards. | Always on |
| `skills/campaign-monitor` | Reviews week-over-week campaign metrics, budget pacing, anomalies, and search term flags. | Daily |
| `skills/search-term-intelligence` | Finds waste, mines positive terms, clusters themes, and drafts negative keyword changes. | Weekly, Monday |
| `skills/keyword-health` | Reviews quality scores, keyword-level CPL or CPA, bid recommendations, and pause candidates. | Weekly, Tuesday |
| `skills/ad-copy-performance` | Analyzes responsive search ad assets, headline and description effectiveness, and creative fatigue. | Biweekly |
| `skills/geo-device-schedule` | Reviews location, device, day-of-week, and hour-of-day performance with bid adjustment recommendations. | Biweekly |
| `skills/competitive-intelligence` | Reviews auction insights, impression share trends, competitor movement, and defensive opportunities. | Weekly, Thursday |
| `skills/monthly-executive-summary` | Produces a month-over-month executive rollup with budget reallocation recommendations and strategic narrative. | Monthly |
| `skills/pipeline-report` | Connects Google Ads spend to HubSpot CRM pipeline, demos, deal stages, and closed revenue. | Weekly, Monday |

## Importing Into Type

1. Open the target sidekick channel in Type.
2. Go to channel settings, then skills.
3. Choose import from GitHub.
4. Paste this repository URL.
5. Import the skills you want.

The skills are written for Google Ads, formerly Google AdWords, but they avoid assuming a specific tool surface beyond what the user's Type channel has connected. They tell the sidekick to discover available Google Ads, analytics, CRM, spreadsheet, document, and notification tools before acting.

## Setup

After importing, users should edit the imported skills or ask the sidekick to customize them:

```text
Customize these Google Ads skills for our account, conversion goals, reporting cadence, risk tolerance, CRM, and approval rules.
```

Useful details to add directly to the imported skill instructions:

- Google Ads manager account and client account names
- timezone, currency, and reporting calendar
- primary conversion actions and attribution model
- account goal: CPL, CPA, ROAS, pipeline, revenue, or share of voice
- budget guardrails and pacing rules
- campaigns, products, regions, and brands to prioritize
- whether the sidekick may apply low-risk changes or only draft recommendations
- negative keyword, bid, budget, pause, and asset approval rules
- CRM source such as HubSpot or Salesforce, including lifecycle stages to count
- default update channel and executive summary recipients

## Change Control

By default, these skills should monitor, summarize, draft, and recommend. They should not change budgets, bids, campaign status, negative keywords, final URLs, conversion tracking, or CRM data unless the imported skill instructions explicitly grant that authority.

## Design Notes

This is a Type-oriented Google Ads skill collection inspired by a practical paid-search agent roster: campaign monitor, search term intelligence, keyword health, ad copy performance, geo/device/schedule analysis, competitive intelligence, monthly executive summary, and pipeline reporting. It does not copy proprietary playbooks or private account data.

## License

MIT. See `LICENSE`.

