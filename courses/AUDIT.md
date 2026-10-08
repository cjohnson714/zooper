# Curriculum audit

Date: 2026-10-08. Checker: `wf/audit/check.js` (run `node check.js`, add `list` to print the order). Helpers: `skills.js`, `refs.js`, `ctx.js`.

## Order used

Y1: TOY 100, TOY 101, FND 110, TOY 120, TOY 190.
Y2: TOY 150, TOY 210, TOY 220, TOY 230, FND 210, BLK 250, TOY 290.
Y3: TOY 310, 320, 330, 340 (optional), FND 290, TCH 395 (optional).
Y4: TOY 410, 420, 490, BUS 380 (optional).
Electives LAC 330, CLR 310, TUN 320, GAR 410, HER 420, DES 430, MST 499 are metadata only (no unit files; their units come from the old curriculum). That is 117 units in the flat list.

## Mechanical checks (all pass now)

- Unit ids unique across all files.
- Every `prereq_units` id exists and comes earlier in the order above. The one exception is `5.1` (TUN 320), listed by optional T395.6; it is a valid old-curriculum id.
- All 22 spec courses present, plus the 7 elective metadata files. Unit lists match SPEC.md for every course.
- `required` flags match SPEC (optional: TOY 340, BUS 380, TCH 395, all electives).
- credits = hours/45 to 0.1 in every file. Course hours equal the sum of unit hours (optional units excluded) and are within 15% of SPEC.
- Every Learn line has a left-handed option or the "mirror" sentence.
- No forbidden words (behind, late, overdue, missed, streak, failure, must), no em dashes, no emoji.
- Projects have a valid tier; every unit has a pass list and 2 to 4 `wrong` rows.

## Fixed

- FND 210 / 2.14: Learn line now says "both left-handed and right-handed versions" (the old wording read "left- and right-handed" and was not clearly an option).
- "behind" removed from five places (TOY 230 T230.1, TOY 310 T310.4, TOY 410 summary, TOY 420 T420.4 twice). Meaning kept.
- Value/grayscale method was taught three times (B4, T330.2, T410.6). T330.2 and T410.6 now point back to B4 and T330.2 as refreshers. No prerequisite added, so the toy path does not wait on the blanket studio.
- No id, prerequisite, credit or hours errors were found, so none were changed.

## Judged fine, left alone

- TCH 395 hours are 40 (Level I). T395.6 (30 h) is marked optional inside an optional course, so it is not counted.
- TOY 210 has an extra unit, T210.5 (Three characters, 7 h). SPEC allows adding units. Course hours are 25.
- UK terms: T150.3 has the 1-hour micro-lesson, and 2.9 says it builds on it. 2.9 does not list T150.3 as a prerequisite, so FND 210 can be done without it.
- Bobbles, popcorns, puffs: T220.6 (in the round) and 2.5 (flat rows) teach the same stitches. T220.6 says so and works either way round, so this is overlap by design.
- Embroidery: 3.3 uses a simple embroidered mouth with a linked tutorial before T210.2 teaches it fully. Safety, felt and crocheted eyes: T120.4 introduces, T210.4 deepens. Same sources are reused.
- Staggered increases appear in 1.7 round tables before T230.1 explains staggered vs stacked. The tables are given in full, so nothing needs to be known first.
- Cables 2.7 mention a "charted practice piece" before 2.8 teaches symbol charts. It describes the linked tutorial and the drill is written out, so it does not depend on chart reading.
- T320.1, T320.2, T320.3 reuse one bear and one bunny body pattern on purpose.

## Remains for a human

- T190.1 (the exam) repeats the oval and sphere drills of 3.4 and 3.1 closely, which suits an exam but is not a fresh test. Consider changing the dimensions.
- Hours for B9 (170 h) and the whole of BLK 250 (239 h) run across years 2 to 4; the order above puts BLK in Year 2 only for sequencing.
- FND 210 starts after TOY 150 in this order. If you want the minor to start earlier in Year 2, nothing breaks: its prerequisites are all FND 110 units and TOY 101 units.
- External facts (prices, programs, URLs) were not re-verified in this pass.
