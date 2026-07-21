# chandu45-droid.github.io

This repo hosts **3 static sites**, all served from GitHub Pages on a single domain:

| Path | Site | What |
|---|---|---|
| [`/`](https://chandu45-droid.github.io/) | **Steal Deals Hub** | Deals redirect layer for the Steal Deals Telegram channel |
| [`/portfolio/`](https://chandu45-droid.github.io/portfolio/) | **Portfolio** | Showcase of 4 AI-built products |
| [`/pm-simulator/`](https://chandu45-droid.github.io/pm-simulator/) | **PM Simulator** | Daily PM decision-making game with a share loop |

---

## Steal Deals Hub (`/`)

Static redirect layer for the Steal Deals Telegram channel (`@steal_deals_hub`).

**Why this exists:** Amazon Associates policy does not permit posting affiliate
links directly into messaging apps. The bot publishes every deal here first;
Telegram posts link to `index.html#deal-<ASIN>` on this page, and the affiliate
link lives only on this page.

- `index.html` — the deals page (single file, no build step)
- `deals.json` — rolling deal feed, written by `steal-deals-bot/site_publisher.py`
  on the `master` branch of this repo

Do not edit `deals.json` by hand — the bot overwrites it every cycle.

As an Amazon Associate, Steal Deals Hub earns from qualifying purchases.

## Portfolio (`/portfolio/`)

A project showcase page presenting 4 AI-built products: PM Simulator, Sortd,
Cricket Underworld, and Data Product Assistant. No separate repo — lives
entirely under `portfolio/` in this repo.

## PM Simulator (`/pm-simulator/`)

A daily PM decision-making game — players work through a scenario beat each
day and share their results. No separate public repo; the game lives entirely
under `pm-simulator/` in this repo.
