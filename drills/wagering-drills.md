# Wagering Strategy Drills

This is a drill specification for mastering Jeopardy! wagering math — Daily Double sizing, Final Jeopardy calculations, and the strategic reasoning behind each. It is written for an experienced trivia competitor who needs to make wagering decisions automatic so that under stage pressure the math is already done. Wagering is a pure skill: it requires no trivia knowledge and can be fully learned through repetition. These drills target that skill; see `training-system.md` for how they fit into the weekly cadence, `drills/buzzer-drills.md` for timing, and `drills/knowledge-drills.md` for the knowledge layer.

---

## Why Wagering Matters

Wagering is the only dimension of Jeopardy! that is entirely under the contestant's control. You cannot guarantee you will know the answer or win the buzzer race, but you can guarantee your wager is mathematically optimal. James Holzhauer's Daily Double earnings accounted for ~$653,416 — nearly 30% of his $2.4M total winnings — from roughly 6% of the questions he answered. That leverage comes from wagering aggressively with a high accuracy rate (~95% on DDs).

Conversely, poor Final Jeopardy wagers cost contestants winnable games every week. Keith Williams (2003 College Championship winner) documented hundreds of suboptimal FJ wagers on his site The Final Wager, showing that many losses stem from arithmetic errors or failure to apply basic cover-bet logic — not from wrong answers.

