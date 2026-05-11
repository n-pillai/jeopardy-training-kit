# Knowledge-Gap Drills

This is a drill specification for identifying and closing knowledge gaps in Jeopardy! preparation. It is written for an experienced trivia competitor who already has broad general knowledge and needs a systematic method to find the specific categories where the show's clue writers will expose weaknesses. The problem is not "learn everything" — it is "find the 10–15 categories where you lose clues you should win, and close those gaps efficiently." These drills target that identification-and-remediation cycle; see `training-system.md` for how they fit into the weekly cadence, `drills/buzzer-drills.md` for the separate problem of timing, and `drills/wagering-drills.md` for wagering math.

---

## Core Concept: The Coryat Score as Diagnostic Tool

The Coryat score, developed by 1996 two-day champion Karl Coryat, strips out all wagering to isolate raw knowledge and buzzer skill. For knowledge-gap work, the Coryat score's real value is not the headline number — it is the **per-category breakdown** that reveals where you are losing clues.

**How Coryat scoring works (quick reference):**

- Correct response: + face value ($200–$2,000)
- Incorrect response (you buzzed in and were wrong): − face value
- Daily Doubles: score at face value only (no DD wager), no penalty for forced incorrect
- Final Jeopardy: excluded entirely

**Benchmarks:** A ~$24,000 Coryat average suggests a decent chance of passing the Anytime Test; ~$28,000 suggests strong competitiveness on the show. One practitioner documented a deliberate-tracking effect: their average rose from $18,200 to $21,800 over 3 weeks simply by paying attention to category-level performance and adjusting study accordingly.

