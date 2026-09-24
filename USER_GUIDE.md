# WICK User Guide

WICK is a personal FX trading journal that runs entirely in your browser — no login, no install, no server.

**App:** https://git-papichulo.github.io/wick/

## Getting Started

- The first time you open WICK, a **Main Account** is created automatically and the **Sumi Ink** theme is applied.
- Tap the **☰ menu** (top-right of most screens) to open the sidebar and jump between the five sections: **Dashboard, Journal, Plan & Prep, Learning, Settings & Tools**.
- Tap **Add Trade** any time to log a trade.

## Dashboard

Your at-a-glance overview:
- **Risk Monitor** — how close you are to your daily/weekly loss limits
- **Recent Trades** — your latest entries
- **Performance** — win rate, P&L, and related stats
- **Equity Curve** — balance over time
- **Watchlist** — add pairs you want to track (e.g. EURUSD, XAUUSD); live prices need a free Alpha Vantage API key (see Settings below)

## Adding a Trade

Tap **Add Trade**, then choose a mode:

- **Open Trade** — you've just entered a position and haven't closed it yet. Fill in Symbol, Direction, Strategy, Session, Entry, Stop Loss, Take Profit, and Lot Size — R:R is calculated automatically. Close it later from the Journal.
- **Closed Trade** — you're logging a trade that's already finished. Same fields, plus Exit Price and Final PnL.

Either mode lets you attach a screenshot and add notes — useful for reviewing psychology/execution later.

## Journal

Your full trade history:
- Filter by **status** (All / Open / Closed) and sort as needed
- Tap a trade to see full details, edit it, or close an open position
- Deleting a trade cannot be undone

## Plan & Prep

Two tabs:
- **Plan** — your pre-trade prep workspace
- **TOS Decision** — a step-by-step assistant that walks you through the decision before you take a trade

## Learning Center

Built-in reference material, organized by strategy:
- Candle Range Theory (CRT)
- ICT (Inner Circle Trader concepts)
- Smart Money Concepts (SMC)
- Callisto FX Methodology
- Classic Support & Resistance
- Trend Following
- Liquidity Sweep Strategy

Plus a glossary covering terms like NY AM Killzone, Overnight High & Low, PDH/PDL, Swing Points, and more.

## Settings & Tools

Four sub-tabs:

**Settings**
- Risk per Trade (%), Minimum R:R, Daily/Weekly Loss Limit — these drive the Dashboard's Risk Monitor
- Alpha Vantage API key — paste a free key ([get one here](https://www.alphavantage.co/support/#api-key)) to power the Dashboard watchlist's live prices (free tier: ~25 requests/day, 5/min)
- Appearance — pick from 4 themes: Sumi Ink, Indigo Market, Forest Clay, Teal Gold

**Accounts**
- Each account has its own currency, broker, trades, balance, and watchlist
- Add, switch between, or delete accounts from here
- Deleting an account with existing trades asks you to first move them to another account — otherwise they're kept in storage but no longer reachable from any account

**Ledger**
- 30-day view of every transaction affecting your account balance
- **Audit Balance** to check your balance matches your trade history
- **Clear Ledger / Clear Trades / Reset Balance** — all destructive and permanent, use with care

**Backup**
- **Export** — download all your data as a JSON file
- **Import** — restore from a previously exported JSON file

## Data & Privacy

WICK stores everything locally in your browser (IndexedDB/localStorage) — nothing is sent to a server. This means:
- Your data only exists on the device/browser you used to enter it
- Clearing site data, switching browsers, or using a different device gives you a fresh, empty app
- **Back up regularly** via Settings & Tools → Backup → Export, especially before clearing browser data or switching devices

## Tip: add it to your phone's home screen

WICK isn't an installable app (no PWA prompt), but you can still create a shortcut: open the app in your mobile browser, then use the browser's menu → **Add to Home Screen**. It opens like an app, still running from the same browser storage.
