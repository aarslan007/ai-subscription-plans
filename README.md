# AI Subscription Plans

Every AI subscription plan behind Tech Unbloated's [best AI subscription guide](https://techunbloated.com/tools/best-ai-subscription/) and [best AI for coding](https://techunbloated.com/tools/best-coding-plan/): 227 plans from 66 tools, with monthly prices checked against each vendor's own pricing page.

It covers eleven kinds of plan: coding, chat and writing, task agents, always-on agents, image, video, music, voice, design and websites, research, and all-in-one bundles. Only plans you can buy with a normal card are included. Region-locked deals and API pay-as-you-go pricing are left out.

If you just want to know which plan to buy, [read the guide](https://techunbloated.com/tools/best-ai-subscription/): it picks one for each job, from chat and coding to video and voice. This repo is for anyone who wants the raw table.

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
| `categories` | Which uses the plan covers: `code`, `chat`, `agent`, `always-on`, `image`, `video`, `music`, `voice`, `design`, `academic` (research), `aggregate` (all-in-one) |
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

Prices and limits move every month. We run a price check against vendor pages each month and update this repo after it. Not every row is re-checked every month, so each one carries its own `verified_date`. Check the vendor page before you pay. Local taxes and regional prices can differ from the US dollar figures here.

Found a price that's wrong? Open an issue with the vendor link.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use it, change it, or build on it, commercially too. Credit "Tech Unbloated" with a link to https://techunbloated.com/tools/best-ai-subscription/.
