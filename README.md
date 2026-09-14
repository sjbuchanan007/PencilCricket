# Pencil Cricket

A two-dice, pass-and-play cricket game for the browser. No installation, no
build step — it's a single self-contained HTML file.

## Play it

Open `index.html` in any browser, or serve the folder locally:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Rules

The batting side rolls the **Batting Die**: 1, 2, 3, 4, 6, or **OWZTHAT**.

- A number is runs scored off that ball — play carries straight on. A 4 is a
  Boundary (FOUR); a 6 is a Maximum (SIX).
- **OWZTHAT** is an appeal. The bowling side rolls the **Bowling Die** to
  answer it: Bowled, Stumped, Caught, Not Out, No Ball, or L.B.W.
  - **Not Out** — the appeal fails, no runs, batting continues.
  - **No Ball** — the appeal fails and the batting side gets 1 run.
  - Anything else (Bowled, Stumped, Caught, L.B.W.) is a wicket.
- An innings ends when the wicket limit falls (10, by default). Each side
  bats one innings; the higher score wins. Equal scores is a Tie.
- There's no built-in over limit — the "Limit overs" format at setup adds
  one as an optional house rule for a fixed-length match instead of playing
  to all out.

Rules adapted from *Owzthat*, the dice cricket game invented by Lindop's in
1924 and patented in 1932.

## Notes

The game keeps the in-progress match in the browser's `localStorage` so a
match can be resumed after an accidental refresh (per-device only — it isn't
shared or synced anywhere).
