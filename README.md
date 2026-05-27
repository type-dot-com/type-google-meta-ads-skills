# Type Google and Meta Ads Skills

Open-source skill collection for connecting Google Ads and Meta Ads workflows to a Type AI teammate.

This repository is designed for Type's GitHub skill import flow. Paste the repository URL into the Type channel skill importer and select the skills you want to add.

## Google Ads Skills

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

## Meta Ads Skills

| Skill | What it does | Suggested cadence |
| --- | --- | --- |
| `skills/meta-ads-command-center` | Orchestrates Meta Ads analysis, routing, change control, source discovery, and paid-social reporting standards. | Always on |
| `skills/meta-account-audit` | Runs a read-only account audit across tracking, campaign structure, delivery, creative, audience, and measurement health. | First run, then monthly |
| `skills/meta-performance-monitor` | Reviews spend, pacing, ROAS or CPA, CPM, link CTR, frequency, anomalies, and delivery status. | Daily or weekly |
| `skills/meta-creative-fatigue` | Diagnoses creative fatigue, weak hooks, format gaps, placement fit, and refresh priorities. | Weekly |
| `skills/meta-audience-delivery` | Reviews audience overlap, broad or lookalike strategy, retargeting, placements, learning phase, and delivery constraints. | Biweekly |
| `skills/meta-budget-scaling` | Builds budget, CBO or ABO, and scaling recommendations using ROAS, CPA, MER, frequency, and learning-phase guardrails. | Weekly |
| `skills/meta-revenue-attribution` | Connects Meta spend to Shopify, GA4, HubSpot, Salesforce, or BI revenue and pipeline data. | Weekly or monthly |

## Importing Into Type

1. Open the target Type AI teammate channel.
2. Go to channel settings, then skills.
3. Choose import from GitHub.
4. Paste this repository URL.
5. Import the skills you want.

The skills are written for Google Ads, formerly Google AdWords, and Meta Ads, formerly Facebook Ads. They avoid assuming a specific tool surface beyond what the user's Type channel has connected. They tell the Type AI teammate to discover available Ads, analytics, CRM, ecommerce, spreadsheet, document, and notification tools before acting.

## Setup

After importing, users should edit the imported skills or ask the Type AI teammate to customize them:

```text
Customize these Google and Meta Ads skills for our accounts, conversion goals, reporting cadence, risk tolerance, revenue sources, CRM, and approval rules.
```

Useful details to add directly to the imported skill instructions:

- Google Ads manager account and client account names
- Meta business manager, ad account, Pixel, and Conversions API status
- timezone, currency, and reporting calendar
- primary conversion actions and attribution model
- account goal: CPL, CPA, ROAS, MER, pipeline, revenue, or share of voice
- budget guardrails and pacing rules
- campaigns, products, regions, audiences, creative concepts, and brands to prioritize
- whether the Type AI teammate may apply low-risk changes or only draft recommendations
- negative keyword, bid, budget, pause, audience, creative, and asset approval rules
- ecommerce, analytics, and CRM sources such as Shopify, GA4, HubSpot, or Salesforce
- default update channel and executive summary recipients

## Change Control

By default, these skills should monitor, summarize, draft, and recommend. They should not change budgets, bids, campaign status, ad set status, ads, audiences, negative keywords, final URLs, conversion tracking, Pixel or CAPI settings, or CRM data unless the imported skill instructions explicitly grant that authority.

## Design Notes

This is a Type-oriented paid ads skill collection. The Google Ads section is inspired by a practical paid-search agent roster: campaign monitor, search term intelligence, keyword health, ad copy performance, geo/device/schedule analysis, competitive intelligence, monthly executive summary, and pipeline reporting. The Meta Ads section is conceptually inspired by [NotFair](https://github.com/nowork-studio/NotFair)'s public Meta Ads audit and manage split, rewritten around Type's connected-app model rather than NotFair's MCP and filesystem contract. It does not copy proprietary playbooks or private account data.

## License

MIT. See `LICENSE`.
