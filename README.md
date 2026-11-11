# Gridlure content

Content published to the Gridlure app through this repo's GitHub Pages site:

- `days.json`: themed daily puzzles.
- `collections.json`: monthly collections (Classics is built into the app).

The app checks GitHub first and keeps a matching copy built in as a fallback.

Rules for days:

- Publish a day at least a day before it releases (6:00 AM Pacific). Until then it
  can be added, changed, or removed. After that it's frozen on every phone that has it.
- A phone that never had a released day (a new install) still picks it up, as long as
  nobody has played that date on it, so keep past days in the file.

Rules for everything:

- Every picture must be solvable by logic alone and have a caption. The app checks
  and skips anything that isn't, or that's malformed.
- A broken file is ignored entirely, so a typo can't wipe anything out.
- A collection's `id` is permanent (progress is saved under it). Monthly ones are
  `YYYY-MM`, and `"plus": true` puts them behind Gridlure Plus.

Format: pictures are the same as in `ThemedDays.json` in the app. See
`docs/DailySystemPlan.md` and `MONETIZATION.md` in the app repo.