**Source:** [The Action Network, "How James Holzhauer Used Sports Betting Principles"](https://www.actionnetwork.com/entertainment/james-holzhauer-jeopardy-sports-betting-expected-value-2019); [The Final Wager tutorial](https://thefinalwager.wordpress.com/tutorial/); [Wikipedia, "Strategies and Skills of Jeopardy! Champions"](https://en.wikipedia.org/wiki/Strategies_and_skills_of_Jeopardy!_champions)

---

## Part 1: Daily Double Wagering

### The Decision Framework

Daily Double wagering is a function of three variables: your score relative to opponents, the category strength, and the number of clues remaining. The minimum DD wager is $5; the maximum is your entire score (a "true Daily Double") or $1,000 in the Jeopardy! round / $2,000 in Double Jeopardy! if your score is below that threshold.

**Core rules of thumb:**

| Situation | Recommended Wager | Rationale |
|-----------|------------------|-----------|
| Leading + strong category | Aggressive: 50–100% of score | Positive expected value at high accuracy. Holzhauer went all-in on Jeopardy!-round DDs ~90% of the time. |
| Leading + weak category | Minimum ($5) | Preserve the lead. A wrong answer on a large DD wager can flip a dominant position. Alex Jacob used this approach routinely. |
| Trailing | Aggressive: often true DD | The DD is the best tool for closing a gap. You need to take risks to catch up — small wagers lock in a losing position. |
| Close game, late in DJ round | Enough to reach 2× second place | Sets up a lock or crush game going into FJ, which dramatically simplifies your FJ wager. |
| Early Jeopardy! round DD | True DD (if score is low) | With most of the game remaining, the downside of going to $0 is recoverable. The upside of doubling is a bankroll that compounds. |

**Source:** [The Action Network](https://www.actionnetwork.com/entertainment/james-holzhauer-jeopardy-sports-betting-expected-value-2019); [Wikipedia, "Strategies and Skills"](https://en.wikipedia.org/wiki/Strategies_and_skills_of_Jeopardy!_champions); [Board Control DD Calculator](https://boardcontrol.io/dd.html)

### The Expected Value Test

Before wagering, run this mental check: *If I faced this category 100 times, how often would I get it right?*

| Self-Assessed Accuracy | EV of True DD (from $10,000) | Recommendation |
|------------------------|------------------------------|----------------|
| 90%+ | +$8,000 per attempt | Bet big (50–100%) |
| 70–89% | +$4,000–$7,800 | Bet moderately (30–60%) |
| 50–69% | +$0–$3,800 | Bet small or minimum |
| Below 50% | Negative | Bet $5 |

*Example:* You have $12,000, leading by $4,000, and the DD is in "World Capitals" — a strong category for you (estimated 85% accuracy). A true DD ($12,000 wager) has EV of ($12,000 × 0.85) − ($12,000 × 0.15) = $10,200 − $1,800 = **+$8,400**. Even a wrong answer leaves you at $0 with time to recover. A $6,000 wager has EV of +$4,200 and keeps you at $6,000 minimum. Either is defensible; the game state (how far ahead, how many clues remain) tips the decision.

**Source:** [The Action Network](https://www.actionnetwork.com/entertainment/james-holzhauer-jeopardy-sports-betting-expected-value-2019); IBM Watson wagering research per [IBM Research News](http://ibmresearchnews.blogspot.com/2011/02/watsons-wagering-strategies.html)

### Drill 1: Daily Double Snap Decisions (10 Minutes)

**Goal:** Make DD wager sizing automatic by practicing game-state → wager decisions under time pressure.

**Setup:** A stack of 20 scenario cards (create from the table below, or use the scenarios at the end of this file). Each card lists: your score, opponents' scores, round (J! or DJ!), clues remaining, and category name. A timer.

**Protocol:**

1. Shuffle the scenario cards.
2. Set a timer — you have **15 seconds per card** to state your wager and one-sentence rationale.
3. Flip the card, read the scenario, announce your wager aloud.
4. After all 20 cards, review: were your decisions consistent with the framework above? Mark any where you froze, changed your mind, or made an arithmetic error.
5. Track: cards completed within 15 seconds, decisions consistent with framework (self-scored), time to decision (if using a stopwatch).

**Worked example scenario:** Your score: $6,200. Opponents: $4,800 and $3,100. Round: Jeopardy! (18 clues remaining). Category: "European History" (strong for you).

- **Analysis:** You lead by $1,400. Lots of game remaining. Strong category. Even if wrong, you have $0 and 18 clues to rebuild.
- **Recommended wager:** True Daily Double — $6,200. EV is strongly positive at 85%+ accuracy, and the downside is recoverable this early.
- **Time to decide:** Should take under 10 seconds with practice.

**Progression:**

| Week | Cards per Session | Time per Card | Focus |
|------|-------------------|---------------|-------|
| 1–2 | 10 | 20 seconds | Learn the framework, allow calculator |
| 3–4 | 15 | 15 seconds | No calculator, mental math only |
| 5+ | 20 | 10 seconds | Add pressure (standing, bright lights) |

**Source:** Framework derived from [The Action Network](https://www.actionnetwork.com/entertainment/james-holzhauer-jeopardy-sports-betting-expected-value-2019); drill structure is original (opinion — modeled on deliberate-practice principles)

---

## Part 2: Final Jeopardy Wagering

Final Jeopardy wagering is the most consequential single decision in any Jeopardy! game. The math uses only addition and subtraction. The hard part is not the arithmetic — it is classifying the game state quickly, under stage lights, with 30 seconds on the clock.

### Game Classification

Before calculating a wager, classify the game by the ratio of second place's score to first place's score. This determines which rules apply.

| Classification | Ratio (2nd ÷ 1st) | Leader's Situation |
|---------------|-------------------|-------------------|
| **Lock Game** | < 50% | Cannot lose regardless of FJ outcome. Bet $0–$999. |
| **Lock-Tie Game** | = 50% | Bet $0 (opponent can tie at most). Post-2014 rules: ties go to a tiebreaker clue, so $0 is still safe. |
| **Crush Game** | 50%–66.7% | Standard cover bet. Comfortable margin. |
| **Two-Thirds Game** | 66.7%–75% | Standard cover bet. Margins tighter. |
| **Three-Quarters Game** | > 75% | Standard cover bet. Very tight — one miscalculation loses. |

**Source:** [TheJeopardyFan.com, "Wagering Strategy 101"](https://thejeopardyfan.com/final-jeopardy-betting); [The Final Wager tutorial](https://thefinalwager.wordpress.com/tutorial/); `prep-strategies-research.md` (Final Jeopardy Wagering Math section)

### The Two-Stage Calculation

Every FJ wager follows a two-stage process. **Stage 1** determines the minimum you must bet to cover the next player's all-in. **Stage 2** checks whether being wrong at that wager level still beats the player behind you.

**Stage 1 — The Cover Bet (offense):**

```
Cover Bet = (2nd Place Score × 2) + $1 − Your Score
```

This is the amount the leader must wager to finish $1 ahead of a second-place player who bets everything and answers correctly.

**Stage 2 — The Safety Check (defense):**

```
Your Score − Cover Bet = Your Wrong-Answer Total
```

Compare this to third place's maximum (their score × 2). If your wrong-answer total exceeds third place's maximum, you are safe even when wrong. If not, you face **Stratton's Dilemma** (see below).

**Source:** [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting); [The Final Wager](https://thefinalwager.wordpress.com/tutorial/)

### Second-Place and Third-Place Wagers

Second-place players run the same two-stage process but in the opposite direction:

- **Stage 1:** "If the leader wagers the cover bet and is wrong, what score do they land on?" → Leader's Score − Cover Bet. You want to beat that number if you are right.
- **Stage 2:** "If I am wrong, does third place (going all-in) beat me?" → Your Score − Your Wager vs. 3rd Place × 2.

**Third place** has the simplest math: bet everything. Your only winning scenario is that both players ahead of you are wrong and you are right. Maximizing your correct-answer total gives the best chance.

**Source:** [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting); [Jeopardy.com, "Final Jeopardy! Wagering Strategy"](https://www.jeopardy.com/jbuzz/behind-scenes/final-jeopardy-wagering-strategy)

### Stratton's Dilemma

Named after Ted Stratton (Season 21, game #4695, aired 2005-01-21). Coined by Andy Saunders.

**Definition:** A second-place player faces Stratton's Dilemma when the minimum wager needed to cover third place (in case third goes all-in and is correct) exceeds the maximum wager that keeps them above the leader's projected wrong-answer score.

In plain English: you can't simultaneously protect yourself from the person behind you *and* stay positioned to beat the leader if they are wrong. You must choose.

**Community consensus:** Cover third place. Accept the leader's structural advantage and bet that the leader is wrong. The reasoning: if the leader is right with a proper cover bet, you lose regardless — you can only win on a triple stumper or leader-wrong scenario, and covering third ensures you at least survive to collect second-place money if only you are wrong.

**Source:** [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting); [JBoard.tv, "Final Jeopardy wagering theory"](https://jboard.tv/viewtopic.php?t=341); Andy Saunders, J-Archive community

### The Fundamental Principle

> "When leading, it is significantly better to lose by getting Final Jeopardy! incorrect than it is to lose by getting Final Jeopardy! correct and be overtaken by a trailing player."

Design your wager so being wrong doesn't cost you the game when your opponent is also wrong. This single sentence governs every FJ wager.

**Source:** [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting)

---

## Part 3: Worked Example Scenarios

### Scenario 1: Standard Crush Game (Leader's Perspective)

**Scores entering FJ:** You $18,700 | Player B $12,400 | Player C $6,000

**Step 1 — Classify:** $12,400 ÷ $18,700 = 66.3% → **Crush Game** (just under two-thirds).

**Step 2 — Cover bet:**
- (12,400 × 2) + 1 − 18,700 = 24,801 − 18,700 = **$6,101**

**Step 3 — Safety check:**
- Your wrong-answer total: 18,700 − 6,101 = **$12,599**
- Player C's maximum: 6,000 × 2 = $12,000
- $12,599 > $12,000 → **Safe.** Even if you are wrong, you beat Player C's best case.

**Optimal wager: $6,101.** If correct: $24,801 (beats Player B's max of $24,800). If wrong: $12,599 (beats Player C's max of $12,000). You win in all scenarios except "you wrong + Player B right," which no wager can prevent.

**Source:** [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting)

---

### Scenario 2: Lock Game (Leader's Perspective)

**Scores entering FJ:** You $22,000 | Player B $9,800 | Player C $5,400

**Step 1 — Classify:** $9,800 ÷ $22,000 = 44.5% → **Lock Game** (under 50%).

**Step 2 — Cover bet:**
- Player B's maximum: 9,800 × 2 = $19,600
- You already have $22,000 > $19,600. **No cover bet needed.**

**Step 3 — Optimal wager:** $0 to $2,399 (any amount that keeps you above $19,600 if wrong). Safest: **$0**. If you want to maximize winnings: $2,399 (22,000 − 2,399 = 19,601, still $1 above Player B's max).

**Why this matters for practice:** Lock games look easy on paper, but contestants make errors when they wager too much and convert a guaranteed win into a loss. In a televised Season 39 game, a leader with a lock game wagered $10,000 and lost after answering incorrectly — a win thrown away by arithmetic.

**Source:** [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting)

---

### Scenario 3: Three-Quarters Game with Stratton's Dilemma (Second Place's Perspective)

**Scores entering FJ:** Player A $16,000 | You $13,200 | Player C $8,600

**Step 1 — Leader's likely cover bet:**
- (13,200 × 2) + 1 − 16,000 = 26,401 − 16,000 = $10,401
- Leader's wrong-answer total: 16,000 − 10,401 = **$5,599**

**Step 2 — Your cover of Player C:**
- Player C's maximum: 8,600 × 2 = $17,200
- You need: wager enough so that if you are right, you beat $17,200. Minimum: 17,200 + 1 − 13,200 = **$4,001**
- Your wrong-answer total with that wager: 13,200 − 4,001 = **$9,199**

**Step 3 — Can you catch the leader if wrong?**
- Leader's wrong-answer total: $5,599
- Your wrong-answer total: $9,199
- $9,199 > $5,599 → **Yes.** If both are wrong, you win. No Stratton's Dilemma here.

**Now consider a tighter version:** Player C has $11,000 instead of $8,600.
- Player C's maximum: $22,000
- Minimum cover of C: 22,000 + 1 − 13,200 = **$8,801**
- Your wrong-answer total: 13,200 − 8,801 = **$4,399**
- Leader's wrong-answer total: $5,599
- $4,399 < $5,599 → **Stratton's Dilemma.** Covering Player C causes you to fall below the leader's wrong score.
- **Decision (consensus):** Bet $8,801 anyway. Cover third place. You can only win if the leader is wrong, and covering C ensures you survive a triple stumper or a C-right/you-wrong scenario.

**Source:** [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting); [JBoard.tv wagering theory](https://jboard.tv/viewtopic.php?t=341)

---

### Scenario 4: Real-Game Reconstruction (Boettcher vs. Holzhauer)

**Scores entering FJ:** Emma Boettcher $26,600 | James Holzhauer $23,400 | Jay Sexton $11,000

This is the game that ended Holzhauer's 32-game streak (aired June 3, 2019).

**Emma's calculation (leader):**
- Cover bet: (23,400 × 2) + 1 − 26,600 = 46,801 − 26,600 = **$20,201**
- Safety check: 26,600 − 20,201 = $6,399. Jay's max: 11,000 × 2 = $22,000. $6,399 < $22,000 — not safe against Jay, but Jay would need to be right while Emma is wrong. Emma accepted this and wagered $20,201.
- Final total (correct): $46,801.

**James's calculation (second place):**
- Emma's likely wrong-answer total: $6,399
- To beat Emma if both wrong: wager at most 23,400 − 6,400 = $16,999. But at that wager, if right: $40,399 — still below Emma's $46,801 if she is also right.
- James recognized he could only win if Emma was wrong. He pivoted to protecting second place: wager enough that even if wrong, he beats Jay's max ($22,000). So: 23,400 − wager ≥ 22,001 → wager ≤ $1,399. He wagered **$1,399**.
- James answered incorrectly. Final: $22,001 — exactly $1 above Jay's theoretical max.

**Lesson:** James's wager was strategically optimal given his reading of the game state. He could not catch Emma if she was right, so he locked in second place. This is a textbook defensive wager from a trailing position.

**Source:** [Jeopardy.com, "Final Jeopardy! Wagering Strategy"](https://www.jeopardy.com/jbuzz/behind-scenes/final-jeopardy-wagering-strategy); [TV Insider, "How Do Jeopardy! Players Decide on Their Final Wagers?"](https://www.tvinsider.com/1176782/jeopardy-final-jeopardy-wagering-strategy/)

---

## Drill Protocols

### Drill 2: Final Jeopardy Classification Speed (10 Minutes)

**Goal:** Classify game states instantly so the two-stage calculation starts from the right framework.

**Setup:** 15 scenario cards, each showing three players' scores. Timer.

**Protocol:**

1. Flip a card. Within **10 seconds**, state the game classification (Lock, Lock-Tie, Crush, Two-Thirds, Three-Quarters) and identify whether Stratton's Dilemma exists for second place.
2. Check against the answer key.
3. Track: correct classifications out of 15, average time per card.

**Worked example:** Scores: $14,000 / $9,500 / $4,200.
- Ratio: 9,500 ÷ 14,000 = 67.9% → **Two-Thirds Game.**
- Stratton check: Leader's cover bet = (9,500 × 2) + 1 − 14,000 = $5,001. Leader's wrong = $8,999. Second's cover of third: (4,200 × 2) + 1 − 9,500 = $0 (second already exceeds third's max). No Stratton's Dilemma.
- Time: should take 8–10 seconds with practice.

**Progression:** Same schedule as Drill 1 (Weeks 1–2: 20s per card, Weeks 3–4: 15s, Weeks 5+: 10s).

**Source:** Classification system from [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting)

---

### Drill 3: Full FJ Wager Calculation Under Pressure (15 Minutes)

**Goal:** Execute the complete two-stage calculation for all three positions in under 60 seconds, simulating the 30 seconds + commercial break contestants get on the show.

**Setup:** 10 scenario cards with three players' scores and position assignment (you are Player A, B, or C). Pen and scratch paper. Timer.

**Protocol:**

1. Flip a card. You have **60 seconds** to:
   - Classify the game.
   - Calculate your optimal wager using the two-stage process.
   - State your wager and one-sentence rationale.
2. Check against the answer key.
3. After all 10 scenarios, review errors. Categorize: arithmetic error, classification error, or strategic error (correct math, wrong reasoning).
4. Track: correct wagers out of 10, average time, error types.

**Target benchmarks:**

| Week | Scenarios | Time Limit | Target Accuracy |
|------|-----------|------------|-----------------|
| 1–2 | 5 | 90 seconds | 60% (learning) |
| 3–4 | 8 | 60 seconds | 80% |
| 5+ | 10 | 45 seconds | 90%+ |

**Worked example:** Card reads: "You are Player B. Scores: A = $15,800, B (you) = $11,200, C = $7,400."

- Classify: 11,200 ÷ 15,800 = 70.9% → Two-Thirds Game.
- Leader A's cover bet: (11,200 × 2) + 1 − 15,800 = $6,601. A's wrong-answer total: $9,199.
- Your cover of C: (7,400 × 2) + 1 − 11,200 = $3,601.
- Your wrong-answer total: 11,200 − 3,601 = $7,599.
- Stratton check: $7,599 < $9,199 → **No Dilemma.** If both you and A are wrong, you beat A.
- **Your wager: $3,601.** If right: $14,801 (doesn't beat A's correct total of $22,401, but beats C's max of $14,800). If wrong: $7,599 (beats A's wrong-answer total of $9,199? No — $7,599 < $9,199. Actually $7,599 < $9,199, so A would beat you if both wrong. Reconsider: should you wager *less* to stay above A's wrong total? Your max safe wager: 11,200 − 9,200 = $2,000. But then you don't cover C's max ($14,800 vs. your right total of $13,200). This is a judgment call — opinion: cover C at $3,601, accept the A-wrong risk.)

This kind of tension is exactly what the drill teaches. Not every scenario has a clean answer.

**Source:** Two-stage framework from [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting); [The Final Wager](https://thefinalwager.wordpress.com/tutorial/)

---

### Drill 4: Watch-and-Wager (20 Minutes)

**Goal:** Practice wagering in real time with actual game footage, combining classification, calculation, and decision-making under the emotional pressure of watching a competitive game unfold.

**Setup:** A recorded Jeopardy! episode (YouTube, streaming, or Pluto TV). Pen, scratch paper, and a score sheet. Pause remote.

**Protocol:**

1. Watch the episode normally through both rounds, tracking all three players' scores.
2. When the Final Jeopardy category is revealed (before the clue), **pause the episode.**
3. Write down the three scores. Set a 60-second timer.
4. Calculate your optimal wager for each of the three positions (leader, second, third). Write each down with a one-line rationale.
5. **Unpause.** Watch to see what the contestants actually wagered.
6. Compare your wagers to theirs. Were the contestants' wagers optimal? Were yours? Log any discrepancies.
7. Also calculate Daily Double wagers in real time as they appear: pause when the DD is revealed, note the scores, write your recommended wager, then compare to what the contestant wagered.

**What to track in `progress-tracker.md`:**
- FJ wagers calculated correctly (self-assessed against framework)
- DD wagers where your recommendation differed from the contestant's — and whether yours or theirs was better per the framework
- Number of Stratton's Dilemma scenarios encountered and handled correctly

**Worked example:** You watch Season 40, Game 85. Scores entering FJ: $19,200 / $14,600 / $8,200. You pause, classify (75.5% — Three-Quarters), calculate cover bet ($10,001), check safety ($9,199 vs. $16,400 — not safe against C, but C would need to be right while you're wrong). Contestant A wagered $12,000 — an overbid by $1,999 that unnecessarily risks falling below C's max. You caught the error. Log it.

**Source:** Drill structure is original; the watch-and-calculate method is widely recommended on [JBoard.tv](https://jboard.tv/viewtopic.php?t=4205) and [The Final Wager](https://thefinalwager.wordpress.com/tutorial/)

---

## Scenario Card Bank

Use these to create drill cards for Drills 1–3. Answers follow each scenario.

### Daily Double Scenarios

| # | Your Score | Opp A | Opp B | Round | Clues Left | Category Strength | Recommended Wager |
|---|-----------|-------|-------|-------|------------|-------------------|-------------------|
| 1 | $3,400 | $2,600 | $1,800 | J! | 22 | Strong | True DD ($3,400) — early game, small downside, strong category |
| 2 | $14,200 | $8,600 | $6,000 | DJ! | 18 | Weak | $5 minimum — preserve $5,600 lead in a weak category |
| 3 | $7,800 | $12,400 | $9,200 | DJ! | 12 | Strong | True DD ($7,800) — trailing, need to close gap |
| 4 | $16,000 | $8,100 | $5,400 | DJ! | 6 | Medium | $200–$1,000 — already near lock game; a small bet maintains advantage |
| 5 | $9,600 | $9,400 | $7,200 | DJ! | 15 | Strong | $5,000–$9,600 — tight race, strong category, need separation |

### Final Jeopardy Scenarios

| # | Player A | Player B | Player C | Your Position | Classification | Your Optimal Wager |
|---|---------|---------|---------|---------------|----------------|-------------------|
| 1 | $20,000 | $9,800 | $4,600 | A (leader) | Lock | $0–$399 |
| 2 | $17,400 | $13,000 | $9,200 | A (leader) | Three-Quarters | $8,601 |
| 3 | $15,600 | $11,800 | $3,200 | B (second) | Three-Quarters | $3,601 (cover C only — no Dilemma) |
| 4 | $21,000 | $14,800 | $10,400 | B (second) | Two-Thirds | $6,001 (cover C; Dilemma exists — accept it) |
| 5 | $18,200 | $12,600 | $6,800 | C (third) | Crush | $6,800 (all-in — only path to victory) |

---

## How to Measure Improvement

Track these metrics in `progress-tracker.md` (see the "Drill metrics" section — wagering decision outcomes vs. rule recommendation):

1. **DD decision accuracy:** Percentage of DD scenarios where your wager is consistent with the framework. Target: 90%+ by Week 4.
2. **FJ classification speed:** Average seconds to classify a game state. Target: under 10 seconds by Week 4.
3. **FJ wager accuracy:** Percentage of FJ scenarios where your calculated wager matches the optimal answer. Target: 80% by Week 3, 95% by Week 6.
4. **Watch-and-Wager error log:** Track how often real contestants make suboptimal wagers — this builds pattern recognition. Many contestants overbid in lock games or underbid in trailing positions.

**General transfer to trivia league:** Wagering drills are **Jeopardy!-specific** — most trivia league formats do not have wagering components. However, the decision-making under pressure and the habit of thinking about risk/reward translate loosely to final-round strategy in formats that involve point wagers. See the Transfer Classification table in `training-system.md` for the full breakdown.

---

## Quick Reference Card

Print or save this for at-a-glance use during practice.

```
DAILY DOUBLE
  Leading + strong category → Bet big (50–100%)
  Leading + weak category  → Bet $5
  Trailing                 → Bet big (true DD if needed)
  Near lock game (DJ!)     → Bet just enough to reach 2× second

FINAL JEOPARDY — LEADER
  1. Cover bet = (2nd × 2) + $1 − Your Score
  2. Safety: Your Score − Cover Bet > 3rd × 2? → Safe
  3. If not safe → Bet cover anyway (accept the risk)
  Lock game (2nd < 50% of you) → Bet $0

FINAL JEOPARDY — SECOND PLACE
  1. Leader's wrong total = Leader − Leader's Cover Bet
  2. Cover 3rd: (3rd × 2) + $1 − Your Score
  3. Your wrong total > Leader's wrong total? → No Dilemma
  4. Stratton's Dilemma? → Cover 3rd anyway

FINAL JEOPARDY — THIRD PLACE
  → Bet everything
```

**Source:** Synthesized from [TheJeopardyFan.com](https://thejeopardyfan.com/final-jeopardy-betting); [The Final Wager](https://thefinalwager.wordpress.com/tutorial/); [Jeopardy.com](https://www.jeopardy.com/jbuzz/behind-scenes/final-jeopardy-wagering-strategy)
