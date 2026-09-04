# RAID Project — Historical Knowledge Extraction

I am migrating my RAID: Shadow Legends project from ChatGPT to Claude Cowork.

This conversation is **one of approximately 24 separate chats within my RAID project**. I need you to act as a **historical archivist** for THIS conversation.

Do not give me a generic summary.

Instead, carefully examine the entire conversation available to you and extract **as much useful RAID knowledge as possible** so that another AI can continue the project without losing the reasoning, decisions, strategies, recommendations, experiments, preferences, or account information contained here.

Your output will eventually be combined with the outputs from the other RAID conversations and given to Claude Cowork.

## CRITICAL RULES

### 1. Extract information; do not invent it

Only report information that is actually present or strongly established in this conversation.

If something is uncertain, say:

* `UNCERTAIN`
* `NOT CONFIRMED`
* `HISTORICAL`
* `NEEDS VERIFICATION`

Do not fill gaps with your general RAID knowledge.

You may explain RAID mechanics when necessary to make the historical discussion understandable, but clearly distinguish your explanation from information that came from me.

---

### 2. Preserve historical context

This is an archive, not just a snapshot of my current account.

Preserve:

* What we originally tried
* What we changed
* What worked
* What failed
* What we rejected
* Why we rejected it
* What I preferred
* What I disliked
* What I was trying to accomplish
* What conclusions we reached
* What remained unresolved

Another AI needs to understand **how we got here**, not just the final answer.

---

### 3. Do NOT assume old information is still current

A champion, team, build, goal, or recommendation may have been correct at the time but obsolete now.

Label things appropriately:

* `CURRENT` — explicitly current at the end of this conversation
* `HISTORICAL` — true/relevant at an earlier point
* `RECOMMENDED` — suggested but not necessarily implemented
* `TESTED` — actually tested
* `REJECTED` — considered and rejected
* `FAILED` — attempted and unsuccessful
* `PLANNED` — intended but not completed
* `COMPLETED`
* `UNCERTAIN`
* `NEEDS VERIFICATION`

If the conversation contains evidence that something changed, preserve both states and explain the change.

---

# OUTPUT FORMAT

Produce the following sections.

---

# 1. CONVERSATION OVERVIEW

Give this conversation a descriptive title.

Then provide:

* Approximate subject/date range if known
* Main purpose of the conversation
* Major RAID areas covered
* Most important conclusions

---

# 2. ACCOUNT / PROGRESSION INFORMATION

Extract every account-level fact mentioned.

Examples:

* Current progression
* Unlocked content
* Clan Boss difficulty
* Dungeons
* Doom Tower
* Hydra
* Arena
* Faction Wars
* Cursed City
* Events/tournaments
* Daily/weekly progression
* Resource limitations
* Gear limitations
* Any other progression information

For each important fact, indicate whether it appears current or historical.

Do not omit seemingly minor information if it could affect future team-building decisions.

---

# 3. CHAMPION ROSTER INFORMATION

Extract **every champion mentioned in this conversation**.

For each champion, capture whatever information is actually available:

| Champion | Owned? | Level | Rank | Ascension | Masteries | Blessing | Gear/Build | Role | Status | Notes |
| -------- | ------ | ----- | ---- | --------- | --------- | -------- | ---------- | ---- | ------ | ----- |

Possible status values:

* OWNED
* NOT OWNED
* RECOMMENDED
* CONSIDERED
* CURRENT
* BENCHED
* BUILT
* UNBUILT
* UNKNOWN

### IMPORTANT

A champion being mentioned does NOT automatically mean I own them.

Explicitly distinguish:

> "I own Champion X"

from:

> "ChatGPT suggested Champion X"

from:

> "We discussed Champion X as part of a theoretical team"

from:

> "I don't own Champion X"

This distinction is extremely important.

---

# 4. CHAMPION-SPECIFIC KNOWLEDGE

For every important champion discussed, extract:

* Why the champion was considered
* Their strengths
* Their weaknesses
* Their intended role
* What content they were being considered for
* Recommended build
* Recommended stats
* Masteries
* Blessing
* Gear
* Books
* Speed
* Accuracy
* HP/DEF/ATK/CR/CD/etc. where mentioned
* Skill priorities
* AI settings
* Whether they were ultimately used
* Whether they were rejected
* Why they were rejected
* Whether they are a future priority

Do not lose champion-specific reasoning.

---

# 5. TEAMS / COMPOSITIONS

This is one of the most important sections.

Extract **every meaningful team composition discussed**.

For each team:

## Team Name / Purpose

Example:
`Nightmare Clan Boss — Unkillable`

