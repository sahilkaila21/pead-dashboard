# PEAD Strategy Backtest Dashboard

A self-contained, interactive backtest dashboard for a post-earnings-announcement
drift (PEAD) trading strategy: 85 liquid large-cap US stocks, 2019–2026, earnings
surprise as the sole entry signal, ATR-based risk management.

**Live page:** published via GitHub Pages from this repo (see repo settings for the URL).

## What's here

Just `index.html` — a single static file with all backtest data (472 trades,
equity curve, per-trade explanations) embedded directly in the page. No backend,
no build step, no external dependencies. Everything runs in your browser:

- Full backtest metrics, equity curve, and walk-forward results by year
- A searchable/sortable table of every trade
- A **Trade Inspector**: click any trade to see exactly why it fired (the
  earnings surprise %, ATR-based stop, hold period) and why it closed
- **Historical playback**: step through all 472 trades chronologically
- A **Simulation Lab**: enter your own capital and time horizon, and it
  bootstrap-resamples the actual historical trades to show a realistic range
  of outcomes (not a single optimistic projection)

## What this is not

This repo intentionally contains **only the dashboard**, not the trading
engine, backtest code, or strategy configuration — those live in a separate
private repository. This is a snapshot of results for reference and
discussion, not a live or updating page.

Research/backtest only — not investment advice, not live trading.
