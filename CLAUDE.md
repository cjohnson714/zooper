# Crochet Master Plan — project brief

`crochet-master-plan.html` is a single-file app (no build step) published as a claude.ai artifact:
https://claude.ai/artifact/XoNkeg5R9bsqSy4GCu6Wk4. Republish it after every change, keeping its
capabilities (`db`, `user`, `downloads`, `sample`).

## The learner's goals (decided October 2026)

- **Main focus: amigurumi and toys.** Become an excellent toymaker first.
- **Then the fundamentals**, enough to be on the road to master crocheter (CGOA Fundamentals review).
- **Dream project:** a very intricate blanket that looks great (the Sophie's Universe ladder).
- **Everything else is optional** — colorwork, Tunisian, lace, garments, heritage techniques,
  garment design, the CGOA Advanced exam. Present these like honors/elective courses: available
  and complete, but clearly labeled optional and kept out of the required path.
- **Sustainability over speed.** Enjoy the hobby, avoid burnout, but keep a structured, logical
  direction. No guilt mechanics (streak pressure, "you're behind" copy). A lighter week is progress.
- Prefers more information to less, as long as the main toy path isn't cluttered with
  information that isn't relevant to it.

## Structure (rebuilt October 2026 as "The Amigurumi Major")

- A four-year toymaking major, about 944 required hours (3 to 4 years at 4 to 6 h a week). Courses live in
  `courses/*.json` (source of truth for content); `research/LIBRARY.json` is the verified resource library.
- Year 1 TOY 100, 101, 120, 190 · Year 2 TOY 150, 210, 220, 230, 290 · Year 3 TOY 310, 320, 330 · Year 4 TOY 410, 420, 490.
- Required minor: Fundamentals FND 110, 210, 290 (CGOA Fundamentals review). Required studio: BLK 250 (heirloom blanket).
- Optional: TOY 340, BUS 380, TCH 395, and electives LAC 330, CLR 310, TUN 320, GAR 410, HER 420, DES 430, MST 499.
- Unit ids keep their original curriculum numbers where a unit existed (1.1, 3.1 ...); new units are Tnnn.x and B1..B11.
  Never renumber: saved progress is keyed by unit id.
- Rebuild the page from `courses/` with a build script (the pipeline lived in the session scratchpad: it reads the
  courses and LIBRARY.json, swaps them into `crochet-master-plan.html`, and applies the design system).
- Design: Young Serif display, Atkinson Hyperlegible Next body, Maple Mono for counts and pattern notation.
  The home screen draws progress as a crochet magic ring (one round per year, one stitch per required unit).

## What the learner already has

- Units 0, 1.0, 1.1, 1.5, 1.6, 1.7 were covered with their first toys (Felix, Mort, Pierre).
- Hooks: Clover Amour 2.75 and 3.5 mm, Tulip Etimo Rose 3.5 mm, two Woobles 4 mm.
- Main yarn: Lion Brand 24/7 Cotton (186 yd per 100 g skein); DK for Pica Pau book 1.
- Owns pins, Poly-Fil, safety eyes, markers, bent-tip needles, scissors, pom-pom makers.
- Stores: Michaels (Sugarcreek Plaza), The Yarn Remedy (Greenville), Walmart; online WeCrochet,
  Hobbii, LoveCrafts.

## Open ideas, not yet built

- Skill tags on every project so the app can suggest the next toy that adds one new skill.
- Pattern companion: parse a pattern into rounds and check stitch counts against the counter.
- Yarn stash with yardage, subtracted from the shopping list.
- Per-project time tracking to replace the "half your time on the path" forecast assumption.

## Working rules

- Verify outside facts (prices, programs, patterns) before adding them; date anything that goes stale.
- Test in a headless browser at phone width, light and dark, before publishing.

## Known limits of the October 2026 research

- WebFetch was blocked, so facts come from search snippets. Items marked verified were confirmed by a second
  agent's search; none were opened as pages. Re-check prices and links in a normal browser before relying on them.
- r/Amigurumi and r/CrochetHelp wikis could not be read; check them for a beginner page worth crediting.
- Open questions: whether Edward's Menagerie: The New Collection uses US or UK terms; the Sophie's Universe book's
  part and round counts; 2026 prices of The Essential Guide to Amigurumi and Hooked by Kati courses.
- Hour estimates for toys are guesses until the learner logs real project times.
