# AI Subscription Plans

Every AI subscription plan in the [Tech Unbloated AI subscription finder](https://techunbloated.com/tools/best-ai-subscription/): 228 plans from 66 tools, with monthly prices checked against each vendor's own pricing page.

It covers eleven kinds of plan: coding, chat and writing, task agents, always-on agents, image, video, music, voice, design and websites, research, and all-in-one bundles. Only plans you can buy with a normal card are included. Region-locked deals and API pay-as-you-go pricing are left out.

If you just want the plan that fits how you work, [use the finder](https://techunbloated.com/tools/best-ai-subscription/). This repo is for anyone who wants the raw table.

## Files

- `plans.csv`: one row per plan. List fields are separated by `; `.
- `plans.json`: the same rows, with lists kept as arrays, plus the catalog date.

## Columns

| Column | What it holds |
|---|---|
| `tool` | Product name |
| `plan` | Plan name as the vendor sells it |
| `price_monthly_usd` | Published monthly price in US dollars when billed monthly. Blank means the price could not be confirmed |
| `seat_type` | `individual` or `business` |
| `categories` | Which finder tracks the plan appears in: `code`, `chat`, `agent`, `always-on`, `image`, `video`, `music`, `voice`, `design`, `academic` (research), `aggregate` (all-in-one) |
| `surfaces` | Where you use it, such as `web-app`, `chat`, `ide-extension`, `terminal-agent`, `mobile-app`, `plugin` |
| `included_volume` | What the plan includes, in the vendor's own units (credits, messages, requests, or minutes) |
| `session_cap`, `weekly_cap` | Short-window and weekly limits, where the vendor publishes them |
| `overage_behavior` | What happens at the limit: `hard-cap`, `paid-overage`, or blank when the vendor doesn't say |
| `model_tier` | `frontier`, `balanced`, or `cheap-pool`; blank where it does not apply |
| `models` | Models the plan includes, as listed by the vendor |
| `confidence` | `official` (vendor page), `secondary` (reputable third party), or `confirm` (needs a fresh check) |
| `verified_date` | When that row was last checked |
| `pricing_url` | The vendor's pricing page |

## How fresh it is

Prices and limits move every month. The catalog is re-checked against vendor pages monthly, and this repo is updated with it. Every row carries its own `verified_date`, so check the vendor page before you pay. Local taxes and regional prices can differ from the US dollar figures here.

Found a price that's wrong? Open an issue with the vendor link.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use it, change it, or build on it, commercially too. Credit "Tech Unbloated" with a link to https://techunbloated.com/tools/best-ai-subscription/.
