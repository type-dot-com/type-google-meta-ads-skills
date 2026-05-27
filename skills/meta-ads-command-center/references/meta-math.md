# Meta Ads Math

Use this reference when a finding needs dollar-denominated impact, profitability framing, or a forecast.

## Core Formulas

```text
CPM = spend / impressions * 1000
CPC = spend / link clicks
Link CTR = link clicks / impressions * 100
Hook rate = 3-second video views / impressions * 100
Hold rate = thruplays / 3-second video views * 100
CPA = spend / results
ROAS = purchase conversion value / spend
Frequency = impressions / reach
Landing page CVR = landing page conversions / landing page views * 100
MER = total business revenue / total marketing spend
```

Use link clicks for CTR and CPC unless the user explicitly asks for all clicks. All clicks include engagement actions that may not send a user to the destination.

## Profitability

When AOV and gross margin are known:

```text
Break-even ROAS = 1 / gross margin
Break-even CPA = AOV * gross margin
Unit profit = AOV * gross margin - CPA
Headroom = (break-even CPA - current CPA) * monthly conversions
```

When lead-to-customer rate is known:

```text
Break-even lead CPA = AOV * gross margin * lead-to-customer rate
```

Do not compute break-even from guessed margin unless the output is clearly labeled as an estimate and the user is asked to confirm it before any account mutation.

## Interpretation Rules

- Meta is bought on impressions, so CPM and frequency often explain performance changes before CPC does.
- ROAS is useful for ecommerce ad sets, but it is platform-attributed and depends on the attribution setting.
- CPA is useful for lead generation and SaaS, but downstream CRM quality matters more than cheap leads.
- MER is a portfolio metric and should not be used to judge a single ad set.
- A budget increase under creative fatigue usually amplifies the problem.
- A budget change that is too large can destabilize delivery and should be staged.

## Fatigue Heuristic

Treat creative fatigue as likely when multiple signals align:

- frequency is rising
- CPM is rising week over week
- link CTR is falling week over week
- video hook rate is falling, if video metrics exist
- no tracking, landing page, or seasonality issue explains the change

For cold prospecting, high frequency plus rising CPM is usually a creative or audience saturation problem. For warm retargeting, higher frequency may be acceptable, but falling CTR or rising CPA still warrants a refresh.

## Forecasting

Use three scenarios when forecasting scale:

```text
Projected spend = daily budget * days in period
Projected conversions = projected spend / historical CPA
Projected revenue = projected conversions * AOV
```

Cap projections at a reasonable range around observed spend. Call out that doubling spend rarely doubles results on Meta because audience saturation and learning effects create diminishing returns.

