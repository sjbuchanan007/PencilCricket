# Roadmap

Ideas for Pencil Cricket that aren't built yet.

- [ ] **Coin toss animation** — animate the flip instead of resolving it instantly.
- [ ] **Two batters at the crease** — track a striker and non-striker instead of
      one batter alone; swap who's on strike at the end of each over, and after
      an odd-numbered score off a ball (no-ball runs don't trigger a swap).
- [ ] **Weighted scoring and dismissal odds** — move off a uniform 1-in-6 per
      die face toward probabilities closer to real cricket (e.g. singles more
      common than sixes, "Not Out" more common than "Bowled").
- [ ] **Two-dice batting variant (optional house rule)** — an alternate
      batting die pair that adds dot balls (0) and extras (byes/leg byes)
      alongside the existing no-ball, for more realistic scoring variance.
      Offer it as a format choice at setup, alongside "Classic" and "Limit
      overs", rather than replacing the single-die Owzthat default.
      Working idea: sum-of-two-dice determines the outcome (36 equally
      likely combinations across sums 2–12, e.g. sum 4 = Four, sum 6 = Six,
      with the other 9 sums covering dot balls, 1s, 2s, 3s, extras, and the
      OWZTHAT appeal). Open question, needs more thought: the sum
      distribution is a bell curve peaking at 7, so sum 6 (5/36 combos) is
      naturally more frequent than sum 4 (3/36) — backwards from real
      cricket where fours are commoner than sixes. Decide whether to keep
      the mapping as-is, swap which sum represents four vs six, or not
      worry about matching real-world frequency at all.
