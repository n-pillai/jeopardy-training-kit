# Jeopardy! Training Kit

A complete, research-backed preparation system for competing on Jeopardy! — built for experienced trivia competitors who want to layer on the show-specific skills that separate winners from knowledgeable-but-unlucky contestants.

This kit is also the first real-world use of [goal-kit](https://github.com/n-pillai/goal-kit): the entire document set was researched and written by a Claude Code agent running a long-horizon goal loop over several iterations. `GOAL.md` shows the objective, constraints, and per-iteration progress log exactly as the agent left them.

---

## What's in here

```
jeopardy-training-kit/
├── GOAL.md                        ← the agent's goal — objective, non-goals, validation, progress log
├── LoopOutcome.png                ← screenshot of the completed goal-kit run
├── prep-strategies-research.md   ← research memo: what actually wins on Jeopardy!
├── training-system.md            ← the full training system (weekly cadence, session structure, ramp plan)
├── progress-tracker.md           ← the tracking template you fill in during practice
├── resources.md                  ← annotated ledger of every tool, book, and community
├── drills/
│   ├── buzzer-drills.md          ← 4 buzzer drill protocols with progression tables
│   ├── knowledge-drills.md       ← Coryat scoring, category gap work, Pavlov study, Anki
│   └── wagering-drills.md        ← Daily Double + Final Jeopardy math, 4 drill protocols
└── .claude/                      ← goal-kit slash commands (active in any Claude Code session here)
    ├── commands/
    │   ├── goal.md               ← /goal <objective>
    │   ├── goal-status.md        ← /goal-status
    │   ├── goal-pause.md         ← /goal-pause
    │   ├── goal-resume.md        ← /goal-resume
    │   └── goal-clear.md         ← /goal-clear
    └── hooks/
        └── load_goal.py          ← SessionStart hook — auto-injects goal into every Claude session
```

---

## The training system at a glance

The kit targets the **Jeopardy!-specific layer** on top of existing general trivia knowledge:

| Skill | What it is | Where to start |
|-------|-----------|----------------|
| **Buzzer timing** | The lockout system punishes early clicks with a 250ms penalty. Mastering it is widely cited as the #1 differentiator between similarly-knowledgeable contestants. | `drills/buzzer-drills.md` |
| **Knowledge gaps** | Systematic Coryat scoring identifies your weakest categories. Targeted study closes them efficiently — no need to learn everything. | `drills/knowledge-drills.md` |
| **Wagering math** | Daily Double sizing and Final Jeopardy cover-bet calculations have optimal strategies. Most contestants leave money on the table. | `drills/wagering-drills.md` |
| **Stage performance** | Tape days run 5 games over ~8 hours. Physical stamina, composure under pressure, and smooth game-select mechanics all matter. | `prep-strategies-research.md` |

**Three phases:** Weeks 1–2 (baseline), Weeks 3–6 (build), Weeks 7+ (peak/maintain). Caps at 90 minutes/day. Low-availability weeks drop to ~1.5 hours — the system is designed to survive real life.

---

## How to use it

### Start here

1. Read `prep-strategies-research.md` for the research foundation.
2. Read `training-system.md` to understand the weekly structure and session formats.
3. Open `progress-tracker.md` — this is where you log everything.
4. Run Weeks 1–2 as pure baseline: 3–4 J-Archive Coryat games, 3 buzzer Drill 1 sessions, 5 wagering scenarios. No improvement targets yet — just measurement.

### Tools you'll need (all free to start)

- [J-Archive](https://j-archive.com) — complete clue archive, the canonical practice resource
- [J! Scorer](https://j-scorer.com) — Coryat scoring with category tagging
- [The Buzzer App](https://thebuzzerapp.com) — simulated lockout timing practice
- A clicky retractable pen — that's it for hardware until you're serious

Full annotated list with costs and training-system placement: `resources.md`.

---

## Using goal-kit to run a v2 loop

This repo ships with the goal-kit `.claude/` folder pre-installed. If you open this repo in Claude Code, the five `/goal*` slash commands are immediately available:

```
/goal-status          # see the current goal and recent progress
/goal-pause           # stop the loop, preserve state
/goal-resume          # pick back up from latest progress
/goal-clear           # archive current goal, start fresh
```

The SessionStart hook (`load_goal.py`) will auto-inject the goal context into every new Claude Code session while the goal status is `active` — so the agent never forgets what it's working on across session breaks.

The GOAL.md in this repo has `Status: done` (the v1 doc-building run is complete). To start a v2 loop — automated weekly plan generation based on your tracker data — set a new goal:

```
/goal Build a week-by-week training plan generator: read progress-tracker.md each week, produce a personalized plan diff
```

See [goal-kit](https://github.com/n-pillai/goal-kit) for full documentation on the loop runner, budget enforcement, and per-run JSON archive.

---

## Sources

Every empirical or strategic claim in the kit is sourced. Key references:

- Fritz Holznagel, *Secrets of the Buzzer* (2021) — buzzer timing science
- Ken Jennings, *Brainiac* (Villard, 2006) — knowledge architecture and recall
- Colin Davy, ["How I Won Jeopardy With Data Science"](https://colindavy.medium.com/how-i-won-jeopardy-with-data-science-c2e9b52a1958) (Medium, 2020)
- Monica Thieu, *Psychonomic Bulletin & Review* (2024) via [Scientific American](https://www.scientificamerican.com/article/jeopardy-winner-reveals-entwined-memory-systems-make-a-trivia-champion/)
- [BuzzerBlog.com](https://www.buzzerblog.com/thecall/) — contestant preparation guide
- [TheJeopardyFan.com](https://thejeopardyfan.com) and [The Final Wager](https://thefinalwager.com) — wagering strategy

Full annotated list in `resources.md`.
