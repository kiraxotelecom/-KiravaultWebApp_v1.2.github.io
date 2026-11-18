# KiraVault Changelog

Newest version first. Bump `APP_VER` in `index.html` and the cache name in `sw.js` together on every release, then add a block here.

## 2.2.0 · 19 Nov 2026

### New
- **Why this number?** Tap **Safe to spend** (Home card or Finance) to see the sum: money you have, minus bills, debts, savings commitments and goal reserves, with the list of items being set aside. If commitments exceed your money it says by how much.
- **Undo for edits.** Any Edit dialog (transaction, bill/debt, goal, project) now shows the same Undo bar as delete. The bar has a shrinking line so you can see the 8 seconds running out. Saving with no change shows nothing.
- **Safe-to-spend alerts.**
  - While adding a transaction or SMS, a hint appears if the amount is more than Safe to spend.
  - After saving any new expense that pushes you under zero, a notice appears with a **Why?** button. Paying a bill does not trigger it.
  - Needs attention lists a bill that is due today or overdue when your accounts (or its pay-from account) cannot cover it.
- **Same as last time.** Quick add shows chips for expenses you repeat (two or more times in 90 days, e.g. Fuel, Lunch). One tap logs it with the same amount, account, category and charge, with Undo. If the account is short it opens the Add form instead.
- **Share an SMS to KiraVault (Android).** After the installed app updates, KiraVault appears in the Share menu. A shared Mobile Money SMS opens Add from SMS; other text opens Quick add. It waits for the PIN lock and the welcome screen.
- **One-tap file backup.** The Home reminder and the Settings **Back up now** button now save the backup file straight to Downloads and confirm it. Share backup and Save as file remain in Settings.

### Improved
- The Install card is one line with **Install** (or **How**) and an ✕ that dismisses it for good.
- The toast no longer hides a newer message early.

## 2.1.10 · 19 Nov 2026

### New
- **Charts replay at sensible moments** (instead of only once):
  - when you **scroll** a chart into view (charts below the fold used to animate where you couldn't see them);
  - when you **come back** to a screen or reopen the app after being away for 30 seconds or more (shorter trips stay still);
  - after a successful **pull-down sync**.
  Charts with the same data you just looked at never replay on a plain redraw.
- **Repeat every 10 s (optional).** A new switch in Settings, under Animations, replays the charts currently on screen every 10 seconds. It is **off by default**. It pauses while a popup is open, while you are typing, during swipe or pull gestures, and when the app is in the background or locked. It stops after 5 repeats until you touch the screen again. It only shows while Animations is on.

### Fixed
- Bar charts no longer alter their own markup while animating, so they can be recognised as "already seen".

## 2.1.9 · 19 Nov 2026

### New
- **Animations switch.** Settings now has an **Animations** on/off switch. Off turns off every animation in the app: charts, count-ups, screen transitions, swipe motion and celebrations. The pull-to-sync spinner still spins so you can see it working. It is saved with your settings and backups. The device's "reduce motion" setting still applies on its own.
- **Donut sweeps in.** The My accounts donut draws its slices round clockwise, one after another.
- **Finance overview charts animate.** The Total available line draws in, the Daily allowance bars grow up from the baseline, and the Spending pace line draws in. Like the Insights charts, they play on first appearance or when their data changes.

### Improved
- **Quieter sync status on Home.** After signing in, the large "Synced" card is now one small muted line with a status dot (green synced, amber waiting, pulsing blue syncing). Tap it to open Cloud sync settings. The "Sync across devices" prompt for signed-out users is unchanged.

## 2.1.8 · 19 Nov 2026

### New
- **Swipe a transaction.** In Transactions, swipe a row right to **Edit** or left to **Delete**.
  - The row follows your finger and a coloured layer appears behind it (grey, then blue or red once you pass the commit point).
  - A short swipe springs back and does nothing. Only a full swipe commits.
  - Delete slides the row out and shows the normal **Undo** bar (8 seconds). Undo restores the row in its original place.
  - A light haptic fires when you cross the commit point (where the device supports it).
  - A one-time tip explains the gesture on touch devices.
- **Pull down to sync.** Pull down from the top of any screen. The indicator stretches with increasing resistance, spins while syncing, then confirms **Synced just now**. If Cloud sync is off or fails, it says so instead of failing silently.
- **Charts draw themselves in Insights.** Lines draw left to right, area fills fade in, end dots pop in. Forecast and spending-pace charts reveal left to right. Charts play when they first appear or when their data changes, not on every redraw.

### Improved
- Insights summary figures (Income, Expenses, Net) now count up like the Home cards.
- Native browser pull-to-refresh is disabled so it cannot fight the new gesture.
- All new motion is switched off when the device has "reduce motion" turned on.

### Notes
- Tapping a row still opens the Edit / Receipt / Delete menu, so nothing depends on swiping.
- Swipe and pull-to-sync work with finger, pen and mouse.
- Earlier versions are not documented here. Add them below as they are written up.
