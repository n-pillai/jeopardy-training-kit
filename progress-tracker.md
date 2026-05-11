# Jeopardy! Training Progress Tracker

This is the measurement instrument for the Jeopardy! training system described in `training-system.md`. It is designed for an experienced trivia competitor building Jeopardy!-specific skills on top of an existing knowledge base. Fill in each section as you train; the data here feeds the weekly review process and, in v2, will be read by an automated loop to generate personalized weekly plans. Every metric below corresponds to a drill protocol defined in `drills/buzzer-drills.md`, `drills/knowledge-drills.md`, or `drills/wagering-drills.md`, and every tool referenced is annotated in `resources.md`.

---

## Drill Metrics

### Coryat Scores

Record one row per J-Archive game played. Use [J! Scorer](https://j-scorer.com) or the Coryat iOS app to score; both pull games from [J-Archive](https://j-archive.com). See `drills/knowledge-drills.md` for the Coryat scoring protocol and category-tagging method.

| Date | Game # (J-Archive) | Coryat Score | Top 3 Categories | Bottom 3 Categories | Notes |
|------|---------------------|-------------|-------------------|----------------------|-------|
| | | | | | |

**Running average:** _____ (update weekly; benchmark: ~$24,000 = solid Anytime Test chance, ~$28,000 = strong show competitiveness — per `prep-strategies-research.md`)

**Worked example:** If you play J-Archive game #9012 on a Wednesday session and score $21,400, with correct responses in Shakespeare ($1,800), World Capitals ($2,000), and American History ($1,600) but misses in Opera ($0), Ballet ($-400), and Chemistry ($-200), the row would be:

| Date | Game # | Coryat | Top 3 | Bottom 3 | Notes |
|------|--------|--------|-------|----------|-------|
| 2026-05-12 | 9012 | $21,400 | Shakespeare, World Capitals, American History | Opera, Ballet, Chemistry | First time seeing Ballet as a category; Opera was a total blank |

### Weak Categories Log

Maintain a running list of categories that appear in your bottom 3 across multiple games. When a category appears 3+ times, escalate it to a targeted deep-dive using the gap-closing protocol in `drills/knowledge-drills.md`. Use the 70/30 allocation rule: 70% of knowledge study time on weak categories, 30% on extending strengths.

| Category | Times in Bottom 3 | Escalated to Deep-Dive? | Date Escalated | Status |
|----------|--------------------|------------------------|----------------|--------|
| | | | | |

<!-- v2: the loop reads this table to generate the next week's category priority list -->

### Buzzer Metrics

Record one row per buzzer drill session. See `drills/buzzer-drills.md` for drill protocols and progression targets. Measure reaction time (RT) with the Buzzer App or manual stopwatch method described in Drill 1.

| Date | Drill # | Delay Setting | Reps | Median RT (ms) | Lockout Rate (%) | LBR Count | Notes |
|------|---------|--------------|------|----------------|-----------------|-----------|-------|
| | | | | | | | |

**Key terms:**
- **Median RT:** Median reaction time in milliseconds from light activation to click. Target progression: ~230ms (baseline) → <200ms (Week 4) → <170ms (Week 6) → <150ms (peak). Benchmarks from Holznagel, *Secrets of the Buzzer* (2021).
- **Lockout Rate:** Percentage of attempts where you clicked before the light, triggering the 250ms penalty. Target: <15% for light-reaction drills, <25% acceptable for voice-anticipation drills.
- **LBR Count:** "Lost Buzzer Races" — clues where you knew the correct response but someone else buzzed in first. Lower is better. Target: <3 per game at peak (see `drills/buzzer-drills.md`, Drill 4 benchmarks).

**Worked example:** A Drill 4 (Full-Game Simulation) session: median RT = 204ms, lockout rate = 8%, LBR count = 5 (five clues where you knew the answer but lost the buzzer race).

| Date | Drill # | Delay | Reps | Median RT | Lockout % | LBR | Notes |
|------|---------|-------|------|-----------|-----------|-----|-------|
| 2026-05-14 | 4 | — | 60 | 204ms | 8% | 5 | Lost 5 buzzer races at avg $800 face value = $4,000 lost; grip improving per Holznagel |

### Wagering Drill Outcomes

Record one row per wagering drill session. See `drills/wagering-drills.md` for scenario banks and the two-stage Final Jeopardy calculation.

| Date | Drill # | Scenarios Attempted | Correct | Accuracy (%) | Avg Time per Scenario | Notes |
|------|---------|--------------------|---------|--------------|-----------------------|-------|
| | | | | | | |

**"Correct" means:** Your wager matched the optimal wager within $200 (for FJ scenarios) or matched the recommended action (for DD scenarios: aggressive / minimum / strategic). See the decision tables in `drills/wagering-drills.md`.

**Worked example:** A Drill 3 (Full FJ Calculation Under Pressure) session with 5 scenarios, 60-second time limit each: 4/5 correct (80%), average 42 seconds per scenario. The miss was a Stratton's Dilemma scenario where you forgot to check second place's optimal cover bet.

| Date | Drill # | Attempted | Correct | Accuracy | Avg Time | Notes |
|------|---------|-----------|---------|----------|----------|-------|
| 2026-05-15 | 3 | 5 | 4 | 80% | 42s | Missed Stratton's Dilemma — need to review trailing-leader logic |

### Session Completion

Track planned vs. completed sessions each week. A completion rate below 60% for 2 consecutive weeks triggers a burnout flag (see `training-system.md`, "Designed for Week-by-Week Iteration").

| Week Starting | Low-Availability Week? | Sessions Planned | Sessions Completed | Completion Rate | Notes |
|---------------|----------------------|------------------|--------------------|-----------------|-------|
| | | | | | |

<!-- v2: the loop reads completion rate to detect burnout risk -->

---

## Trivia League Baseline + Ongoing Results

### Pre-Training Baseline

Record the last 3+ trivia league games played before starting Week 1 of the training system. This establishes the cross-validation baseline that general-transfer drills (Coryat play, category deep-dives, full-game simulation) should improve over time. See `training-system.md`, "Real-World Transfer" section, for the transfer classification and validation logic.

| Date | League / Format | Score or Placement | Category Breakdown (if available) | Notes |
|------|----------------|-------------------|-----------------------------------|-------|
| | | | | |
| | | | | |
| | | | | |

**Baseline summary:** _____ (e.g., "Average placement: 3rd of 6 teams; strongest categories: history, geography; weakest: pop culture, science")

### Ongoing League Results (During Training)

Record every league game during training. Compare rolling 4-week averages to the baseline above. A sustained upward trend correlated with rising Coryat averages is the strongest evidence that knowledge-building drills are working (see `training-system.md`, "How League Results Validate Training").

| Date | Training Week # | League / Format | Score or Placement | Category Breakdown (if available) | Notable Misses or Strengths |
|------|----------------|----------------|-------------------|-----------------------------------|-----------------------------|
| | | | | | |

**Rolling 4-week average:** _____ (update every 4 weeks; compare to baseline)

**Interpretation guide:**
- League scores rising + Coryat rising = general-transfer drills are working. Stay the course.
- League scores flat + Coryat rising = knowledge gains are Jeopardy!-format-specific, not transferring. Adjust category targeting to overlap with league content areas.
- League scores declining + any Coryat trend = possible burnout or over-training. Consider a recovery week per `training-system.md`.

<!-- v2: the loop reads this section and the Coryat table to produce a league transfer report -->

---

## Subjective Self-Rating

Rate each dimension 1–5 at the end of each training week. These ratings are a v2 loop input (see `training-system.md`, "Designed for Week-by-Week Iteration") — they provide adjustment signal alongside the objective metrics above. If 3+ dimensions trend downward for 2 consecutive weeks, the v2 loop will recommend a recovery week.

**Scale:** 1 = very low / struggling, 2 = below average, 3 = adequate / steady, 4 = good / improving, 5 = strong / confident

| Week # | Date | Confidence | Recall Speed | Buzzer Feel | Wager Comfort | Stage Nerves | Notes |
|--------|------|------------|-------------|-------------|---------------|-------------|-------|
| | | | | | | | |

**Dimension definitions:**
- **Confidence:** Overall readiness feeling — "Could I perform well if I taped tomorrow?"
- **Recall Speed:** Subjective sense of how fast answers come during Coryat play and league games.
- **Buzzer Feel:** Comfort and timing intuition with the buzzer device. Are you anticipating well, or still reacting?
- **Wager Comfort:** Confidence in wagering math under time pressure. Can you do the cover-bet calculation in 30 seconds?
- **Stage Nerves:** Anxiety level during simulated game conditions or when imagining a real taping. 1 = very anxious, 5 = calm and focused.

**Worked example:** End of Week 3, first week of the Build phase:

| Week # | Date | Confidence | Recall Speed | Buzzer Feel | Wager Comfort | Stage Nerves | Notes |
|--------|------|------------|-------------|-------------|---------------|-------------|-------|
| 3 | 2026-05-26 | 3 | 3 | 2 | 4 | 2 | Buzzer still feels unnatural; wagering math is clicking; stage nerves high after watching a taping video |

---

## Weekly Review Checklist

Use this checklist during the Sunday review session (see `training-system.md`, weekly cadence). It ensures all metrics are logged and ready for the next week's planning.

- [ ] All Coryat games logged with category breakdown
- [ ] Weak categories list updated (escalate any category at 3+ appearances)
- [ ] Buzzer metrics logged for each drill session
- [ ] Wagering drill outcomes logged
- [ ] Session completion rate calculated
- [ ] League game results recorded (if league night occurred this week)
- [ ] Subjective self-ratings filled in for the week
- [ ] Compared this week's Coryat average to running average
- [ ] Compared this week's buzzer median RT to last week
- [ ] Identified next week's priority: which skill area needs the most attention?

<!-- v2: the loop runs this checklist programmatically and flags any missing data before generating the next week's plan -->