## Champions

1.
2.
3.
4.
5.

## Ownership

Indicate which champions were actually confirmed owned at the time.

## Intended Content

Examples:

* Clan Boss
* Arena
* Dungeon
* Doom Tower
* Hydra
* Faction Wars
* Cursed City
* Campaign
* etc.

## Strategy

Explain the team's intended strategy.

## Speed Tune

Capture every speed requirement or relationship mentioned.

Include:

* Champion speeds
* Turn order
* Speed ranges
* Speed ratios
* Boss speed assumptions
* Difficulty
* Rotation
* Skill cooldown timing
* Opening sequence

## Skill Settings

Capture:

* A1/A2/A3 priorities
* Auto/manual requirements
* Opening skill
* Delay requirements
* AI presets

## Required Stats

Capture:

* Accuracy
* Defense
* HP
* Crit Rate
* Crit Damage
* Attack
* Speed
* Resistance
* etc.

## Required Gear / Investment

Capture:

* Gear quality
* Sets
* Masteries
* Books
* Ascension
* Blessings
* Blessing level
* Great Hall requirements
* Other requirements

## Expected Performance

Capture any:

* Damage estimates
* Key counts
* Survivability
* Turn counts
* Speed
* Success rate
* Rewards
* Comparisons

## Result

Was the team:

* Recommended
* Built
* Tested
* Successful
* Failed
* Rejected
* Replaced
* Still under consideration

## Why

Preserve the reasoning.

---

# 6. CLAN BOSS — COMPLETE HISTORY

If Clan Boss was discussed at all, create a dedicated chronological history.

Capture:

### Starting Point

What was my original Clan Boss situation?

### Teams Tried

List every team.

### Problems

What went wrong?

Examples:

* Damage too low
* Champion dies
* Stun target problem
* Speed tune breaks
* Buff timing
* Debuff timing
* Lack of survivability
* Gear limitations
* AI problems

### Recommendations

What did ChatGPT recommend?

### Changes

What did I actually change?

### Results

What happened?

### Current Conclusion

What was the final recommendation/conclusion of this conversation?

### Outstanding Problems

What was still unresolved?

---

# 7. OTHER GAME CONTENT

Repeat the team/strategy extraction for any other RAID content discussed.

Possible categories:

* Arena
* Classic Arena
* Live Arena
* Tag Team Arena
* Clan Boss
* Hydra
* Doom Tower
* Faction Wars
* Cursed City
* Spider
* Dragon
* Fire Knight
* Ice Golem
* Sand Devil
* Shogun
* Iron Twins
* Phantom Shogun
* Campaign
* Events
* Tournaments
* Sintranos
* Any other content

Do not create empty sections unless relevant.

---

# 8. BUILDS / STAT TARGETS

Extract every meaningful build recommendation.

For each build:

* Champion
* Purpose
* Speed
* Accuracy
* HP
* DEF
* ATK
* Crit Rate
* Crit Damage
* Resistance
* Sets
* Main stats
* Substats
* Masteries
* Blessing
* Books
* Ascension
* Other requirements

Also record **why** those stats were recommended.

---

# 9. BLESSINGS

Extract every blessing discussion.

For each:

* Champion
* Recommended blessing
* Alternative blessings
* Reasoning
* Content where it applies
* Whether it was actually selected
* Whether the recommendation is current or historical

---

# 10. MASTERIES

Extract every mastery discussion.

Capture:

* Champion
* Recommended mastery tree
* Key masteries
* Reasoning
* Content
* Whether actually applied

---

# 11. GEAR

Extract meaningful gear recommendations.

Capture:

* Champion
* Gear sets
* Required stats
* Important pieces
* Gear quality
* Whether gear was available
* Gear farming recommendations
* Gear swaps
* Gear that should NOT be used

---

# 12. RESOURCES / INVESTMENT

Extract recommendations involving:

* Books
* Chickens
* Potions
* Silver
* Gems
* Energy
* Shards
* XP
* Gear
* Blessings
* Masteries
* Ascension
* Other scarce resources

Especially preserve recommendations involving **what NOT to spend resources on**.

---

# 13. PRIORITIES / GOALS

Extract every goal mentioned.

Separate:

### Immediate Goals

### Short-Term Goals

### Long-Term Goals

### Completed Goals

### Abandoned Goals

### Goals That Changed

For each goal, explain why it mattered.

---

# 14. RECOMMENDATIONS

Create a consolidated list of meaningful recommendations made during this conversation.

For each:

**Recommendation:**
**Reason:**
**For:**
**Status:**
**Still believed valid?** — only if the conversation itself establishes this.

