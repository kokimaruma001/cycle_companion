# Cycle Companion — README

An interactive 28-day cycle tracker. Tap any day on the ring to see that
phase's mood, a short playful description, and a partner do's/don'ts list.

## How to use it

1. Open `cycle-tracker.html` (double-click it, or drag it into a browser).
2. Enter the **first day of your last period** in the date field and hit
   **Save**. The wheel will jump to today's actual cycle day and mark it
   with a small dot outside the ring.
3. Tap any of the 28 day segments to preview that phase's card — this
   doesn't change your tracked "today," it's just for browsing.
4. Close the tab any time. Your start date and the last day you tapped are
   both remembered, so it picks up where you left off next time you open it.

## The four phases (standard 28-day model)

| Phase | Days | Vibe |
|---|---|---|
| Menstrual | 1–5 | Bear Cave Mode |
| Follicular | 6–13 | Main Character Rising |
| Ovulation | 14–16 | Peak Glow |
| Luteal | 17–28 | The Feral Countdown |

## Automatic cycle rollover

The tracker doesn't just wrap the day count — it actually **advances the
saved start date** once a full 28-day cycle has passed. So if you entered
your start date two cycles ago and never touched the app since, the next
time you open it, it detects the gap and quietly rolls the stored start
date forward by however many whole 28-day cycles have elapsed, then
recalculates "today" from that new, current-cycle start date. You'll
always see the correct day-in-cycle without needing to re-enter anything
— until your real period starts on a different day than the model
predicts, at which point you should just enter the new date and hit
**Save** again to re-sync.

## Where your data lives

- Your start date and selected day are saved to this artifact's private
  storage (`window.storage`, personal — not shared with anyone else).
- Nothing is sent anywhere else; it only persists across sessions on this
  device/account inside Claude.

## A note on accuracy

This uses a fixed 28-day model as a general reference point. Real cycles
commonly range anywhere from about 21 to 35 days, and can vary
month-to-month for all kinds of normal reasons. Treat the day numbers and
phase boundaries as a rough guide — not a diagnosis, not birth control,
and not a substitute for tracking your actual symptoms or talking to a
doctor if something feels off.
