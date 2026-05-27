# Change Control Policy

Use this policy before applying any Meta Ads, tracking, analytics, ecommerce, or CRM mutation.

## Risk Levels

- `low` - report generation, saved view creation, task creation, internal draft, brief creation, or annotation.
- `medium` - budget recommendation, pause recommendation, creative refresh brief, audience recommendation, placement recommendation, or naming cleanup plan.
- `high` - budget edit, campaign status edit, ad set status edit, ad status edit, optimization event edit, attribution edit, audience edit, placement edit, creative edit, Pixel or CAPI setting edit, or CRM attribution edit.
- `critical` - billing, account access, pixel deletion, event deletion, conversion configuration deletion, customer list uploads, large campaign restructuring, automated bidding strategy switch, or changes affecting many campaigns.

## Default Permission

By default, only `low` actions may be completed without approval. `medium` actions should be drafted or recommended. `high` and `critical` actions require explicit imported-skill authority or approval in the current thread.

## Approval Checklist

Before applying a medium-risk or higher mutation, confirm:

- account, campaign, ad set, and ad scope
- exact change list
- current value and proposed value
- date range and evidence
- expected impact
- learning-phase or attribution risk
- rollback path
- owner who approved the change
- whether the change should be logged or annotated

## Never Auto-Apply

Never auto-apply these unless the imported skill instructions name the exact allowed case:

- budget increases or decreases
- campaign, ad set, or ad pauses
- optimization event changes
- attribution setting changes
- audience targeting changes
- placement changes
- ad creative launches or replacements
- Pixel, CAPI, event, or deduplication changes
- billing, access, account-linking, or catalog changes
- customer list uploads or removals
- CRM lifecycle, revenue, or attribution field edits

## Safe Draft Format

```text
Proposed change: <specific edit>.
Scope: <account/campaign/ad set/ad>.
Current value: <current setting>.
Proposed value: <new setting>.
Evidence: <metric window and finding>.
Expected impact: <plain-language expectation>.
Risk: <learning, attribution, policy, or revenue risk>.
Rollback: <how to undo>.
Approval needed: <yes/no and from whom>.
```

