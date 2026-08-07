# Personal Jeopardy! Training System

This is a structured, day-by-day training system for an experienced trivia competitor preparing to compete on Jeopardy!. It assumes strong general knowledge and active quiz league participation, and focuses on the Jeopardy!-specific skills that the show's format demands: buzzer timing, wagering math, format adaptation, and stage performance. The system is designed around real-life constraints — a full-time job, parenting obligations, and ongoing trivia league commitments — and caps at 90 minutes per day at peak. Every drill referenced here is fully specified in the companion drill files (`drills/buzzer-drills.md`, `drills/knowledge-drills.md`, `drills/wagering-drills.md`); every tool is annotated in `resources.md`; progress is tracked in `progress-tracker.md`.

---

## Weekly Cadence

The schedule assumes training availability alternates on a roughly week-on/week-off pattern — for example, due to alternating work travel, on-call weeks, or other recurring schedule constraints — with work running standard weekday hours. Training volume flexes around high- and low-availability weeks.

### High-Availability Week (Higher Volume)

| Day | Available Time | Session Type |
|-----|---------------|--------------|
| Monday | 60 min (evening) | Knowledge gap work + buzzer drill |
| Tuesday | 30 min (evening) | Wagering drill |
| Wednesday | 60 min (evening) | Full-game simulation |
| Thursday | 30 min (evening) | Buzzer drill (light-reaction or voice-anticipation) |
| Friday | Off | Rest / passive intake (read a chapter, watch a documentary) |
| Saturday | 90 min (morning) | Long block: full-game sim + category deep-dive |
| Sunday | 30 min (flexible) | Wagering scenarios + weekly review |

**Weekly total:** ~5 hours active training + passive intake.

### Low-Availability Week (Lower Volume)

| Day | Available Time | Session Type |
|-----|---------------|--------------|
| Monday | 15 min (after bedtime) | Buzzer drill only (Drill 1 or 3 — mechanical, low cognitive load) |
| Tuesday | Off | — |
| Wednesday | 30 min (after bedtime) | One J-Archive game, Coryat scored |
| Thursday | Off | — |
| Friday | Off | — |
| Saturday | 30 min (morning) | Wagering drill or Pavlov flashcards |
| Sunday | 15 min (flexible) | Weekly review only — log metrics, update tracker |

**Weekly total:** ~1.5 hours active training. Low-availability weeks prioritize maintaining buzzer muscle memory and not losing momentum rather than building new skill.

### Trivia League Nights

