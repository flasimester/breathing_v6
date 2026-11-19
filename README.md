# Altitude Breath

An 8-week breathwork program for summiting 4000 m+ mountains, built as a single installable web app. English and Hungarian (EN / HU switch in the header).

## What's inside
- **Today**: set a start date and see this week, today's sessions, a next-session button and a weekly progress bar. The plan adapts without "failing": repeat a week, start from any week, shift the schedule later, or make sessions lighter / longer (about ∓25%), with undo.
- **Wk 1-2 / 3-5 / 6-8**: the full program. Every exercise has an **i** explanation (what it works, why do it) and a guided timer: breath pacers, a CO₂ tolerance table with shrinking rests and tap-to-end holds, an optional Wim Hof session, countdowns and a stopwatch.
- **Summit**: quick mountain tools (calm breathing, step-rhythm cue, pursed-lip cue, recovery reset, descent breathing), a "Symptoms mean descend" reminder, and a **Before you go** section: acclimatization basics, planning and summit-morning tips, and a saved pre-trip checklist (based on CDC Yellow Book / Wilderness Medical Society guidance, general information only).
- **Progress**: a calm practice history (no scores), recent breath holds, an optional baseline / retest, backup export and import, and a calendar (.ics) of your schedule.
- **Safety**: read this first.

## Sound that survives a locked screen
Fixed-length sessions and the looping summit cues are rendered into an audio track, so the cues keep playing with the screen locked on most phones (lock-screen controls included). Sessions with open-ended holds (CO₂ table, Wim Hof) and sessions over 90 minutes use live cues and need the screen on.

## Privacy
Everything stays on your device in the browser's local storage. No account, no analytics, no external requests, no fonts loaded from the internet. Use **Progress → Export backup** to move your data to another phone.

## Run it
Open `index.html`, or visit the GitHub Pages site.

## Deploy on GitHub Pages
1. Push these files to the root of a repo.
2. **Settings → Pages → Build and deployment → Deploy from a branch**, choose `main` and `/ (root)`.
3. After a minute the site is live at `https://<user>.github.io/<repo>/`.
4. Fix the link-preview tags (they need an absolute URL). From the repo root:
   ```
   sed -i 's#https://YOUR-USERNAME.github.io/YOUR-REPO#https://<user>.github.io/<repo>#g' index.html
   ```
5. Optional: **Settings → General → Social preview → Upload** `social-preview.png`.
6. Put your name in `LICENSE`.

## Install on your phone
- **iPhone:** open the site in Safari, Share, Add to Home Screen.
- **Android:** open in Chrome, menu, Install app.

## Safety
Breathwork supports acclimatization; it does not replace it. Never hold your breath in water or while driving, do breath-holds lying down or sitting on the floor away from hard objects, and check with a doctor first if you have heart or lung issues. Symptoms mean descend.

## Notes for contributors
No build step and no dependencies. Content and translations live in `index.html` (`PH`, `HUPH`, `INFO`, `INFO_HU`, `UI`). If you change the app, bump `CACHE` in `sw.js`.
