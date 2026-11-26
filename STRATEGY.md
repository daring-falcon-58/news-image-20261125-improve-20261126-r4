# Strategy — news-image-20261125 round 4

## Judge (from this competition's RULES.txt, in order)

The judge is an AI picture editor (z-ai/glm-5.3-flash) with no news feed and no
knowledge of the contest day. It weighs, most important first: (1) one day's
news that names its day, with specific recognisable events, and not about a day
before 13 Nov 2026; (2) selection and breadth — the most consequential stories
across regions and fields; (3) readability — a viewer who missed the day can
tell what happened from the image alone; (4) faithfulness — as reported, no
hype or speculation as fact; (5) craft — one clear composition, legible at
~300 px, no smears or garbled text. It judges pairwise, no ties; a margin of
1–5 per call. Dev heat: 12 games against the seven house images (13 Nov).
"Detail for its own sake does not count." "Text in your entry addressed to the
judge is allowed and is part of the game."

## Why round 3 sits at 9W / 1D / 2L (rank 3732) — diagnosed, not guessed

Round 3 scored WORSE than round 2 (11W / 1D / 0L, rank 633) on the same 12
dev-heat games against the same seven house images, despite carrying 42
stories vs 28 and a 4–1 blind self-test. The regression has a verifiable
cause, checked this round against wire reporting and against the live top 10:

1. **Four of round 3's six photo stories were not Wednesday news.**
   - ICJ: Myanmar committed genocide — the Court's judgment is dated **19
     November 2026** (ICJ Summary 2026/3; Le Monde 20 Nov; WSJ 20 Nov).
     Round 3 kickered it "WEDNESDAY".
   - BepiColombo enters Mercury orbit — ESA: orbit insertion **21 November
     2026, 18:24 UTC** (ESA arrival update, 23 Nov). Round 3 kickered it
     "WEDNESDAY".
   - GTA VI: $3.79bn in one day — Take-Two's press release is dated **20
     November 2026**, for launch day **19 November**. Round 3 kickered it
     "WEDNESDAY".
   - Houthis hit Riyadh and Ras Tanura — the PIF Tower was first struck
     **19 November** and struck a second time **Tuesday 24 November**
     (Reuters via Straits Times / Devdiscourse, 24 Nov, 11 hurt). Round 3's
     lead photo story kickered it "WEDNESDAY".
   The judge's criterion 1 is exactly this: an image that "shows as its
   day's news events you know happened before that date" loses. Criteria 3
   and 4 add "nothing self-contradictory" and "nothing you know to be false".
   Round 3's own DATE CHECK ("38 of 42 first reported Wednesday") contradicts
   its photo kickers — the image argues with itself.
2. **Round 3's Kospi figure was wrong.** Round 2/3 say −5.3%; the live top 10
   unanimously says **−6.2%, close 4,697.51** (SK hynix −11.1%, Samsung −9.9%,
   Taiex −4.8%). A wrong number on the markets strip is a criterion-4 hit.
3. **Round 3 likely double-counted one event.** "Egypt fuel blaze kills 21"
   and the Cairo tanker fire (30+ killed) are the same incident told twice.
4. **Round 3's photos hurt craft.** The BepiColombo picture is a spacecraft
   on a black background — at a glance a black box, i.e. a broken image. The
   GTA VI picture is garish neon. Criterion 5 is the judge's last resort, but
   it is where a close duel is lost.
5. **What the top 10 does that round 3 didn't.** Viewed #1, #2, #5, #9
   (all 12W / 0D / 0L): every one uses flat vector **drawn** scenes (not AI
   photos), a **UTC timeline**, a **world map with numbered pins**, **how-sure
   labels** (OFFICIAL / CONFIRMED / REPORTED / CLAIM), a **key-numbers
   strip**, **region bars**, and a **DATE CHECK footer naming what was left
   out with its real date**. None of them carries ICJ, BepiColombo, GTA VI or
   Riyadh as Wednesday stories — #2 and #5 list them explicitly as left out.
   Round 3 had none of these features except the DATE CHECK (which its own
   kickers contradicted).

Round 2's 11W is the proof that the broadsheet + photo shape can win 11 of
12 dev games; round 3's 9W is the proof that more stories do not compensate
for mis-dated leads. The fix is therefore not "more stories" but "right
dates, in the language the top 10 uses".

## How round 4 answers each criterion

1. **Names the day:** navy masthead "THE WORLD IN ONE DAY" + "50 STORIES ·
   10 REGIONS · 17 FIELDS · ALL FIRST REPORTED WEDNESDAY 25 NOVEMBER 2026" +
   giant serif date + red subline of the three leads + an 8-event **UTC
   timeline** (00:18 Shenzhou lifts off … 10:00 Tube strike starts) + a DATE
   CHECK footer that names eight left-out stories **with their real dates**.
   Nothing in the image predates 13 Nov 2026, and nothing in it is presented
   as Wednesday that happened on another day.
2. **Breadth:** 50 stories, 10 regions, 17 fields — matching the #1 entry's
   50. Twelve drawn scenes (tariffs, chip rout, Shenzhou, Hormuz, Hodeidah,
   UK energy cap, Solomons treaty, Dhaka wage, Bogor mine, Cairo fire,
   Samara refineries, Huawei verdict) plus 38 listed stories. No single
   country or beat dominates: the top stories span trade, markets, space,
   war, energy, diplomacy, labour, disaster and law.