League games are not "off nights" — they are the real-world cross-validation signal (see [Real-World Transfer](#real-world-transfer) below). On league nights, replace the scheduled session with league play and log results in `progress-tracker.md`. If the league game is short, add 15 minutes of buzzer work afterward while recall is still primed.

---

## Session Structure

### The 30-Minute Session

A 30-minute block is the minimum useful training unit. Structure it as a single focused drill:

1. **Setup** (2 min): Stand up. Get your buzzer device. Open the relevant tool (Buzzer App, J-Archive, wagering worksheet). Set a timer.
2. **Warm-up** (3 min): 10–15 rapid buzzer clicks to activate muscle memory, even if the session is knowledge- or wagering-focused.
3. **Main drill** (20 min): One drill protocol from the drill files. Examples:
   - Buzzer: Drill 1 (Light-Reaction) — 50 buzzes at current delay setting.
   - Knowledge: Play one J-Archive game, Coryat scored, with category tagging.
   - Wagering: Work through 5 Final Jeopardy scenarios from `drills/wagering-drills.md`.
4. **Log** (5 min): Record metrics in `progress-tracker.md`. Note anything surprising — a category that was unexpectedly weak, a reaction-time spike, a wagering scenario that felt confusing.

### The 60-Minute Session

A 60-minute block allows combining two complementary drills:

1. **Setup + warm-up** (5 min): Same as above.
2. **Primary drill** (25 min): The session's main focus — typically a full J-Archive game or an extended buzzer protocol.
3. **Secondary drill** (20 min): A complementary skill. Pair knowledge work with buzzer work (different neural demands — the switch itself is useful recovery). Do not pair two high-cognitive-load drills (e.g., wagering math + category deep-dive).
4. **Cool-down and log** (10 min): Record metrics. Review the session's category breakdown. Flag any category that appeared 3+ times and was answered incorrectly — this feeds the knowledge gap identification process in `drills/knowledge-drills.md`.

**Recommended pairings:**

| Primary (25 min) | Secondary (20 min) | Why |
|---|---|---|
| J-Archive full game (Coryat) | Buzzer Drill 1 (Light-Reaction) | Knowledge recall followed by mechanical timing — different systems, good recovery |
| Category deep-dive (flashcards) | Buzzer Drill 2 (Voice-Anticipation) | Content acquisition + timing practice on recorded episodes |
| Wagering scenarios | Buzzer Drill 3 (Rapid-Click Endurance) | Math-heavy work + physical/mechanical work |

### The 90-Minute Block (Peak Only)

The maximum daily session. Used on high-availability Saturdays and during pre-audition/taping intensives. Structure:

1. **Setup + warm-up** (5 min)
2. **Full-game simulation** (35 min): Buzzer Drill 4 from `drills/buzzer-drills.md` — play a complete J-Archive game with buzzer, Coryat scoring, LBR tracking, and lockout tracking.
3. **Break** (5 min): Stand up, hydrate. Do not review scores yet.
4. **Category deep-dive** (25 min): Based on the weakest category from the game just played (or from the running weak-category list in `progress-tracker.md`). Use the gap-closing protocols in `drills/knowledge-drills.md`.
5. **Wagering block** (15 min): 3 Final Jeopardy scenarios from `drills/wagering-drills.md`, worked through completely with written math.
6. **Review and log** (5 min): Record all metrics. Update weak-category list. Compare today's Coryat to the running average.

---

## Ramp Plan

### Weeks 1–2: Baseline

**Goal:** Establish starting metrics across all skill areas. No improvement targets yet — just measurement.

**Activities:**
- Play 3–4 J-Archive games with Coryat scoring to establish a knowledge baseline. Tag categories and log in `progress-tracker.md`. Compare to the benchmark ranges in `prep-strategies-research.md`: ~$24,000 Coryat suggests a decent chance of passing the online test; ~$28,000 suggests strong competitiveness.
- Run Buzzer Drill 1 (Light-Reaction) at 1000ms delay, 3 sessions, to establish reaction-time baseline. Typical starting median: ~230ms (per Holznagel, *Secrets of the Buzzer*, 2021).
- Work through 5 Final Jeopardy wagering scenarios from `drills/wagering-drills.md` to establish comfort level with the cover-bet formula.
- Record trivia league baseline: log the last 3+ league game results (with category-level breakdown if available) in the "Trivia league baseline" section of `progress-tracker.md`.
- Take the Jeopardy! Anytime Test if not taken in the past 12 months ([jeopardy.com/be-on-j/anytime-test](https://www.jeopardy.com/be-on-j/anytime-test)).

**Time commitment:** 30 min/session, 3–4 sessions/week. ~2 hours total per week.

**Deliverable:** A completed baseline section in `progress-tracker.md` with: Coryat average, top 3 and bottom 3 categories, buzzer RT median, wagering comfort (1–5 self-rating), and trivia league baseline scores.

### Weeks 3–6: Build

**Goal:** Systematically improve across all three skill pillars (buzzer, knowledge gaps, wagering) while maintaining trivia league performance.

**Week 3–4 focus: Buzzer + Knowledge Gaps**
- Buzzer Drill 1 progression: move to 400ms delay. Target median RT < 200ms.
- Introduce Buzzer Drill 2 (Voice-Anticipation) — 1 session/week using recorded episodes.
- Begin knowledge gap work: identify the 3 weakest categories from baseline Coryat games and run targeted study using protocols in `drills/knowledge-drills.md`.
- Continue Coryat games: 2 per week minimum.
- Study Pavlov clues: 15 min/session, 2 sessions/week (see `drills/knowledge-drills.md` and `resources.md` for Pavlov resources).

**Week 5–6 focus: Integration + Wagering**
- Buzzer Drill 1 progression: move to 130ms delay. Target median RT < 170ms.
- Introduce Buzzer Drill 3 (Rapid-Click Endurance) — 1 session/week.
- Begin Buzzer Drill 4 (Full-Game Simulation) — the integration drill that combines buzzer + knowledge. 1 session/week on the 90-minute Saturday block.
- Wagering: increase to 2 sessions/week. Move beyond the cover-bet formula to Stratton's Dilemma, trailing scenarios, and penultimate wager calculations (all in `drills/wagering-drills.md`).
- Introduce the Forrest Bounce in full-game simulations — practice selecting clues bottom-up and jumping between categories.

**Time commitment:** Ramp from ~3 hours/week (Week 3) to ~5 hours/week (Week 6) on high-availability weeks. Low-availability weeks stay at ~1.5 hours.

### Weeks 7+: Peak / Maintain

**Goal:** Maintain skill levels, continue closing knowledge gaps, and shift toward game-day readiness.

**Ongoing weekly targets (high-availability week):**
- 2 full-game simulations (Buzzer Drill 4) with Coryat + LBR + lockout tracking.
- 2 buzzer-only sessions (alternate between Drills 1, 2, and 3).
- 1 wagering session (3–5 scenarios).
- 1 category deep-dive targeting the current weakest area.
- 1 weekly review: compare this week's metrics to last week's, update `progress-tracker.md`, adjust next week's focus.

**Buzzer target:** Median RT < 150ms (Drill 1 at 0ms delay), lockout rate < 15% (Drill 2), LBR < 3 per game (Drill 4).

**Knowledge target:** Coryat trending upward, bottom-3 categories rotating (if the same categories remain weakest for 3+ weeks, escalate study intensity per `drills/knowledge-drills.md`).

**Wagering target:** Cover-bet calculation completed correctly within 15 seconds, Stratton's Dilemma scenarios resolved correctly 90%+ of the time.

**Stage readiness:** During peak phase, all full-game simulations should be done standing, in dress shoes or equivalent, under bright lighting, speaking responses aloud. This is Holzhauer's method for closing the "Couch Brain vs. Game Show Brain" gap (see `prep-strategies-research.md`).

---

## The Week Before an Audition

If you receive an audition invitation (the callback after passing the Anytime Test), shift to audition-specific prep for 5–7 days:

1. **Sharpen, don't cram.** Do not try to learn new categories. Focus on recalling what you already know faster. Run Pavlov flashcards at speed (target: answer within 3 seconds). Play 1 Coryat game per day to keep the rhythm.

2. **Mock audition practice.** The audition includes a second written test (50 clues, 8 seconds each — harder than the Anytime Test), a mock game in groups of three, and a personal interview. Practice:
   - Timed written responses: use J-Archive clues, 8 seconds per clue, pen on paper.
   - Speaking aloud: answer every practice clue in full-sentence form ("What is…" / "Who is…"). Enunciation matters — coordinators evaluate it.
   - Personal anecdote: prepare 3 interesting personal stories (30–60 seconds each) for the interview segment. The show wants entertaining TV; charisma and camera comfort are evaluated alongside knowledge.

3. **Buzzer maintenance.** Do not increase buzzer intensity — just maintain. 10-minute sessions, 3x in the final week.

4. **Logistics.** Review the audition process details in `prep-strategies-research.md` (Audition and Contestant Search section). Bring a photo ID. Dress as you would for a TV appearance — this is part of the evaluation.

**Source:** [Jon Santiago's audition guide](https://santiagos.space/how-to-get-on-jeopardy/); [BuzzerBlog.com, "So, You Got The Call"](https://www.buzzerblog.com/thecall/)

## The Week Before a Taping

If you are called from the contestant pool for a taping date (typically 2–6 weeks' notice):

1. **Peak week.** This is the week to hit maximum training volume — 90-minute blocks on every available day. Run 2 full-game simulations per day if time allows. Standing, dress shoes, bright lights, speaking aloud.

2. **Wagering automation.** The cover-bet formula and Stratton's Dilemma must be automatic — you will be doing this math on camera under time pressure with no calculator. Run 10 scenarios per day from `drills/wagering-drills.md`. Write the math by hand, not in your head.

3. **Stage simulation.** Practice stating wagers aloud in confident, clear voice. Practice the Forrest Bounce — say category names and dollar amounts aloud ("I'll take [Category] for $1,200"). Practice recovering from a wrong answer: take a breath, release it, move to the next clue.

4. **Physical preparation.** Stand for 2+ hours at a stretch to build stamina (tape days are 5 episodes over ~8 hours). Practice in the actual shoes and outfit. If traveling to Los Angeles, arrive 2+ days early to adjust to Pacific Time.

5. **Taper the final 2 days.** Reduce to 30-minute sessions. No cramming. Light Pavlov review, one easy Coryat game, gentle buzzer warm-up. Sleep is more valuable than last-minute study.

6. **Pack list:** 3+ outfit changes (winners play again after a wardrobe change), comfortable dress shoes, light snacks, water, any medication, government-issued photo ID.

**Source:** [BuzzerBlog.com](https://www.buzzerblog.com/thecall/); [TV Insider tape day accounts](https://www.tvinsider.com/1162185/jeopardy-contestants-reveal-what-the-day-of-show-is-really-like/); `prep-strategies-research.md` (Stage Performance section)

---

## Sample One-Week Schedule (High-Availability Week, Build Phase — Week 5)

This schedule uses only drills and tools defined in this training kit. It assumes no low-availability obligations and a standard work week.

| Day | Time | Activity | Drill / Tool | Duration |
|-----|------|----------|-------------|----------|
| **Monday** | 7:30 PM | J-Archive game (Coryat scored, category-tagged) | `drills/knowledge-drills.md` — Coryat scoring protocol | 25 min |
| | 7:55 PM | Buzzer Drill 1 (Light-Reaction, 130ms delay) | `drills/buzzer-drills.md` — Drill 1; The Buzzer App | 15 min |
| | 8:10 PM | Log metrics | `progress-tracker.md` | 5 min |
| **Tuesday** | 8:00 PM | Wagering drill: 5 FJ scenarios | `drills/wagering-drills.md` — FJ wagering workout | 20 min |
| | 8:20 PM | Buzzer warm-up (rapid clicks) | `drills/buzzer-drills.md` — Drill 3 (30 cycles) | 5 min |
| | 8:25 PM | Log metrics | `progress-tracker.md` | 5 min |
| **Wednesday** | 7:30 PM | Full-game simulation (Buzzer Drill 4) | `drills/buzzer-drills.md` — Drill 4; J-Archive game | 35 min |
| | 8:05 PM | Category deep-dive (weakest from today's game) | `drills/knowledge-drills.md` — gap-closing protocol | 20 min |
| | 8:25 PM | Log metrics | `progress-tracker.md` | 5 min |
| **Thursday** | 8:00 PM | Buzzer Drill 2 (Voice-Anticipation, recorded episode) | `drills/buzzer-drills.md` — Drill 2 | 25 min |
| | 8:25 PM | Log metrics | `progress-tracker.md` | 5 min |
| **Friday** | — | Rest | Passive intake: read a chapter of *Brainiac* (Jennings, 2006) or watch a documentary in a weak category | — |
| **Saturday** | 9:00 AM | 90-minute block | See [90-Minute Block structure](#the-90-minute-block-peak-only) above | 90 min |
| | | — Full-game sim (Drill 4) | `drills/buzzer-drills.md` — Drill 4 | 35 min |
| | | — Category deep-dive | `drills/knowledge-drills.md` — gap-closing protocol | 25 min |
| | | — Wagering block (3 scenarios) | `drills/wagering-drills.md` | 15 min |
| | | — Review + log | `progress-tracker.md` | 5 min |
| **Sunday** | 10:00 AM | Weekly review | Review all metrics from the week. Compare Coryat trend, RT trend, LBR trend. Update weak-category list. Plan next week's focus areas. | 30 min |

**Weekly total:** ~5 hours active training.

**Tools required for this week:** J-Archive (free), The Buzzer App (free), a clicky pen or Delcom USB button, `progress-tracker.md`, the three drill files in `drills/`. All are listed in `resources.md` with full annotations.

---

## Real-World Transfer

Not all drills in this system are Jeopardy!-specific. Some directly improve general trivia performance and should produce measurable gains in league play. The table below classifies each drill by transfer type, so `progress-tracker.md` can track the right metrics against the right signal.

### Transfer Classification

| Drill | File | Transfer Type | What It Improves | League-Visible? |
|-------|------|--------------|------------------|-----------------|
| Buzzer Drill 1 (Light-Reaction) | `drills/buzzer-drills.md` | Jeopardy!-specific | Reaction to lockout-system lights | No — league formats do not use lockout buzzers |
| Buzzer Drill 2 (Voice-Anticipation) | `drills/buzzer-drills.md` | Jeopardy!-specific | Anticipating host speech cadence | No — league questions are not read by a host with identical cadence |
| Buzzer Drill 3 (Rapid-Click Endurance) | `drills/buzzer-drills.md` | Jeopardy!-specific | Multi-click stamina for lockout system | No |
| Buzzer Drill 4 (Full-Game Simulation) | `drills/buzzer-drills.md` | **General transfer** | Recall under time pressure, decision-making on whether to attempt | **Yes** — faster, more confident recall under pressure transfers directly |
| Coryat scoring / J-Archive play | `drills/knowledge-drills.md` | **General transfer** | Breadth of knowledge, weak-category identification | **Yes** — closing knowledge gaps improves performance in any trivia format |
| Category deep-dive / gap-closing | `drills/knowledge-drills.md` | **General transfer** | Depth in weak areas | **Yes** — targeted study in weak categories |
| Pavlov clue study | `drills/knowledge-drills.md` | Mixed | ~60% of Pavlovs are general knowledge; ~40% are Jeopardy!-writer-specific patterns | **Partially** — many Pavlov answers are simply well-known facts |
| FJ wagering math | `drills/wagering-drills.md` | Jeopardy!-specific | Cover-bet calculation, game-state analysis | No — league formats do not use individual wagering |
| DD wagering strategy | `drills/wagering-drills.md` | Jeopardy!-specific | Risk-sizing under uncertainty | No |
| Stage performance / dress rehearsal | `prep-strategies-research.md` | Jeopardy!-specific | Composure under TV-studio conditions | No |

### How League Results Validate Training

Trivia league games serve as the cross-validation signal for this training system. The logic:

1. **General-transfer drills** (Coryat play, category deep-dives, full-game simulation recall) should produce improvements in league scores over time. If league results are flat or declining after 4+ weeks of training, one of these is likely true:
   - Training is not addressing the categories that appear in league play (adjust category targeting).
   - Training volume is too low on knowledge work relative to buzzer/wagering (rebalance).
   - Fatigue or burnout is degrading performance (reduce volume, add rest days).

2. **Jeopardy!-specific drills** (buzzer timing, wagering math, stage rehearsal) should have **no effect** on league scores. They are not expected to transfer. If league results improve coincidentally, attribute it to the general-transfer drills, not the specific ones.

3. **Tracking protocol:** Record every league game result in the "Trivia league ongoing results" section of `progress-tracker.md`. Compare the pre-training baseline (logged in Weeks 1–2) to rolling 4-week averages during training. A sustained upward trend in league scores, correlated with increased Coryat averages, is the strongest evidence that the knowledge-building drills are working.

*Opinion (not sourced):* For most experienced trivia competitors, the knowledge-building drills will produce the fastest league improvement, while the buzzer and wagering drills are what separate Jeopardy! preparation from general trivia preparation. Both matter, but for different reasons.

---

## Designed for Week-by-Week Iteration

This training system is designed to support a future automated loop (v2) that generates personalized weekly training plans based on the previous week's data. The structures below are the extension points.

### Inputs the v2 Loop Will Need

1. **Last week's `progress-tracker.md` data:**
   - Coryat scores (per game, with category breakdown)
   - Buzzer metrics: median RT, lockout rate, LBR count
   - Wagering drill accuracy (scenarios correct / attempted)
   - Number and type of sessions completed vs. planned

2. **Last 1–2 trivia league game results:**
   - Overall score or placement
   - Category-level breakdown (if available)
   - Any notable misses or surprising strengths

3. **Self-reported subjective ratings (weekly, 1–5 scale):**
   - Confidence (overall readiness feeling)
   - Recall speed (subjective sense of how fast answers come)
   - Buzzer feel (comfort and timing intuition)
   - Wager comfort (confidence in wagering math under pressure)
   - Stage nerves (anxiety level during simulated game conditions)

   <!-- v2: these ratings are in progress-tracker.md, "Subjective self-rating" section -->

### Outputs the v2 Loop Will Produce

1. **Next week's plan diff:** A modified version of the weekly schedule above, adjusted based on:
   - Which skill area showed the least improvement (increase volume).
   - Which skill area plateaued (change drill variant or intensity).
   - Whether it is a high-availability or low-availability week (adjust volume).
   - Whether an audition or taping is upcoming (shift to pre-event protocol).

2. **Category priority update:** A re-ranked list of weak categories based on the latest Coryat data and league results, feeding into `drills/knowledge-drills.md` gap-closing protocol.

3. **Burnout risk flag:** If session completion rate drops below 60% for 2 consecutive weeks, or if subjective ratings trend downward across 3+ dimensions, the loop should recommend a recovery week (reduced volume, no new drills, focus on enjoyable passive intake).

4. **League transfer report:** A comparison of league score trend vs. Coryat trend, testing whether general-transfer drills are producing the expected real-world improvement signal.

<!-- v2: the loop reads progress-tracker.md and this file, generates a "week N+1 plan" appended to a running log, and flags any items above for human review -->
