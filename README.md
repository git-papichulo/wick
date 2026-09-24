# WICK — Personal Trading Plan

A single-file, offline-first trading journal for FX traders. No build step, no backend, no login — open it and start logging trades.

**Live app:** https://git-papichulo.github.io/wick/

## Features

- **Dashboard** — risk monitor, recent trades, performance summary, equity curve, and a price watchlist
- **Add Trade** — log an *open* position or a finished *closed* trade: entry/stop/target, lot size, auto-calculated R:R, an optional screenshot, and notes
- **Journal** — full trade history, filterable by open/closed status and sortable; close an open position later, edit, or delete
- **Plan & Prep** — a pre-trade planning workspace plus a step-by-step **TOS Decision Assistant**
- **Learning Center** — built-in lessons (CRT, ICT, Smart Money Concepts, Callisto FX, Support & Resistance, Trend Following, Liquidity Sweep) and a glossary of trading terms
- **Accounts** — multiple trading accounts, each with its own currency, broker, balance, trades, and watchlist
- **Ledger** — 30-day account ledger with a balance audit tool
- **Backup / Restore** — export and re-import all data as JSON
- **4 built-in themes** — Sumi Ink, Indigo Market, Forest Clay, Teal Gold

See [USER_GUIDE.md](./USER_GUIDE.md) for how to use each of these.

## Tech

- Single self-contained `index.html` — no framework, no build tools, no server
- Data stored locally in the browser (IndexedDB/localStorage) — nothing is sent anywhere
- Optional [Alpha Vantage](https://www.alphavantage.co/support/#api-key) free API key powers the Dashboard watchlist's live prices

## Running it

Open the hosted copy — **https://git-papichulo.github.io/wick/** — or download `index.html` and open it directly in any modern browser.

Because everything lives in browser storage, use **Settings & Tools → Backup → Export** periodically. Clearing site data or switching browsers/devices otherwise means starting from a blank slate.

## Deployment

Served as-is via GitHub Pages from the `main` branch root — `index.html` *is* the app. Updating the app is just committing a new `index.html`.

## Related

WICK also exists as a full Lovable/Supabase web app at [wicktradingplan.lovable.app](https://wicktradingplan.lovable.app) — a separate codebase. This repo is the standalone, no-backend version.
