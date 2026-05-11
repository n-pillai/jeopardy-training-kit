# Goal

**Status:** done

## Objective

Build a **Jeopardy! Training System** designed to prepare a competitor to
compete and win on the actual show. The agent should research current public
prep wisdom (books, blogs, fan communities, former champions' guidance),
distill it, and produce a coherent training system that can be run day-to-day.

**v1 scope (this goal):** Terminate the loop when the document set is
complete and consistent. Do **not** attempt to run training, generate
practice content, or simulate progress.

**v2 (out of scope here, but design for it):** A future loop may extend to
"generate one week of training, run it, track outcomes (including ongoing
trivia league game results as a real-world progress signal), adjust,
generate next week." Where the v1 docs make assumptions or define structures
that v2 will iterate on, leave clear extension points (named sections,
fillable tables, explicit "to be measured weekly" markers).

Deliver six artifacts, all in the project folder:

1. `prep-strategies-research.md` — distilled research memo on what actually
   wins on Jeopardy!. Organize by impact tier (high/medium/low leverage). For
   each strategy: one-paragraph claim, the evidence behind it, and the source
   (URL or book title + author + year). Cover at minimum: buzzer timing,
   Daily Double / Final Jeopardy wagering, knowledge breadth vs. depth, recall
   speed, audition / contestant-search process, and stage performance under
   pressure.

2. `training-system.md` — the personal training system. Sections: weekly
   cadence (anchored to a realistic schedule with typical schedule constraints),
   session structure (what a 30-min session looks like vs. a 90-min block),
   ramp plan (weeks 1–2 baseline, weeks 3–6 build, weeks 7+ peak/maintain),
   what to do the week before an audition or taping, and a sample one-week
   schedule using only this kit's drills. Pull explicitly from
   `prep-strategies-research.md`.
   - **Real-world transfer:** explicitly identify which drills should
     produce metrics that improve trivia league performance (general
     transfer) vs. those that are Jeopardy!-specific (buzzer, wagering math,
     stage performance). League games are the cross-validation signal — the
     system should be designed so that progress on transferable drills shows
     up in league results.
   - **v2 hooks:** end with a short "Designed for week-by-week iteration"
     section listing the inputs a future loop will need (last week's tracker
     data, last 1–2 league game results, self-reported drill subjective
     ratings) and the outputs it will produce (next week's plan diff).

3. `drills/buzzer-drills.md` — buzzer timing drill specs. Include the physical
   setup options (clicker pen, phone app, J-Archive companion tools), 3+
   drill protocols with timing and progression, and how to measure
   improvement. Cite sources for each protocol's origin where possible.

4. `drills/knowledge-drills.md` — knowledge-gap drill specs. Methods to
   identify weak categories (Coryat scoring against J-Archive games, category
   tagging), drill protocols for closing identified gaps, and how to balance
   shoring up weaknesses vs. extending strengths. Reference real free tools
   (J-Archive, JBoard, etc.) — do not build new content.

5. `drills/wagering-drills.md` — wagering-strategy drill specs. Cover Daily
   Double sizing, Final Jeopardy wagering math (lock games, runaway games,
   trailing scenarios, Stratton/Saunders rules), and the two-stage Final
   wager calculation. Include 3+ worked example scenarios with the math.

6. `resources.md` — annotated ledger of tools, books, sites, and communities
   for ongoing prep. For each: what it is, who it's for, free/paid (and rough
   cost), time investment, and where it slots into the training system. End
   with a "minimum viable kit" subset (3–5 items) for someone starting today.

After all six exist, run a final integration pass and add `progress-tracker.md`
— a tracking template to fill in during practice. Sections:
- **Drill metrics:** Coryat scores per J-Archive game played, weak
  categories logged, buzzer reaction-time aggregates, wagering decision
  outcomes vs. the rule recommendation.
- **Trivia league baseline + ongoing results:** a place to record the
  pre-training baseline (the last 3+ league games before week 1, or as many
  as are available, with category-level breakdown if available), then
  per-game results during training. Designed so the v2 loop can read this
  section to detect whether general trivia performance is rising in
  parallel with Jeopardy!-specific drills, even with a small initial sample.
- **Subjective self-rating:** weekly 1–5 ratings on confidence, recall
  speed, buzzer feel, wager comfort, stage nerves — for the v2 loop to use
  as adjustment signal alongside the objective metrics.

Reference `progress-tracker.md` from `training-system.md` so the system and
the instrument stay coupled.

## Non-goals

- Do **not** modify any pipeline or planning documents. Pipeline updates
  happen during weekly review.
- Do **not** generate original trivia questions or "Jeopardy!-style" content.
  Point at existing free repositories (J-Archive is canonical). Building new
  trivia content is a different project (and a copyright minefield).
- Do **not** invent statistics or attribute claims to sources you can't cite
  (e.g. "85% of champions do X" without a real source). If a claim can't be
  sourced, mark it as an opinion or remove it.
