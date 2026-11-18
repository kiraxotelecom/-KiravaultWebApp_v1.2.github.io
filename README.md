# KiraVault (web)

Plan, Work, Grow: your finances and work in one place. KiraVault answers one question: **how much can I safely spend?**

It tracks Bank, Mobile Money and Cash, counts bills, debts and savings as commitments, and never counts client money until it is actually received.

**Current version: 2.2.0** · see [CHANGELOG.md](CHANGELOG.md)

## What's new in 2.2.0
- Tap Safe to spend to see the arithmetic ("Why this number?")
- Undo (8 seconds) for edits, not only deletes
- Gentle Safe-to-spend alerts, a one-line Install bar, "Same as last time" chips, Android share target for SMS, one-tap backup file

## Also in 2.1.10
- Charts replay when scrolled into view, when you return after 30 s+, and after a sync
- Optional "Repeat every 10 s" switch in Settings (off by default)

## Also in 2.1.9
- Animations on/off switch in Settings
- Donut and Finance overview charts animate
- Quieter sync status on Home

## Also in 2.1.8
- Swipe a transaction right to edit, left to delete (with Undo)
- Pull down to sync
- Insights charts that draw themselves

## Features
- **Finance:** accounts, transactions, bills and debts, savings goals
- **Work:** projects, tasks, clients and payments
- **Calendar:** colour-coded workload and bills due
- **Insights:** budgets, spending, month comparison and a 30-day cash forecast
- **Private by default:** works offline and stays on this device unless you turn on Cloud sync in Settings

## Files
| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `sw.js` | Offline cache and reminders |
| `manifest.webmanifest`, `icon-*.png`, `intro.jpg` | Install and branding assets |

## Releasing
1. Change `APP_VER` in `index.html`.
2. Change the cache name in `sw.js` (`kiravault-x.y.z`).
3. Add a block at the top of `CHANGELOG.md`.

Developed by Kirabo Isa Bilal.
