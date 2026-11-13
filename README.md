# Gridlure content

Content published to the Gridlure app through this repo's GitHub Pages site:

- `days2.json`: the daily puzzles, a 10×10 and a 15×15 for each date (format 2).
  Build 4 and later read this one.
- `days.json`: the old format (a 5×5 and a 10×10), kept only for TestFlight builds
  1–3. Leave it in place, and don't add new days to it.
- `collections.json`: the Plus collections (Classics is built into the app).
- `privacy.html`: the privacy policy, linked from App Store Connect.

Election Week (Nov 6) only has a 15×15 in `days2.json`: its 10×10 is built into the
app and can't be replaced.

The app checks GitHub first and keeps a matching copy built in as a fallback.

Rules for days:

- Publish a day at least a day before it releases (6:00 AM Pacific). Until then it
  can be added, changed, or removed.
- After release, a date is frozen on every phone that has played it. Phones that
  haven't played it (new installs, or anyone who skipped that day) follow the file, so
  a fixed archive puzzle reaches them. Keep past days in the file, and avoid changing
  them after launch: friends comparing an archive day would see different puzzles.

Rules for everything:

- Every picture must be solvable by logic alone and have a caption. The app checks
  and skips anything that isn't, or that's malformed.
- Pictures are square: 5×5, 10×10, 15×15, or 20×20. Dailies are 10 and 15 only;
  collections may use any of the four. Other sizes are skipped.
- A broken file is ignored entirely, so a typo can't wipe anything out.
- A collection's `id` is permanent (progress is saved under it). Dated ones are
  `YYYY-MM`, and `"plus": true` puts them behind Gridlure Plus.

Format: pictures are the same as in `ThemedDays.json` in the app. See
`docs/DailySystemPlan.md` and `MONETIZATION.md` in the app repo.