Do not silently convert recommendations into facts.

---

# 15. REJECTED / FAILED STRATEGIES

This section is extremely important.

Document strategies that we tried, considered, or discussed and ultimately rejected.

For each:

* Strategy
* Why it looked promising
* Why it was rejected/failed
* What replaced it
* Whether it might still be useful later

The purpose is to prevent Claude from suggesting the same dead ends again.

---

# 16. DECISIONS

Extract meaningful decisions we made.

Format:

### Decision

### Date / Point in Conversation

### Context

### Decision

### Reasoning

### Alternatives Considered

### Consequence

### Current/Historical Status

Include decisions about:

* Teams
* Champions
* Builds
* Blessings
* Masteries
* Gear
* Resource spending
* Progression
* Strategy
* Priorities

---

# 17. USER PREFERENCES

Extract things I explicitly said I like/dislike/prefer.

This includes:

* Favorite champions
* Preferred playstyle
* Whether I prefer manual vs auto
* Whether I prioritize optimization vs favorites
* Whether I am willing to rebuild
* Whether I prefer simple/reliable teams
* Whether I care about efficiency
* Any other RAID-specific preferences

Do not infer preferences that I never stated.

---

# 18. QUESTIONS / UNCERTAINTIES

List every meaningful unresolved question.

Examples:

* Champion ownership not confirmed
* Speed not confirmed
* Gear unavailable
* Team not tested
* Damage unknown
* Blessing undecided
* Masteries undecided
* Need calculator validation

These should become future investigation items.

---

# 19. TOOLS / EXTERNAL RESOURCES

Extract any tools, websites, calculators, spreadsheets, databases, or other resources mentioned.

Examples include:

* DeadwoodJedi Clan Boss Calculator
* HellHades
* AyumiLove
* RAID Optimizer
* Other calculators/tools

For each explain what it was being used for.

---

# 20. IMPORTANT QUOTES / USER STATEMENTS

Do NOT create a transcript.

However, preserve a small number of exact user statements when the exact wording conveys an important:

* Goal
* Preference
* Constraint
* Decision
* Correction
* Frustration with a strategy
* Clarification about roster

Use quotes sparingly.

---

# 21. CHRONOLOGICAL TIMELINE

Create a concise timeline of the important developments in this conversation.

Example:

`Date/Stage → Situation → Decision → Result → Next Step`

Focus on changes in:

* Roster
* Teams
* Goals
* Strategy
* Builds
* Progression

---

# 22. END-OF-CONVERSATION STATE

This is extremely important.

Describe what was believed to be true **at the end of this conversation**.

Include:

### Current/Latest Team

### Current Goal

### Current Roster Facts

### Current Builds

### Current Priorities

### Known Problems

### Pending Decisions

### Recommended Next Step

This section should represent the final state reached in THIS conversation, even if that state may have subsequently changed in another RAID conversation.

---

# 23. KNOWLEDGE THAT ANOTHER AI MUST NOT LOSE

Finally, identify the **10–20 most important pieces of knowledge from this conversation** that Claude should absolutely retain when the individual conversation is no longer available.

Prioritize information that would prevent Claude from:

* Repeating a failed strategy
* Recommending unavailable champions
* Wasting resources
* Ignoring a stated preference
* Losing a strategic decision
* Misunderstanding my progression
* Repeating an already-solved problem

---

# 24. MACHINE-READABLE SUMMARY

At the very end, provide a compact structured section:

```yaml
conversation:
  title:
  primary_topic:
  date_range:

account:
  progression:
  clan_boss:
  other_content:

champions:
  - name:
    ownership:
    status:
    role:
    build:
    notes:

teams:
  - name:
    content:
    champions:
    strategy:
    speeds:
    requirements:
    status:
    result:
    notes:

goals:
  immediate:
  short_term:
  long_term:
  completed:
  abandoned:

decisions:
  - decision:
    reason:
    status:

recommendations:
  - recommendation:
    status:
    reason:

rejected_strategies:
  - strategy:
    reason:

preferences:
  - preference:

uncertainties:
  - item:

tools:
  - tool:
    purpose:

end_state:
  current_team:
  current_goal:
  current_priority:
  next_action:
```

Only populate fields supported by the conversation.

---

# FINAL INSTRUCTION

Be **exhaustive rather than brief**.

This output is going to be combined with approximately 23 other RAID conversation extractions.

I would rather receive a long, information-dense extraction containing useful historical details than a short polished summary that loses important information.

Do not spend space explaining what you are doing.

**Mine the conversation for knowledge and give me the knowledge.**