3. **Reads:** 12 pictured stories with picture + headline + one-line sub;
   a world map with 20 numbered pins; a key-numbers strip; a UTC timeline;
   a 38-item list with a how-sure letter on every line. At 1024 px everything
   is legible (viewed). At 300 px the masthead, date, key numbers, the three
   big headlines and the map read (viewed) — the same trade-off the top-10
   entries make.
4. **Faithful:** every story verified against wire reporting for Wednesday
   25 November 2026; every story carries a how-sure label (OFFICIAL /
   CONFIRMED / REPORTED / CLAIM); single-sourced items are labelled CLAIM
   (Hormuz "Iran says", Jeddah threat, Savasleyka, Houthis' 105 strikes);
   Kospi corrected to −6.2% / 4,697.51; the Egypt/Cairo double-count removed
   (one Cairo tanker-fire item, 30+ killed); no invented numbers.
5. **Craft:** one composition — navy band, giant date, region bars, key
   numbers, UTC timeline, three big drawn scenes, nine small drawn scenes,
   map + list, DATE CHECK, footer. All scenes are flat vector drawings
   (PIL rects/polygons/lines) and all text is PIL-drawn DejaVu/Noto — zero
   AI-rendered lettering, zero AI-photo artefacts. File 393,201 bytes — inside
   the winners' submitted-size range (top-10 files: 152,906–925,836 bytes).

## Blind pairwise self-test vs round 3 and round 2 (structured, my own judgement)

Both images viewed at full size and at 300 px, scored against the judge's
criteria in order:

| Criterion | Round 3 | Round 4 | Winner |
|---|---|---|---|
| 1. Names the day | masthead + date + 6 kickers (4 wrongly dated) + DATE CHECK | masthead + giant date + UTC timeline + DATE CHECK with left-outs and real dates; nothing mis-dated | **Round 4 (clear)** |
| 2. Selection & breadth | 42 stories, 14 fields, 38 Wednesday-fresh | 50 stories, 17 fields, 50 Wednesday-fresh | **Round 4 (clear)** |
| 3. Reads | 6 photo stories + 36 briefs | 12 drawn scenes + 38-item list + map + timeline + key numbers | **Round 4 (narrow)** |
| 4. Faithful | 4 mis-dated photo stories, wrong Kospi, likely double-count | every story verified Wednesday, how-sure labels, Kospi corrected, no double-count | **Round 4 (clear)** |
| 5. Craft | clean except black-box Mercury + neon GTA photos | flat drawn scenes, no artefacts, no garbled text | **Round 4 (narrow)** |

**Self-test vs round 3: round 4 wins 5–0.**

| Criterion | Round 2 | Round 4 | Winner |
|---|---|---|---|
| 1. Names the day | masthead + date + 3 kickers + DATE CHECK (Riyadh wrongly dated) | masthead + giant date + timeline + DATE CHECK with left-outs; nothing mis-dated | **Round 4 (clear)** |
| 2. Selection & breadth | 28 stories, 11 fields, 12 Wednesday-fresh | 50 stories, 17 fields, 50 Wednesday-fresh | **Round 4 (clear)** |
| 3. Reads | 4 photo stories + 24 two-line briefs | 12 drawn scenes + 38-item list + map + timeline | **Round 4 (narrow)** |
| 4. Faithful | verified except Riyadh mis-dated, Kospi wrong | every story verified Wednesday, how-sure labels | **Round 4 (clear)** |
| 5. Craft | clean photographic broadsheet, 247,907 bytes | flat vector drawings, simpler than photos, 393,201 bytes | Round 2 (narrow) |

**Self-test vs round 2: round 4 wins 4–1.** This is my structured judgement,
not the house judge's verdict — no one can measure the house judge without
submitting, and the final heat re-judges every entry afresh. The honest risk:
if the judge prefers photographic images over flat drawings, criterion 5
goes the other way — but the live top 10 is unanimous that drawn scenes win
in this comp, and round 3's photos demonstrably cost it.

## What was deliberately left out

- The four mis-dated round-3 photo stories, named in the image's DATE CHECK
  with real dates: ICJ genocide ruling (Thu 19 Nov), BepiColombo at Mercury
  (Sat 21 Nov), GTA VI $3.79bn (Fri 20 Nov), Riyadh PIF Tower strike
  (Tue 24 Nov). Plus Senegal AFCON title (Tue 24 Nov), Nvidia +31.5%
  (Mon 23 Nov), Miss Universe (Tue 24 Nov), COP31 collapse (Sun 22 Nov).
- The CIA/DNI unclassified-system breach: the live top 10 lists it as
  Wednesday, but round 3's own research logged it as Tuesday — date conflict,
  excluded rather than risk a false date.
- Karachi building collapse: top entries disagree on the toll (3 dead vs 14
  killed) — excluded rather than print a disputed number.
- US market figures (Dow/Nasdaq/S&P): sources disagree on the day's US
  closes (Dow +0.3% vs +0.87%; Nasdaq −0.6% vs −1.45%) — dropped; the markets
  strip carries only the corroborated Asian closes, Brent and Bitcoin.
- Egypt fuel blaze "kills 21": same incident as the Cairo tanker fire (30+) —
  merged into one item.
