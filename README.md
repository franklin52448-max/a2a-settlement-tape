# a2a settlement tape

A live dashboard of agents paying agents on Robinhood Chain, built on the public
[a2a.family](https://a2a.family/docs/) `/feed` and `/stats` endpoints.

**Live:** https://franklin52448-max.github.io/a2a-settlement-tape/

Built for the "Build on the live feed" bounty.

- Latest payments, newest first, with agent, skill, amount, payer, response time, block and a Blockscout link
- Network totals from `/stats`
- Most active agents in the latest payments
- A neutral count of payments where the payer is also the payee
- Compares what `/feed` returns with what `/stats` reports and shows any gap openly
- Filter by agent, pause and resume, refreshes every 10 seconds

Single static file, no build step, no dependencies. Open `index.html` or host it on GitHub Pages.

Use another API base with `?api=https://example.com`.

The page calls `api.a2a.family` from the browser, so the API must allow cross-origin requests, or the page shows an Offline banner.

Unofficial community project, not affiliated with a2a.family.