- Do **not** speculate about Jeopardy!'s internal contestant-selection
  process beyond what the show publicly publishes. Treat the Anytime Test and
  audition path as the official channels.
- Do **not** recommend paid services without flagging the cost and a
  free-tier alternative.
- Do **not** assume the trainee has zero trivia background. The system should
  target the Jeopardy!-specific layer (buzzer, wagering, format adaptation,
  audition), not general trivia foundations.
- Do **not** make the training system require more than 90 minutes/day at
  peak. Schedule constraints are real; the system must be completable by
  someone with a full-time job and parenting obligations.
- Do **not** edit any files in `goal-kit/` or `.claude/`.

## Validation

For each of the seven deliverables, before logging it "done":

- File exists in the correct location (root or `drills/`).
- Has a one-paragraph "what this is and who it's for" header.
- Every empirical or strategic claim is sourced — URL, book + author + year,
  or named expert. Unsourced claims are removed or labeled as opinion.
- Every drill spec includes at least one worked example with concrete numbers
  (timing, score, category, etc.).
- Cross-references the other deliverables where topics touch (e.g.
  `training-system.md` references each drill file by name; `resources.md`
  lists tools that the drills assume).

After all seven exist, run a final consistency pass:
- Read all seven end-to-end in one iteration.
- Confirm terminology is consistent (e.g. "Coryat", "true Daily Double",
  "lock game" used the same way everywhere).
- Confirm the sample one-week schedule in `training-system.md` only
  references drills/tools that are actually defined in this kit.
- Confirm the "minimum viable kit" in `resources.md` is sufficient to run
  week 1 of the training system as written.
- Confirm `progress-tracker.md` includes a trivia-league section and that
  `training-system.md`'s "Real-world transfer" section is internally
  consistent with which drills the tracker measures for league transfer.
- Confirm `training-system.md` ends with a "Designed for week-by-week
  iteration" v2-hooks section listing the inputs/outputs of a future loop.

## Stop conditions

- All seven deliverables exist and pass the Validation checks → set Status to
  `done` and append a final progress log entry summarizing the system in 3–5
  lines.
- Three consecutive iterations produce no new content or no validation
  progress → set Status to `paused` and append a blocker note.
- A deliverable would require information that can't be obtained via
  publicly available web research (e.g. proprietary contestant-search data,
  paywalled material) → log the gap, ask the user, do not invent.
- Cumulative token usage across iterations exceeds 250K → set Status to
  `paused` for human cost/progress review.

## Progress log

2026-05-09T07:00:00Z | **Final consistency pass completed — goal done.** Read all 7 deliverables end-to-end. Found and fixed one terminology inconsistency: `progress-tracker.md` defined LBR as "Last-Beat Reps" (higher-is-better) while `drills/buzzer-drills.md` and `training-system.md` defined it as "Lost Buzzer Races" (lower-is-better); aligned tracker to match. All other checks passed: terminology consistent (Coryat, true Daily Double, lock/crush/two-thirds/three-quarters game classifications), sample one-week schedule references only drills and tools defined in the kit, MVK in `resources.md` covers Week 1, `progress-tracker.md` includes trivia-league baseline + ongoing sections, transfer classification in `training-system.md` is internally consistent with tracker metrics, and v2-hooks section lists matching inputs/outputs. **System complete:** 7 artifacts — research memo, training system, 3 drill specs, resource ledger, progress tracker — form a cohesive, cross-referenced Jeopardy! preparation kit designed for day-to-day use with clear v2 extension points for automated weekly iteration. | All validation checks pass. | Status set to done.

2026-05-09T06:15:00Z | Created `progress-tracker.md` (artifact 7/7) — 165-line tracking template with 5 sections: Coryat scores table with running average and benchmarks, weak-categories log with escalation protocol, buzzer metrics (RT/lockout/LBR), wagering drill outcomes with accuracy tracking, and session completion rate. Trivia league section has pre-training baseline (3+ games) and ongoing results with rolling 4-week averages and interpretation guide (rising/flat/declining). Subjective self-rating section covers 5 dimensions (confidence, recall speed, buzzer feel, wager comfort, stage nerves) on 1–5 scale. Weekly review checklist ties it all together. 4 worked examples with concrete numbers. Cross-references all 6 companion files. v2 hooks via HTML comments marking sections the loop will read. | Validation: file exists at root, has header paragraph, sourced benchmarks, 4 worked examples, cross-references all deliverables, trivia-league section present, subjective ratings match training-system.md's v2 inputs. Passes all per-deliverable checks. | Next step: run final consistency pass across all 7 deliverables.