**Source:** [J-Archive glossary](https://j-archive.com/help.php); [Trivia Bliss Coryat explainer](https://triviabliss.com/whats-a-coryat-score-in-jeopardy-everything-you-need-to-know/); [TheJeopardyFan.com top Coryat scores](https://thejeopardyfan.com/statistics/top-coryat-scores)

---

## Step 1: Identify Weak Categories

### Protocol 1A: Coryat Scoring with Category Tagging (J! Scorer Method)

**Goal:** Build a data set of per-category accuracy over 10+ games to identify statistically meaningful weaknesses.

**Setup:** [J! Scorer](https://j-scorer.com) (free, browser-based, created by Steve McClellan) or the [Coryat iOS app](https://apps.apple.com/us/app/coryat-j-scorekeeper/id1575111644) (free). Both pull games directly from J-Archive and allow category-level tagging.

**Protocol:**

1. Play one full J-Archive game per session, scoring along in real time using J! Scorer.
2. For each category, assign one or more **topic tags** (e.g., a category called "Rhyme Time" might be tagged "Wordplay"; "19th Century Americans" gets tagged "American History, Biography"). J! Scorer aggregates your accuracy by these tags across all saved games.
3. After each game, review the per-category results before closing the session. Note any category where you scored below 60% (3 of 5 correct in a standard category).
4. After 5 games, review the topic-tag summary page. Sort by accuracy. The bottom 5 topics are your initial gap list.
5. After 10 games, the gap list stabilizes. The bottom 3–5 topics become your active study targets.

**Worked example:** You play 10 J-Archive games over 2 weeks and tag every category. Your J! Scorer topic summary shows:

| Topic Tag | Clues Seen | Correct | Accuracy |
|-----------|-----------|---------|----------|
| Geography | 38 | 34 | 89% |
| American History | 29 | 25 | 86% |
| Literature | 33 | 26 | 79% |
| Science | 27 | 20 | 74% |
| Pop Music | 18 | 11 | 61% |
| Opera / Classical Music | 14 | 7 | 50% |
| Mythology | 12 | 5 | 42% |

Active gap list: **Mythology** (42%), **Opera / Classical Music** (50%), and **Pop Music** (61%). Geography and American History are strengths — no need to study these unless they stall.

**Source:** [J! Scorer](https://j-scorer.com); [J! Scorer help — topic tagging](https://j-scorer.com/help); [JBoard.tv J! Scorer discussion](https://jboard.tv/viewtopic.php?t=4317)

### Protocol 1B: The Data-Science Method (Word-Cloud Category Analysis)

**Goal:** Use frequency analysis of J-Archive clue data to identify the most common answers within your weak categories, so you study the highest-yield material first.

**Background:** Jeopardy! champion Colin Davy scraped ~400,000 clues from J-Archive, partitioned them by category, and generated word clouds of the most frequently appearing answers. He then studied only the most common answers in each weak category rather than trying to learn everything. He identified religion/the Bible as a personal weakness and used this method to efficiently target the highest-frequency answers.

**Protocol (simplified, no scraping required):**

1. After identifying your 3–5 weakest topics via Protocol 1A, go to [J-Archive's search page](https://j-archive.com/search.php).
2. Search for your weak category name (e.g., "opera"). Browse 20–30 clues from different seasons.
3. Tally which correct responses appear most often. In Opera, you will likely find Verdi, Puccini, Wagner, and *La Bohème* dominate.
4. Study the top 10–15 most frequent answers for that category first. This covers the highest-probability clues.
5. Extend to the next 10–15 answers only after the top tier feels automatic.

**Worked example:** You search J-Archive for "Opera" and tally correct responses across 30 clues:

| Answer | Appearances |
|--------|-------------|
| Verdi | 5 |
| Puccini | 4 |
| *La Bohème* | 3 |
| Wagner | 3 |
| *Carmen* (Bizet) | 3 |
| *Aida* | 2 |
| Pavarotti | 2 |

You create a one-page study sheet of the top 15 Opera answers with one memorable fact each (e.g., "Verdi — *Aida* premiered in Cairo in 1871 for the opening of the Suez Canal opera house"). Fifteen minutes of study covers the majority of Opera clues you will ever see on the show.

**Source:** Colin Davy, ["How I Won Jeopardy With Data Science"](https://colindavy.medium.com/how-i-won-jeopardy-with-data-science-c2e9b52a1958) (Medium, 2020)

---

## Step 2: Close the Gaps

### Protocol 2A: Targeted Category Deep-Dive (25-Minute Block)

**Goal:** Systematically improve accuracy in an identified weak category using a structured study session.

**Setup:** J-Archive search, Wikipedia, one-page study sheets (paper or digital), and optionally Anki for spaced repetition.

**Protocol:**

1. **Select the target** (2 min): Choose the weakest category from your current gap list in `progress-tracker.md`.
2. **Frequency scan** (5 min): Search J-Archive for the category. List the 10 most common correct responses you do not already know confidently.
3. **Context build** (12 min): For each of the 10 answers, learn one vivid contextual fact — a narrative hook that embeds the answer in episodic memory rather than rote memorization. Thieu's research (2024) shows trivia experts use intertwined semantic and episodic memory — they remember the context of how they learned a fact, making retrieval faster and more reliable. Jennings links facts in chains of 3–5 degrees of separation. Holzhauer recommends children's reference books because they present facts in memorable, simplified formats.
   - *Example:* To remember that Jean Sibelius is the Finnish composer Jeopardy! asks about, learn that he composed *Finlandia* as a protest against Russian censorship of the Finnish press in 1899 — a story, not a flash card.
4. **Recall test** (4 min): Cover the study sheet. For each of the 10 answers, can you retrieve it from a one-line prompt within 5 seconds? Mark any that take longer than 5 seconds for re-study next session.
5. **Log** (2 min): Record in `progress-tracker.md`: category studied, number of new answers learned, number that passed the 5-second recall test.

**Source for memory methods:** Monica Thieu, *Psychonomic Bulletin & Review* (2024), via [Scientific American](https://www.scientificamerican.com/article/jeopardy-winner-reveals-entwined-memory-systems-make-a-trivia-champion/); Ken Jennings, *Brainiac* (Villard, 2006); [Thrive Global, Holzhauer study methods](https://community.thriveglobal.com/james-holzhauer-jeopardy-champions-recall-information-under-stress-tips-strategies/)

### Protocol 2B: Pavlov Clue Study (15-Minute Block)

**Goal:** Learn the ~900 recurring phrase-to-answer associations ("Pavlov clues") that the show's writers rely on repeatedly.

**What Pavlov clues are:** When a Jeopardy! clue includes the phrase "Chinese-American architect," the answer is virtually always I.M. Pei. "Iowa painter" → Grant Wood. "Finnish composer" → Jean Sibelius. "Father of the Constitution" → James Madison. These are not trivia so much as pattern recognition — the writers use the same trigger phrases across decades. Compilations of ~900 Pavlovs exist.

**Setup:** [J!Study Guide Pavlov deck](https://www.jstudyguide.com/products/the-big-study-deck-of-jeopardy-pavlovs-j-study) (paid, ~$10) or the free [JBoard.tv Pavlov threads](https://www.jboard.tv/viewtopic.php?t=2202) compiled by the community. Optionally import into Anki for spaced repetition.

**Protocol:**

1. Work through 30 Pavlov pairs per session (15 min at ~30 seconds per pair).
2. For each pair: read the trigger phrase, attempt to recall the answer within 3 seconds, check.
3. Mark any missed pairs for re-review. Missed pairs go into a "retry stack" reviewed at the start of the next session.
4. Track: total Pavlovs studied, retry-stack size, percentage recalled on first attempt.

**Progression:**

| Phase | Pavlovs per Session | Target First-Attempt Recall |
|-------|--------------------|-----------------------------|
| Weeks 1–2 | 30 new / session | 50–60% (learning phase) |
| Weeks 3–4 | 20 new + 10 review | 70–80% |
| Weeks 5+ | 10 new + 20 review | 85%+ on review stack |

**Worked example:** You study 30 Pavlovs in your first session and recall 16 on first attempt (53%). The 14 you missed go into the retry stack. In the next session, review the 14 missed pairs first (recall 10 now — 71% on retry), then study 20 new pairs. By Week 4, the retry stack has shrunk to 8 and first-attempt recall rate on new batches is 78%.

**Transfer note:** Approximately 60% of Pavlov clues are general knowledge facts that would help in any trivia format (league play included); the remaining ~40% are Jeopardy!-writer-specific phrasings. See the Transfer Classification table in `training-system.md` for how Pavlov study is classified as "mixed" transfer.

**Source:** [JBoard.tv Pavlov threads](https://www.jboard.tv/viewtopic.php?t=2202); [J!Study Guide](https://www.jstudyguide.com/products/the-big-study-deck-of-jeopardy-pavlovs-j-study); `prep-strategies-research.md` (Knowledge Architecture section)

### Protocol 2C: Spaced Repetition with Anki (Ongoing)

**Goal:** Convert learned material into long-term recall using spaced repetition software, specifically targeting the ~5-second retrieval window that Jeopardy! demands.

**Setup:** [Anki](https://apps.ankiweb.net/) (free, cross-platform). Create a deck called "Jeopardy Prep" with sub-decks for each weak category and for Pavlov clues.

**Protocol:**

1. After each Protocol 2A deep-dive or Protocol 2B Pavlov session, create Anki cards for any new material that did not pass the 5-second recall test.
2. Card format: Front = the trigger phrase or a one-line clue-style prompt. Back = the correct response + one contextual fact.
3. Review Anki daily — the algorithm handles scheduling. Target: keep the daily review queue under 50 cards (roughly 10–15 minutes). If the queue exceeds 50, pause adding new cards until it drops below 30.
4. Use Anki's built-in statistics to track retention rate. Target: 85%+ mature-card retention.

**Key insight (opinion, not sourced):** Anki is not the primary learning tool — it is the *retention* tool. Learning happens during the deep-dive (Protocol 2A) and Pavlov study (Protocol 2B). Anki prevents forgetting what you've already learned. Do not use Anki to cram new material cold; the recall rate will be low and the experience frustrating.

**Source:** [BuzzerBlog.com](https://www.buzzerblog.com/thecall/) (recommends Anki for recall-speed training); Anki documentation at [apps.ankiweb.net](https://apps.ankiweb.net/)

---

## Step 3: Balance Weaknesses vs. Strengths

One of the most important strategic decisions is how to allocate study time between shoring up weak categories and extending strong ones. The research and champion accounts suggest the following framework:

### The 70/30 Rule (Opinion — Community Consensus, Not Formally Studied)

Allocate roughly **70% of knowledge study time to weak categories** and **30% to maintaining and extending strengths**. The reasoning:

1. **Weak categories have higher marginal returns.** Going from 40% to 70% accuracy in a category (learning ~6 new answers per 20 clues) is achievable in a few hours of targeted study. Going from 85% to 95% in a strong category requires far more effort for fewer additional correct responses.

2. **But strengths pay the bills.** Strong categories are where you build your Coryat base and where you can confidently bet big on Daily Doubles. Letting strengths atrophy while chasing weaknesses is counterproductive.

3. **Rotate weak categories.** Once a weak category rises above 70% accuracy over 5+ games (tracked in `progress-tracker.md`), move it off the active gap list and replace it with the next weakest topic. The gap list should always have exactly 3–5 active targets.

**Champion precedent:** Matt Amodio (38-game winner, 2021) described his approach as identifying personal weaknesses and "fine-tuning those" rather than studying every possible subject. He recognized his strengths in history, geography, literature, and classical music, and focused his preparation on modern pop culture — his identified gap.

**Source:** [Den of Geek, "How Do Jeopardy! Contestants Study?"](https://www.denofgeek.com/tv/jeopardy-how-do-contestants-study/); [Wikipedia, "Strategies and Skills of Jeopardy! Champions"](https://en.wikipedia.org/wiki/Strategies_and_skills_of_Jeopardy!_champions)

### When to Study Strengths

Spend the 30% "strengths" allocation on:

- **High-frequency categories where you are already strong** (e.g., Geography, U.S. Presidents). These categories appear so often that even a 90% accuracy rate means you are missing clues regularly in absolute terms. A single additional correct response per game in a high-frequency category is worth more than perfect accuracy in a category that appears once every 10 games.
- **Extending into adjacent areas.** If you are strong in American History, extend into Canadian or Mexican history — categories the show uses occasionally and that share overlapping knowledge structures.
- **Maintaining Pavlov recall.** Even after completing the Pavlov deck, review 10–15 per session to prevent decay.

---

## Tools Reference

| Tool | Cost | What It Does | Used In |
|------|------|-------------|---------|
| [J-Archive](https://j-archive.com) | Free | Complete archive of Jeopardy! clues and games dating to 1984. The canonical source for play-along games and category frequency data. | Protocols 1A, 1B, 2A |
| [J! Scorer](https://j-scorer.com) | Free | Real-time Coryat scorer with category topic tagging and cross-game stats. | Protocol 1A |
| [Coryat iOS app](https://apps.apple.com/us/app/coryat-j-scorekeeper/id1575111644) | Free | Mobile Coryat scorer with category tracking. | Protocol 1A (mobile) |
| [JBoard.tv](https://www.jboard.tv) | Free | Community forum with Pavlov compilations, category discussions, and study strategies. | Protocols 1B, 2B |
| [J!Study Guide Pavlov deck](https://www.jstudyguide.com/products/the-big-study-deck-of-jeopardy-pavlovs-j-study) | ~$10 | Curated deck of ~900 Pavlov clue-answer pairs. | Protocol 2B |
| [Anki](https://apps.ankiweb.net/) | Free | Spaced-repetition flashcard software for long-term retention. | Protocol 2C |
| [Trivial Studies](https://www.trivialstudies.com/jeopardy) | Free | Searchable Jeopardy! clue database with category filtering. | Protocols 1B, 2A |

All tools listed here are also annotated with full descriptions in `resources.md`. The "minimum viable kit" for knowledge work is: J-Archive + J! Scorer + a free Pavlov list from JBoard.tv. Total cost: $0.

---

## How to Measure Improvement

Track these metrics in `progress-tracker.md` (see the "Drill metrics" section — Coryat scores and weak categories):

1. **Coryat score per game:** The headline number. Plot weekly. Target trajectory depends on baseline — see `prep-strategies-research.md` for benchmark ranges.
2. **Per-topic accuracy (from J! Scorer):** The diagnostic number. Active gap-list categories should trend upward. A category exits the gap list when it sustains 70%+ accuracy over 5 consecutive games.
3. **Pavlov recall rate:** First-attempt recall percentage per session. Target: 85%+ on the review stack by Week 5.
4. **Anki retention rate:** Mature-card retention. Target: 85%+. If it drops below 80%, reduce new-card intake and focus on review.
5. **Gap list rotation:** How often categories rotate off the active gap list. Healthy rotation (one category exits every 2–3 weeks) indicates the system is working. If the same categories remain on the gap list for 4+ weeks without improvement, escalate: increase study time for those categories, try a different learning approach (e.g., switch from Anki cards to reading a narrative book or watching a documentary), or accept the gap and allocate time elsewhere.

**General transfer to trivia league:** Coryat scoring, category deep-dives, and Pavlov study all produce general-knowledge improvement that should be visible in league results. See the Transfer Classification table in `training-system.md` — these drills are tagged as "general transfer" or "mixed." Record league game results in `progress-tracker.md` and compare the pre-training baseline to rolling 4-week averages during training to detect whether knowledge-building work is translating to real-world performance.

---

## Escalation Protocol: When a Gap Won't Close

If a category remains below 60% accuracy after 3 weeks of targeted study (6+ deep-dive sessions), try the following escalation steps in order:

1. **Switch the learning modality.** If you have been using flashcards, try reading a short narrative book or watching a documentary series on the topic. Thieu's research suggests that episodic (story-based) memory formation is more robust than rote fact acquisition for trivia recall. Holzhauer specifically used children's reference books for this reason.
2. **Narrow the scope.** Instead of studying "Classical Music" broadly, target only "Classical Music composers who appear in Jeopardy! clues" — typically 15–20 names. Use Protocol 1B (frequency analysis) to find the exact list.
3. **Accept and de-prioritize.** Some categories may be genuinely outside your interest or cognitive strengths. If a category appears infrequently (fewer than 5 clues per 10 games) and resists improvement, move it off the active gap list and allocate time to higher-frequency weaknesses. The goal is not perfection — it is maximum Coryat improvement per hour of study.

**Source for escalation logic:** Monica Thieu, *Psychonomic Bulletin & Review* (2024), via [Scientific American](https://www.scientificamerican.com/article/jeopardy-winner-reveals-entwined-memory-systems-make-a-trivia-champion/); Jennings, *Brainiac* (Villard, 2006); Holzhauer's children's-book method per [Thrive Global](https://community.thriveglobal.com/james-holzhauer-jeopardy-champions-recall-information-under-stress-tips-strategies/)
