# KiraVault Changelog

Newest version first. Bump `APP_VER` in `index.html` and the cache name in `sw.js` together on every release, then add a block here.

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