2026-05-09T04:30:00Z | Created `resources.md` (artifact 6/7) — 258-line annotated resource ledger covering 15 online tools/sites (J-Archive, J! Scorer, Buzzer App, TheJeopardyFan, The Final Wager, JBoard, Jeopardy.com Prep Center, BuzzerBlog, Jeopardad, Seterra, Sporcle), 5 books (Holznagel, Jennings, Harris, Hamilton, Lewis), 1 hardware item (Delcom USB), 2 spaced-repetition resources (Anki, Pavlov lists), and 2 communities (Reddit, JBoard). Each entry annotated with description, audience level, cost, free alternative, time investment, and training-system placement. Includes cost summary table and 4-item Minimum Viable Kit ($0 total) mapped to Week 1. 26 cross-references to companion files, 17 URLs. | Validation: file exists at root, has header paragraph, no unsourced empirical claims, worked examples with numbers, cross-references all deliverables, MVK sufficient for Week 1. Passes all per-deliverable checks. | Next step: create `progress-tracker.md` (artifact 7), then run final consistency pass.

2026-05-09T01:15:00Z | Created `drills/wagering-drills.md` (artifact 5/7) — 405-line drill spec covering Daily Double sizing (EV framework, 5-scenario decision table), Final Jeopardy two-stage calculation (cover bet + safety check), game classification (lock/crush/two-thirds/three-quarters), Stratton's Dilemma, and 4 drill protocols (DD snap decisions, FJ classification speed, full FJ calculation under pressure, watch-and-wager with recorded episodes). Includes 4 fully worked scenarios with dollar-amount math (crush game, lock game, Stratton's Dilemma, Boettcher-vs-Holzhauer reconstruction), a 10-scenario card bank, and a printable quick-reference card. All claims sourced (TheJeopardyFan, The Final Wager, Jeopardy.com, Action Network, JBoard, IBM Watson research, Wikipedia). Cross-references all 6 companion files. | Validation: file exists in drills/, has header paragraph, 17 source citations, 4+ worked examples with concrete numbers, cross-references all deliverables. Passes all per-deliverable checks. | Next step: create `resources.md` (artifact 6).

2026-05-08T23:45:00Z | Created `drills/knowledge-drills.md` (artifact 4/7) — 210-line drill spec with 3-step structure: (1) identify weak categories via Coryat scoring with J! Scorer topic tagging and Colin Davy's frequency-analysis method, (2) close gaps via targeted 25-min deep-dives, Pavlov clue study (~900 pairs with progression schedule), and Anki spaced repetition, (3) balance weaknesses vs. strengths using a 70/30 allocation framework with gap-list rotation. Includes escalation protocol for persistent gaps, 7-tool reference table, 5 worked examples with concrete numbers. All claims sourced (J-Archive, J! Scorer, Colin Davy/Medium, JBoard, Thieu/Scientific American, Jennings, Holzhauer). Cross-references all 6 companion files. | Validation: file exists in drills/, has header paragraph, sourced claims, worked examples, cross-references. Passes all per-deliverable checks. | Next step: create `drills/wagering-drills.md` (artifact 5).

2026-05-09T00:10:00Z | Created `training-system.md` (artifact 2/7) — 291-line personal training system with weekly cadence (high-availability/low-availability weeks), session structures (30/60/90 min), 3-phase ramp plan (baseline → build → peak), pre-audition and pre-taping protocols, sample one-week schedule using only this kit's drills, transfer classification table (10 drills mapped to general-transfer vs. Jeopardy!-specific), league cross-validation logic, and v2-hooks section listing inputs/outputs for a future iteration loop. All claims sourced or labeled as opinion. 53 cross-references to companion files. | Validation: file exists at root, has header paragraph, sourced claims, worked examples with concrete numbers, cross-references all deliverables. Passes all per-deliverable checks. | Next step: create `drills/knowledge-drills.md` (artifact 4) or `drills/wagering-drills.md` (artifact 5).

2026-05-08T23:15:00Z | Created `drills/buzzer-drills.md` (artifact 3/7) — 218-line drill spec with 4 setup options (pen, Delcom USB, Buzzer App, recorded episodes), 4 drill protocols (light-reaction baseline, voice-anticipation timing, rapid-click endurance, full-game simulation), progression tables, worked examples with concrete numbers, and measurement framework. All claims sourced. Cross-references training-system.md, knowledge-drills.md, resources.md, progress-tracker.md. | Validation: file exists in drills/, has header paragraph, sourced claims, worked examples, cross-references. Passes all per-deliverable checks. | Next step: create `drills/knowledge-drills.md` (artifact 4) or `drills/wagering-drills.md` (artifact 5).

2026-05-08T22:30:00Z | Created `prep-strategies-research.md` (artifact 1/7) — 208-line research memo organized by impact tier covering buzzer timing, DD/FJ wagering, knowledge architecture, recall speed, audition process, and stage performance. All claims sourced with URLs or book citations. | Validation: file exists, has header paragraph, sourced claims, worked examples with numbers, cross-references `resources.md`. Passes all per-deliverable checks. | Next step: create `drills/buzzer-drills.md` (artifact 3) or `training-system.md` (artifact 2).
