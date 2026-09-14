# Pencil Cricket

A two-dice, pass-and-play version of the classic paper-and-pencil cricket game.
No installation, no build step — it's a single self-contained HTML file.

## Play it

Open `index.html` in any browser, or serve the folder locally:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Rules

Every ball, both dice are rolled.

- **Matching numbers** (a double) is a wicket. The dismissal depends on the
  number rolled: 1 = Caught, 2 = Stumped, 3 = Run Out, 4 = LBW,
  5 = Caught & Bowled, 6 = Bowled.
- **Different numbers** score runs equal to the sum of the two dice (3–11).
  A sum of 9 or 10 is a Boundary (FOUR); 11, the highest possible, is a
  Maximum (SIX).
- Six balls make an over.
- The team batting first sets a target. The second team wins by reaching it
  before running out of overs or wickets; otherwise the higher score wins.
  Equal scores is a Tie.

Overs per innings and wickets per innings are configurable at match setup.

## Notes

The game keeps the in-progress match in the browser's `localStorage` so a
match can be resumed after an accidental refresh (per-device only — it isn't
shared or synced anywhere).
