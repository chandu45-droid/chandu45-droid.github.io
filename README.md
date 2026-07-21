# Steal Deals Hub — deals site (gh-pages)

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
