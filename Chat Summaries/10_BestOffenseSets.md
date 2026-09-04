Below is the historical extraction for this specific conversation. I have treated **user statements as authoritative**, and assistant-generated claims as **recommendations/historical discussion rather than confirmed account facts**. Where the earlier assistant appears to have made an unsupported or potentially incorrect claim, I explicitly flag it rather than turning it into project knowledge.

# RAID Project — Historical Knowledge Extraction

## Conversation: RAID Champion Builds, Permanent Fusions, Campaign Modeling & Early Progression

---

# 1. CONVERSATION OVERVIEW

**Descriptive title:**
**RAID Champion Builds, Fusion Requirements, Campaign Node Modeling, and Early Champion Investment**

**Approximate date range:**
**December 19, 2025 – September 1, 2026**
The substantive RAID discussion occurred primarily **December 19, 2025 – February 2, 2026**, with this extraction requested September 1, 2026.

**Primary purpose of conversation:**

This conversation covered several relatively independent RAID topics:

1. Predator offensive masteries.
2. Correcting an inaccurate Predator mastery recommendation.
3. Whether Ronda was worth taking to 6★.
4. Broadmaw permanent fusion requirements.
5. Exact Broadmaw sub-fusion components.
6. Rhazin Scarhide permanent fusion requirements.
7. Farming locations for Rhazin's Rare components.
8. Designing a generalized `Capacities` / campaign-node data model for the user's RAID/SWGOH project.
9. Gear recommendations for Draconis.

**Major RAID areas covered:**

* Champion masteries
* Champion investment / 6★ decisions
* Permanent Fusions
* Campaign farming
* Campaign data modeling
* Champion gear
* Champion roster/resource planning

**Most important conclusions reached:**

* Predator should use an offensive mastery setup, but the user explicitly corrected the assistant because **Predator does not have Cycle of Violence available**. This is an important correction to preserve.
* Ronda was judged historically to be **worth taking to 6★ if she was going to be used**, although the conversation did not establish whether the user actually 6★ed her.
* Broadmaw's fusion was documented as requiring **Arbalester, Rockbeast, Huntress, and Bloodhorn**.
* Arbalester and Rockbeast were documented as being made from four Uncommons each.
* Rhazin Scarhide was documented as requiring **Lich, Erinyes, Bloodfeather, and Torturehelm**, with each Epic having four Rare components.
* The campaign-node modeling discussion concluded that RAID's Campaign structure is sufficiently different from SWGOH that a **separate RAID-specific node object was recommended**, rather than forcing the existing SWGOH-oriented `Node` object to handle both games.
* For Draconis, the historical recommendation was a **support/survivability-oriented build**, emphasizing Speed and HP rather than damage.

**Important archival warning:**
Several details in the historical assistant responses were presented with confidence but were not established by the user. They should **not** automatically be treated as verified RAID facts. This is particularly true of exact farming locations, drop rates, Draconis mechanics, and some mastery/build details.

---

# 2. ACCOUNT / PROGRESSION INFORMATION

Very little explicit account-level progression information was recorded in this conversation.

### Confirmed

* The user plays **RAID: Shadow Legends**.
* The user is maintaining a broader RAID project.
* The user also maintains a **SWGOH** project/data model and was attempting to determine whether RAID data should share structures with SWGOH.
* The user has a `Game Character` object in their project.
* The user has an existing `Node` object designed around SWGOH.
* The user is interested in tracking campaign farming locations and tying them to character-related data.

### NOT CONFIRMED

The conversation does **not** establish:

* Account level
* Current player level
* Clan Boss difficulty
* Clan Boss team
* Dungeon progression
* Doom Tower progression
* Hydra progression
* Arena tier
* Tag Team Arena tier
* Faction Wars progression
* Cursed City/Sintranos progression
* Gear dungeon levels
* Current shard inventory
* Silver inventory
* Gem inventory
* Energy inventory
* Champion vault contents
* Current 6★ roster
* Current legendary roster
* Current Rare/Epic fusion inventory

Therefore, another AI should **not infer account progression from the champions discussed**.

---

# 3. CHAMPION ROSTER INFORMATION

The conversation mentions many champions, but **almost none are explicitly confirmed as owned**.

This distinction is critical.

| Champion        | Owned?  |     Level |      Rank | Ascension          | Masteries       | Blessing | Gear/Build              | Role                   | Status     | Notes                                            |
| --------------- | ------- | --------: | --------: | ------------------ | --------------- | -------- | ----------------------- | ---------------------- | ---------- | ------------------------------------------------ |
| Predator        | UNKNOWN |   Unknown |   Unknown | Unknown            | Discussed       | Unknown  | Not established         | Damage/offensive       | CONSIDERED | User specifically corrected mastery availability |
| Ronda           | UNKNOWN |   Unknown |   Unknown | Unknown            | Not established | Unknown  | Not established         | Damage/debuffer        | CONSIDERED | User asked whether worth taking to 6★            |
| Broadmaw        | UNKNOWN |       N/A |      Epic | N/A                | N/A             | N/A      | N/A                     | Support/revive-related | CONSIDERED | Discussed as fusion target                       |
| Arbalester      | UNKNOWN |   Unknown |      Rare | Fusion requirement | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Broadmaw component                               |
| Rockbeast       | UNKNOWN |   Unknown |      Rare | Fusion requirement | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Broadmaw component                               |
| Huntress        | UNKNOWN |   Unknown |      Rare | Fusion requirement | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Broadmaw component                               |
| Bloodhorn       | UNKNOWN |   Unknown |      Rare | Fusion requirement | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Broadmaw component                               |
| Commander       | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Arbalester component                  |
| Hardscale       | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Arbalester component                  |
| Dhampir         | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Arbalester component                  |
| Satyr           | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Arbalester component                  |
| Brute           | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Rockbeast component                   |
| Jaeger          | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Rockbeast component                   |
| Warchanter      | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Rockbeast component                   |
| Militia         | UNKNOWN |   Unknown |  Uncommon | N/A                | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Historical Rockbeast component                   |
| Rhazin Scarhide | UNKNOWN | Legendary | Legendary | Fusion target      | N/A             | N/A      | N/A                     | Legendary fusion       | CONSIDERED | Permanent fusion discussion                      |
| Lich            | UNKNOWN |   Unknown |      Epic | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Rhazin component                                 |
| Erinyes         | UNKNOWN |   Unknown |      Epic | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Rhazin component                                 |
| Bloodfeather    | UNKNOWN |   Unknown |      Epic | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Rhazin component                                 |
| Torturehelm     | UNKNOWN |   Unknown |      Epic | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Rhazin component                                 |
| Magus           | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Lich component                                   |
| Marked          | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Lich component                                   |
| Rocktooth       | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Lich component; farming discussed                |
| Penitent        | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Lich component                                   |
| Raider          | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Erinyes component                                |
| Gnarlhorn       | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Erinyes component                                |
| Valerie         | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Erinyes component; farming discussed             |
| Wanderer        | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Erinyes component                                |
| Slitherbrute    | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Bloodfeather component                           |
| Goremask        | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Bloodfeather component; farming discussed        |
| Preserver       | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Bloodfeather component                           |
| Channeler       | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Bloodfeather component                           |
| Skullsworn      | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Torturehelm component; farming discussed         |
| Halberdier      | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Torturehelm component                            |
| Spikehead       | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Torturehelm component                            |
| Theurgist       | UNKNOWN |   Unknown |      Rare | Fusion component   | N/A             | N/A      | N/A                     | Fusion component       | CONSIDERED | Torturehelm component                            |
| Draconis        | UNKNOWN |   Unknown |   Unknown | Unknown            | Not established | Unknown  | Support build discussed | Support                | CONSIDERED | Gear recommendation                              |
| Hephraak        | UNKNOWN |       N/A | Legendary | N/A                | N/A             | N/A      | N/A                     | Damage                 | MENTIONED  | Used only as a comparative example               |
| Baron           | UNKNOWN |       N/A | Legendary | N/A                | N/A             | N/A      | N/A                     | Damage                 | MENTIONED  | Used only as comparative example                 |
| Nekhmet         | UNKNOWN |       N/A | Legendary | N/A                | N/A             | N/A      | N/A                     | Support                | MENTIONED  | Used only as comparative example                 |
| Valkyrie        | UNKNOWN |       N/A | Legendary | N/A                | N/A             | N/A      | N/A                     | Support/defense        | MENTIONED  | Used only as comparative example                 |
| Arbiter         | UNKNOWN |       N/A | Legendary | N/A                | N/A             | N/A      | N/A                     | Support                | MENTIONED  | Used only as comparative example                 |

### Important ownership conclusion

**No champion in this conversation should be marked OWNED unless another conversation establishes ownership.**

In particular, discussion of Ronda, Predator, Draconis, Broadmaw, or Rhazin does **not** prove that the user owned them.

---

# 4. CHAMPION-SPECIFIC KNOWLEDGE

## Predator

### Topic

The user asked:

> "in RAID: Shadow Legends, what are the best offense mysteries for Predator"

This was interpreted as asking for **offensive masteries**, not gear.

### Historical recommendations

The assistant initially proposed an offensive mastery path containing:

* Deadly Precision
* Keen Strike
* Single Out
* Bring It Down
* Cycle of Violence
* Methodical
* Kill Streak
* Helmsmasher / Warmaster

### User correction

The user explicitly stated:

> "he doesnt have cycle of violence"

This is the most important Predator-specific fact in this conversation.

### Result

The assistant acknowledged the error and produced a revised mastery recommendation without Cycle of Violence.

Historical revised recommendations included:

* Deadly Precision
* Keen Strike
* Shield Breaker
* Single Out
* Ruthless Ambush
* Bring It Down
* Methodical
* Kill Streak
* Helmsmasher as a possible Tier 6 choice

Warmaster was presented as an alternative for PvE/boss use.

### Status

**TESTED:** No actual in-game mastery application/testing was documented.

**CORRECTED:** The user caught an incorrect mastery recommendation.

**NEEDS VERIFICATION:** The exact optimal current Predator mastery tree was not independently validated during this conversation.

---

# Ronda

### User question

On January 9, 2026:

> "is Ronda worth taking to 6 *?"

### Historical conclusion

The assistant answered **yes, generally**, provided that Ronda would actually be used.

The reasoning given:

* 6★ provides substantially higher overall stats.
* 6★ unlocks the Banner slot.
* Ronda is a solid general damage dealer.
* Her kit was described as useful for Arena and various PvE areas.
* Her Block Passive Skills / Block Active Skills utility was highlighted.
* She was described as particularly attractive for an F2P player.

### Caveat

The assistant also stated that Ronda is not necessarily the highest-priority 6★ if the user has stronger/meta-defining champions waiting.

### Important account-status distinction

The user **never stated that Ronda was owned** in this conversation.

Therefore:

**Ronda ownership = UNKNOWN.**

The conversation also does not establish that she was actually promoted to 6★.

### Status

**RECOMMENDED historically.**

**NOT CONFIRMED implemented.**

---

# Broadmaw

Broadmaw was discussed strictly as a **permanent fusion target**.

Historical final fusion requirements given:

* Arbalester
* Rockbeast
* Huntress
* Bloodhorn

Each was stated to need to be at the required level/ascension before fusion.

### Historical component tree

```text
Broadmaw
├── Arbalester
│   ├── Commander
│   ├── Hardscale
│   ├── Dhampir
│   └── Satyr
├── Rockbeast
│   ├── Brute
│   ├── Jaeger
│   ├── Warchanter
│   └── Militia
├── Huntress
└── Bloodhorn
```

### Status

**CONSIDERED / RESEARCHED**

No evidence that the user actually completed the Broadmaw fusion.

---

# Rhazin Scarhide

Rhazin was discussed as a permanent Legendary fusion.

Historical final fusion:

```text
Rhazin Scarhide
├── Lich
├── Erinyes
├── Bloodfeather
└── Torturehelm
```

Historical Rare component tree:

```text
Lich
├── Magus
├── Marked
├── Rocktooth
└── Penitent

Erinyes
├── Raider
├── Gnarlhorn
├── Valerie
└── Wanderer

Bloodfeather
├── Slitherbrute
├── Goremask
├── Preserver
└── Channeler

Torturehelm
├── Skullsworn
├── Halberdier
├── Spikehead
└── Theurgist
```

Total Rare components discussed: **16**.

### Status

**CONSIDERED / RESEARCHED**

No evidence in this conversation that the user completed Rhazin.

---

# Draconis

### User question

On February 2, 2026:

> "best gear recommendations for Draconis"

### Historical role interpretation

The assistant treated Draconis as a **support-focused champion** rather than a primary damage dealer.

The historical recommendation emphasized:

* Speed
* HP
* Survivability
* Support utility

### Historical artifact recommendations

Suggested sets:

* Shield
* Speed
* Immortal
* Perception

The assistant specifically suggested:

**Shield + Speed** as a general PvE-oriented concept.

### Historical stat priorities

The assistant recommended:

1. Speed
2. HP%
3. Crit Rate / Crit Damage only if building for damage
4. Accuracy only where applicable

### Historical accessory/main-stat suggestions

The assistant proposed:

* Gloves: HP% or Speed
* Chest: HP%
* Boots: Speed
* Ring: HP% or DEF%
* Amulet: HP% or DEF%
* Banner: HP% or Speed

### Status

**RECOMMENDED historically.**

**NOT CONFIRMED implemented.**

### Verification warning

The exact mechanics and optimal modern Draconis build were not independently verified in this conversation. Treat the historical build as a prior recommendation, not an established current build.

---

# 5. TEAMS / COMPOSITIONS

There were **no actual complete RAID team compositions** developed in this conversation.

No five-champion team was built, speed-tuned, tested, or reported successful.

The conversation was primarily about individual champions, fusion trees, campaign farming, and data modeling.

---

# 6. CLAN BOSS — COMPLETE HISTORY

Clan Boss was **not meaningfully discussed**.

There was no:

* Clan Boss team
* Speed tune
* Difficulty
* Damage result
* Key count
* Stun targeting discussion
* AI setup
* Survivability testing

The assistant mentioned "boss/PvE" only in the context of choosing **Warmaster versus Helmsmasher** for Predator.

Therefore:

**Clan Boss status = NOT DISCUSSED / UNKNOWN.**

Do not infer a Clan Boss progression level from this conversation.

---

# 7. OTHER GAME CONTENT

## Campaign

Campaign was discussed in detail from a **data-modeling** perspective.

The user established the following RAID Campaign structure:

* 12 locations on the map
* 7 stages per location
* 4 difficulty settings:

  * Normal
  * Hard
  * Brutal
  * Nightmare

This is an explicit user-provided structural fact from the conversation.

### Existing Node object

The user's existing `Node` object contains:

* `Game`
* `Mode` — object select: Game Mode
* `Stage` — number
* `Battle` — text
* `Gear` — object select: Gear
* `Shards` — object select: Game Character

The object was originally designed for **SWGOH**.

### User's modeling problem

The user wanted to know whether to:

1. Modify the existing Node object so it can support both SWGOH and RAID, or
2. Create a separate RAID-specific object type.

### Historical recommendation

The assistant recommended a separate RAID-specific node object because RAID Campaign introduces multiple dimensions:

* Location
* Stage
* Difficulty

The suggested conceptual object was:

`RAID_Node`

with fields such as:

* Game
* Location
* Stage
* Difficulty
* Battle
* Gear
* Characters

The assistant also suggested a separate `Capacity` object to connect a character to a RAID node.

### Proposed Capacity concept

Historical proposed fields:

* `Game_Character`
* `RAID_Node`
* `Shard_Capacity`
* `Farmed_Count`
* `Last_Farmed_Date`

The purpose was to model a relationship between a character and a farmable location/reward.

### Important architectural conclusion

**RECOMMENDED:** Keep RAID campaign nodes separate from the SWGOH-oriented Node model.

**REASONING:** RAID's campaign hierarchy is multidimensional enough that forcing both games into the same Node schema risks unnecessary complexity and game-specific fields.

This was a design recommendation, **not confirmed as implemented**.

---

# 8. BUILDS / STAT TARGETS

## Predator

Historical offensive/mastery focus:

* Crit Rate
* Crit Damage
* Damage amplification
* DEF penetration through Helmsmasher
* Warmaster for PvE/boss scenarios

Specific mastery recommendations discussed:

* Deadly Precision
* Keen Strike
* Shield Breaker
* Single Out
* Ruthless Ambush
* Bring It Down
* Methodical
* Kill Streak
* Helmsmasher
* Warmaster

**Critical correction:** Cycle of Violence was initially recommended but the user explicitly said Predator does not have it.

---

## Ronda

Historical build discussion was limited.

The assistant stated that Ronda benefits from:

* Attack
* Crit Rate
* Crit Damage
* Speed

No exact numerical stat targets were established.

No exact artifact set was established.

No exact mastery tree was established.

No exact blessing was established.

---

## Draconis

Historical recommended direction:

### Purpose

Support / survivability.

### Priorities

1. Speed
2. HP%
3. Survivability
4. Accuracy only if needed

### Sets

* Shield
* Speed
* Immortal
* Perception

### Historical general build concept

**Shield + Speed** was presented as a useful PvE configuration.

No exact speed number was established.

No exact HP number was established.

No exact DEF target was established.

---

# 9. BLESSINGS

Very little blessing information occurred in this conversation.

### Predator

No blessing was established.

### Ronda

No blessing was established.

### Broadmaw

No blessing was established.

### Rhazin

No blessing was established.

### Draconis

No blessing was established.

### Conclusion

**No actionable blessing decisions were made in this conversation.**

---

# 10. MASTERIES

## Predator

This was the principal mastery discussion.

### Initial historical recommendation

The assistant initially proposed an offensive path including:

* Deadly Precision
* Keen Strike
* Single Out
* Bring It Down
* Cycle of Violence
* Methodical
* Kill Streak
* Helmsmasher / Warmaster

### User correction

The user explicitly stated:

> "he doesnt have cycle of violence"

### Revised historical recommendation

The assistant removed Cycle of Violence and instead proposed:

* Deadly Precision
* Keen Strike
* Shield Breaker
* Single Out
* Ruthless Ambush
* Bring It Down
* Methodical
* Kill Streak
* Helmsmasher

with Warmaster as a PvE alternative.

### Status

**CORRECTED**

**NOT TESTED**

**NEEDS VERIFICATION** for current optimality.

No mastery selection was explicitly confirmed as having been applied to Predator.

---

# 11. GEAR

## Draconis

Historical recommendation:

### Preferred direction

* Shield
* Speed

### Alternative sets

* Immortal
* Perception

### Stat emphasis

* Speed
* HP%

### General principle

The assistant advised prioritizing good stats over forcing a perfect artifact-set combination.

### Status

**RECOMMENDED**

**NOT CONFIRMED IMPLEMENTED**

---

## Predator

The first Predator answer was actually about **artifact sets**, despite the later conversation clarifying that the user wanted masteries.

Historical gear suggestions included:

* Merciless
* Savage
* Lethal
* Cruel
* Divine Offense

Historical reasoning emphasized:

* Damage
* Crit
* DEF ignore
* Offensive scaling

However, this portion should be treated as **historical/unverified**, because the user's follow-up clarified that their actual question was about masteries.

---

# 12. RESOURCES / INVESTMENT

## Ronda — 6★

Historical recommendation:

**Ronda is worth taking to 6★ if she is going to be used.**

Reasons given:

* Higher stats
* Banner slot
* Stronger damage
* Useful utility
* Broad PvE/PvP applicability

### Resource caveat

The assistant advised delaying Ronda if the account had higher-priority champions ready for 6★.

However, **the user's actual competing champions were never established**.

Therefore this was general advice rather than an account-specific resource decision.

---

## Fusion Resources

Broadmaw and Rhazin discussions imply investment in:

* Champion leveling
* Ascension
* Fusion components
* Campaign farming
* Shards for components that were claimed not to be campaign-farmable

No actual resource inventory was given.

---

# 13. PRIORITIES / GOALS

## Immediate Goals

### Historical

* Determine optimal offensive masteries for Predator.
* Determine whether Ronda deserved 6★ investment.
* Understand Broadmaw fusion requirements.
* Understand Rhazin fusion requirements.
* Identify campaign farming locations for Rhazin components.
* Determine an appropriate RAID campaign data model.
* Determine appropriate Draconis gear.

## Short-Term Goals

Not explicitly stated, but the conversation suggests an interest in:

* Building a reliable database of RAID champions and farming nodes.
* Tracking farmable champion acquisition.
* Integrating RAID data into the user's broader game-character project.

These are **strongly suggested by the modeling discussion**, but should be treated as project intent rather than a formally declared goal.

## Long-Term Goals

No explicit long-term RAID gameplay goal was stated in this conversation.

## Completed Goals

**Knowledge/research completed within conversation:**

* Broadmaw component tree documented.
* Rhazin component tree documented.
* RAID Campaign structure identified.
* Historical Draconis build recommendation generated.
* Predator mastery error identified and corrected.

## Abandoned Goals

None explicitly documented.

---

# 14. RECOMMENDATIONS

### Recommendation: Use an offensive mastery build for Predator

**Reason:** Predator was being treated as an offensive/damage-focused champion.
**For:** Predator
**Status:** RECOMMENDED historically
**Still believed valid?:** NOT ESTABLISHED

### Recommendation: Do not use Cycle of Violence on Predator

**Reason:** User explicitly corrected that Predator does not have this mastery.
**For:** Predator
**Status:** CORRECTED / IMPORTANT HISTORICAL FACT
**Still believed valid?:** This was directly stated by the user, but current game verification is outside this conversation.

### Recommendation: Consider Helmsmasher for offensive Predator

**Reason:** Historical recommendation emphasized DEF penetration and burst damage.
**For:** Predator
**Status:** RECOMMENDED historically

### Recommendation: Consider Warmaster for PvE/boss Predator

**Reason:** Historical recommendation treated Warmaster as the PvE/boss-oriented Tier 6 option.
**For:** Predator
**Status:** RECOMMENDED historically

### Recommendation: Take Ronda to 6★ if she is actively useful

**Reason:** Higher stats, Banner access, and general damage/utility.
**For:** Ronda
**Status:** RECOMMENDED historically
**Implementation:** NOT CONFIRMED

### Recommendation: Separate RAID nodes from SWGOH nodes

**Reason:** RAID Campaign has Location × Stage × Difficulty structure that differs substantially from the user's SWGOH Node model.
**For:** User's game database/project
**Status:** RECOMMENDED
**Implementation:** NOT CONFIRMED

### Recommendation: Use a RAID-specific Capacity relationship

**Reason:** To connect farmable character rewards with the RAID node where they can be obtained.
**For:** User's database
**Status:** RECOMMENDED
**Implementation:** NOT CONFIRMED

### Recommendation: Build Draconis around Speed + HP/survivability

**Reason:** Historical interpretation of Draconis as a support champion.
**For:** Draconis
**Status:** RECOMMENDED historically
**Implementation:** NOT CONFIRMED

---

# 15. REJECTED / FAILED STRATEGIES

## Predator — Cycle of Violence

**Strategy:** Include Cycle of Violence in Predator's offensive mastery path.

**Why it looked promising:**
The assistant was constructing a generic offensive mastery progression and included Cycle of Violence as a cooldown-related damage utility.

**Why rejected/failed:**
The user explicitly corrected:

> "he doesnt have cycle of violence"

**Replacement:**
A revised path omitting Cycle of Violence was provided.

**Future usefulness:**
Do not recommend it for Predator without independent verification of a future game change.

**Status:** REJECTED / CORRECTED.

---

## Forcing RAID and SWGOH into the same Node structure

**Strategy considered:** Modify the existing SWGOH `Node` object to accommodate RAID.

**Why it was questioned:**
RAID introduces Campaign Location and Difficulty dimensions that do not map cleanly to the user's existing SWGOH Node fields.

**Historical recommendation:**
Use a separate RAID-specific node object.

**Status:** The separate-object approach was **RECOMMENDED**, but the conversation does not confirm implementation.

---

# 16. DECISIONS

## Decision 1 — Correct Predator mastery path

**Date:** December 19, 2025

**Context:**
Assistant recommended Cycle of Violence.

**Decision:**
Remove Cycle of Violence.

**Reasoning:**
User explicitly stated Predator does not have it.

**Alternative:**
The assistant replaced it with another offensive mastery path.

**Consequence:**
Predator's mastery planning must not rely on Cycle of Violence.

**Status:** HISTORICAL / CORRECTED.

---

## Decision 2 — Ronda is a reasonable 6★ candidate

**Date:** January 9, 2026

**Context:**
User asked whether Ronda was worth taking to 6★.

**Decision:**
Historically recommended taking her to 6★ if she would actually be used.

**Reasoning:**
Improved stats, Banner access, damage, and utility.

**Consequence:**
Ronda was identified as a potentially worthwhile investment, subject to competing champion priorities.

**Status:** RECOMMENDED; actual implementation NOT CONFIRMED.

---

## Decision 3 — Broadmaw fusion tree

**Date:** January 9, 2026

**Decision:**
Use the documented four-Rare Broadmaw fusion structure.

**Status:** HISTORICAL KNOWLEDGE; completion NOT CONFIRMED.

---

## Decision 4 — Rhazin fusion tree

**Date:** January 9, 2026

**Decision:**
Document the four-Epic Rhazin fusion and its 16 Rare subcomponents.

**Status:** HISTORICAL KNOWLEDGE; completion NOT CONFIRMED.

---

## Decision 5 — Separate RAID campaign node model

**Date:** January 9, 2026

**Context:**
User was designing database objects for RAID and SWGOH.

**Decision:**
Historically recommended a RAID-specific node object instead of overloading the existing SWGOH-oriented Node object.

**Reasoning:**
RAID Campaign has:

* 12 locations
* 7 stages per location
* 4 difficulties

This creates additional structural dimensions.

**Status:** RECOMMENDED / NOT CONFIRMED IMPLEMENTED.

---

# 17. USER PREFERENCES

Only explicit preferences/corrections should be recorded.

### Accuracy of champion-specific mastery recommendations

The user actively noticed that Predator did not have Cycle of Violence and corrected the assistant.

This indicates that **generic mastery recommendations are not sufficient for this user's workflow**; champion-specific availability matters.

However, do **not** infer a broader personality preference beyond this explicit correction.

### Database/project modeling

The user is actively designing reusable game data objects and was considering whether RAID and SWGOH should share a Node model.

This indicates an interest in **structured game data modeling**, but no explicit preference for a particular database architecture was permanently stated.

### No explicit playstyle preference recorded

The conversation does not establish whether the user prefers:

* Manual or Auto
* Speed farming versus reliability
* Meta versus favorites
* F2P optimization
* Minimal rebuilds

Do not infer these from this conversation.

---

# 18. QUESTIONS / UNCERTAINTIES

The following remain unresolved from this conversation:

1. **Does the user actually own Predator?**
2. **Does the user actually own Ronda?**
3. **Did Ronda ever get promoted to 6★?**
4. **Does the user own any of the Broadmaw fusion components?**
5. **Did the user complete Broadmaw?**
6. **Does the user own any of Rhazin's 16 Rare components?**
7. **Did the user complete Rhazin?**
8. **Did the user implement the separate RAID Node object?**
9. **Did the user implement the proposed Capacity object?**
10. **What is the user's actual RAID campaign progression?**
11. **What is the user's actual gear quality?**
12. **What is Draconis's actual role/build in the user's account?**
13. **Was the Draconis Shield + Speed recommendation actually implemented?**
14. **What are the user's actual competing candidates for 6★?**
15. **What is the user's current Predator mastery configuration?**
16. **What is the user's current Ronda build?**
17. **Which Broadmaw/Rhazin components are currently in the user's roster?**
18. **Are the historical farming locations provided by the assistant accurate under the current RAID version?**
19. **Are the historical mastery recommendations still optimal under the current RAID version?**
20. **Are the historical Draconis mechanics/build recommendations still current?**

---

# 19. TOOLS / EXTERNAL RESOURCES

The assistant referenced several external RAID resources during the conversation:

### HellHades

Used for:

* Champion information
* Ronda information
* Rhazin fusion information
* Draconis information
* Artifact/build information

**Status:** Referenced historically.

### AyumiLove

Used for:

* Champion skills/masteries
* Ronda information
* Predator information
* RAID artifact/farming information

**Status:** Referenced historically.

### RaidNinja

Used for:

* Predator build/mastery recommendations

**Status:** Referenced historically.

### Inteleria

Used for:

* Mastery lists
* Artifact set information

**Status:** Referenced historically.

### RAID Support / Plarium

Used for:

* Fusion requirements/rules

**Status:** Referenced historically.

### Reddit

Used as a source of community opinion around Ronda and fusion-related questions.

**Status:** Historical/community source, not an account fact.

### Important verification note

The conversation's external-source usage was **not comprehensive validation**. Some assistant responses appear to have generalized or potentially conflated RAID mechanics. Future use should independently verify current mechanics rather than treating every historical citation as authoritative.

---

# 20. IMPORTANT QUOTES / USER STATEMENTS

These are the most useful exact user statements.

### Predator correction

> "he doesnt have cycle of violence"

This is especially important because it identifies a concrete error in the previous recommendation.

### Ronda investment question

> "is Ronda worth taking to 6 *?"

This establishes that 6★ investment was under consideration, but not that it happened.

### Broadmaw component request

> "yes, please list exact Fusion components"

This indicates the user wanted the complete fusion tree rather than only the final fusion requirements.

### Rhazin farming request

> "yes, please list where to farm each"

This establishes that the user was interested in practical acquisition/farming information, not merely theoretical fusion composition.

### Database architecture question

> "can you help me design a Capacities object to track these, so I can tie them to my Game Character object?"

This is important project context: the user wanted farmability/capacity information connected directly to their `Game Character` records.

### Existing data model

> "I have a Node object, with:
>
> * Game
> * Mode (object select: Game Mode)
> * Stage (number)
> * Battle (text)
> * Gear (object select: Gear)
> * Shards (object select: Game Character)"

This is the concrete schema that existed at that point.

### Cross-game modeling concern

> "I built it to work with SWGOH, but not sure if it's better to modify to work with both games, or create a new object type"

This captures the architectural decision being considered.

---

# 21. CHRONOLOGICAL TIMELINE

### December 19, 2025 → Predator offensive build

**Situation:**
User asked for the best offensive masteries for Predator.

**Initial recommendation:**
Assistant gave a damage-oriented mastery path.

**Problem:**
Assistant included Cycle of Violence.

**User correction:**
User stated Predator does not have Cycle of Violence.

**Result:**
Assistant revised the mastery recommendation without it.

**Status:** Corrected, but not tested.

---

### January 9, 2026 → Ronda 6★ decision

**Situation:**
User asked whether Ronda was worth taking to 6★.

**Recommendation:**
Yes, if she would be used.

**Reasoning:**
Higher stats, Banner access, damage and utility.

**Result:**
No actual 6★ promotion was reported.

**Status:** Recommendation only.

---

### January 9, 2026 → Broadmaw fusion

**Situation:**
User asked for Broadmaw's fusion requirements.

**Recommendation/documentation:**
Broadmaw requires:

* Arbalester
* Rockbeast
* Huntress
* Bloodhorn

Then the user requested the exact subcomponents.

**Result:**
Arbalester and Rockbeast component trees were documented.

**Status:** Research completed; fusion completion not confirmed.

---

### January 9, 2026 → Rhazin Scarhide

**Situation:**
User asked for Rhazin's components.

**Recommendation/documentation:**
Rhazin requires:

* Lich
* Erinyes
* Bloodfeather
* Torturehelm

Each was given a four-Rare component tree.

**Result:**
A complete 16-Rare component list was produced.

---

### January 9, 2026 → Rhazin farming

**Situation:**
User asked where to farm each Rare.

**Result:**
Assistant identified several alleged campaign-farmable Rares and classified others as shard-only.

**Important:**
These farming claims were not independently validated in this conversation and should be considered **HISTORICAL / NEEDS VERIFICATION** before being used as current database data.

---

### January 9, 2026 → RAID campaign database architecture

**Situation:**
User explained RAID Campaign:

* 12 locations
* 7 stages each
* 4 difficulties

The user showed the existing SWGOH-oriented Node schema.

**Problem:**
Whether to adapt Node for both games or create a new object.

**Recommendation:**
Create a RAID-specific node object and connect farmability/capacity to Game Character.

**Status:** Recommended; implementation not confirmed.

---

### February 2, 2026 → Draconis gear

**Situation:**
User asked for the best gear recommendations for Draconis.

**Recommendation:**
Build him as a support-oriented champion emphasizing:

* Speed
* HP
* Survivability

Historical preferred sets:

* Shield
* Speed

with Immortal/Perception as alternatives.

**Status:** Recommendation only.

---

### September 1, 2026 → Historical extraction

**Situation:**
User requested exhaustive archival extraction for migration to Claude Cowork.

**Purpose:**
Preserve the historical reasoning, corrections, recommendations, project architecture, and unresolved questions from this conversation.

---

# 22. END-OF-CONVERSATION STATE

## Current/Latest Team

**NONE ESTABLISHED.**

No complete RAID team was active or documented at the end of the conversation.

## Current Goal

The final substantive topic was:

**Draconis gear/build recommendations.**

However, there was no explicit statement that this was the user's overarching current RAID goal.

## Current Roster Facts

No champion ownership was confirmed in this conversation.

The champions discussed should therefore remain **UNKNOWN ownership** unless corroborated by another RAID project conversation.

## Current Builds

### Predator

Offensive mastery discussion exists, but actual mastery application is unknown.

### Ronda

6★ was recommended if useful, but actual rank is unknown.

### Draconis

Historical recommendation was a Speed + HP/support-oriented build, but implementation is unknown.

## Current Priorities

No definitive account-wide priority order was established.

## Known Problems

* An incorrect Predator mastery recommendation was made and corrected.
* Exact current farmability of Rhazin components needs verification.
* Exact implementation of the RAID campaign data model is unknown.
* Current champion ownership was not captured.

## Pending Decisions

* Whether/when to 6★ Ronda.
* Which fusion components the user actually possesses.
* Whether to complete Broadmaw.
* Whether to complete Rhazin.
* Whether the RAID-specific Node/Capacity schema was implemented.
* Whether Draconis's recommended gear was actually applied.

## Recommended Next Step

For continuation of the larger RAID project, the next AI should **not assume these recommendations were implemented**. It should reconcile:

1. Current champion roster.
2. Current ranks/builds.
3. Current fusion component inventory.
4. Current database schema.
5. Current campaign-node data.
6. Current RAID mechanics/version.

---

# 23. KNOWLEDGE THAT ANOTHER AI MUST NOT LOSE

1. **Predator does NOT have Cycle of Violence according to the user's explicit correction.** The assistant initially recommended it, and the user caught the error. Do not repeat that recommendation without current verification.

2. **Ronda was historically considered worth taking to 6★ if she would actually be used.** This was a recommendation, not confirmation that the user owns or upgraded her.

3. **Broadmaw's documented final fusion components were Arbalester, Rockbeast, Huntress, and Bloodhorn.**

4. **Arbalester's documented subcomponents were Commander, Hardscale, Dhampir, and Satyr.**

5. **Rockbeast's documented subcomponents were Brute, Jaeger, Warchanter, and Militia.**

6. **Rhazin Scarhide's documented final fusion components were Lich, Erinyes, Bloodfeather, and Torturehelm.**

7. **Lich's documented Rare components:** Magus, Marked, Rocktooth, Penitent.

8. **Erinyes's documented Rare components:** Raider, Gnarlhorn, Valerie, Wanderer.

9. **Bloodfeather's documented Rare components:** Slitherbrute, Goremask, Preserver, Channeler.

10. **Torturehelm's documented Rare components:** Skullsworn, Halberdier, Spikehead, Theurgist.

11. **The user explicitly described RAID Campaign as 12 locations × 7 stages, with Normal, Hard, Brutal, and Nightmare difficulties.**

12. The user's existing `Node` object was originally designed for **SWGOH** and contained:

    * Game
    * Mode
    * Stage
    * Battle
    * Gear
    * Shards

13. The user was specifically considering a `Capacities` object tied to the `Game Character` object so that farmability could be tracked.

14. The historical architectural recommendation was to create a **separate RAID-specific Node object**, rather than making the SWGOH Node object increasingly game-specific.

15. A proposed RAID Capacity relationship included a character, RAID node, shard capacity, farmed count, and last-farmed date. This was **proposed, not confirmed implemented**.

16. The Rhazin farming-location information supplied by the assistant is **HISTORICAL / NEEDS VERIFICATION**. Do not import it into a current database without checking it.

17. The historical Draconis recommendation was a **support/survivability build**, emphasizing Speed and HP rather than damage.

18. Historical Draconis gear suggestions included **Shield + Speed**, with Immortal and Perception as alternatives. This was a recommendation, not confirmed implementation.

19. **No complete team composition was established in this conversation.** Do not invent a team from the champions mentioned.

20. **Champion mentions do not establish ownership.** Predator, Ronda, Draconis, Broadmaw, Rhazin, and all fusion components should remain UNKNOWN ownership unless another conversation confirms them.

---

# 24. MACHINE-READABLE SUMMARY

```yaml
conversation:
  title: "RAID Champion Builds, Fusion Requirements, Campaign Modeling, and Early Progression"
  primary_topic: "RAID champion masteries/builds, permanent fusions, campaign farming, and game-data modeling"
  date_range: "2025-12-19 through 2026-09-01"

account:
  progression: "UNKNOWN"
  clan_boss: "NOT DISCUSSED"
  other_content: "Campaign structure discussed; no account progression confirmed"

champions:
  - name: "Predator"
    ownership: "UNKNOWN"
    status: "CONSIDERED"
    role: "offensive damage"
    build: "offensive mastery path discussed"
    notes: "User explicitly corrected that Predator does not have Cycle of Violence"

  - name: "Ronda"
    ownership: "UNKNOWN"
    status: "RECOMMENDED"
    role: "damage/debuffer"
    build: "6-star investment discussed"
    notes: "Historically recommended for 6-star if actively used; actual upgrade not confirmed"

  - name: "Broadmaw"
    ownership: "UNKNOWN"
    status: "CONSIDERED"
    role: "fusion target"
    build: "UNKNOWN"
    notes: "Fusion requirements documented"

  - name: "Rhazin Scarhide"
    ownership: "UNKNOWN"
    status: "CONSIDERED"
    role: "legendary fusion target"
    build: "UNKNOWN"
    notes: "Fusion tree with 16 Rare components documented"

  - name: "Draconis"
    ownership: "UNKNOWN"
    status: "RECOMMENDED"
    role: "support"
    build: "Speed + HP/survivability; Shield + Speed historically suggested"
    notes: "Actual implementation unknown"

  - name: "Arbalester"
    ownership: "UNKNOWN"
    status: "CONSIDERED"
    role: "Broadmaw fusion component"
    build: "N/A"
    notes: "Documented as fused from Commander, Hardscale, Dhampir, Satyr"

  - name: "Rockbeast"
    ownership: "UNKNOWN"
    status: "CONSIDERED"
    role: "Broadmaw fusion component"
    build: "N/A"
    notes: "Documented as fused from Brute, Jaeger, Warchanter, Militia"

  - name: "Huntress"
    ownership: "UNKNOWN"
    status: "CONSIDERED"
    role: "Broadmaw fusion component"
    build: "N/A"
    notes: "Fusion component"

  - name: "Bloodhorn"
    ownership: "UNKNOWN"
    status: "CONSIDERED"
    role: "Broadmaw fusion component"
    build: "N/A"
    notes: "Fusion component"

teams: []

goals:
  immediate:
    - "Determine effective Predator offensive masteries"
    - "Evaluate Ronda for 6-star investment"
    - "Document Broadmaw fusion"
    - "Document Rhazin fusion"
    - "Identify farming locations for fusion components"
    - "Design RAID campaign data model"
    - "Determine Draconis gear"
  short_term:
    - "Build structured RAID farming/node data"
  long_term: []
  completed:
    - "Predator mastery error identified and corrected"
    - "Broadmaw fusion tree documented"
    - "Rhazin fusion tree documented"
    - "RAID Campaign structure documented"
  abandoned: []

decisions:
  - decision: "Do not use Cycle of Violence in Predator mastery recommendations"
    reason: "User explicitly stated Predator does not have Cycle of Violence"
    status: "HISTORICAL/CORRECTED"

  - decision: "Ronda is potentially worth taking to 6-star if actively used"
    reason: "Higher stats, Banner access, damage and utility"
    status: "RECOMMENDED; implementation not confirmed"

  - decision: "Prefer a RAID-specific campaign Node object over overloading the SWGOH Node object"
    reason: "RAID has location, stage, and difficulty dimensions"
    status: "RECOMMENDED; implementation not confirmed"

  - decision: "Use a Capacity relationship between Game Character and RAID farming nodes"
    reason: "Track farmable character acquisition/capacity"
    status: "RECOMMENDED; implementation not confirmed"

recommendations:
  - recommendation: "Predator offensive mastery build"
    status: "RECOMMENDED historically"
    reason: "Damage-focused build"

  - recommendation: "Ronda to 6-star if used"
    status: "RECOMMENDED historically"
    reason: "Improved stats, Banner slot, damage and utility"

  - recommendation: "Draconis Speed + HP/support build"
    status: "RECOMMENDED historically"
    reason: "Support/survivability-oriented role"

  - recommendation: "Shield + Speed for Draconis"
    status: "RECOMMENDED historically"
    reason: "Support utility and survivability"

rejected_strategies:
  - strategy: "Use Cycle of Violence for Predator"
    reason: "User explicitly corrected that Predator does not have it"
  - strategy: "Force RAID and SWGOH campaign nodes into a single increasingly complex Node model"
    reason: "RAID campaign structure introduces location and difficulty dimensions"
    status: "RECOMMENDED against, not confirmed formally rejected"

preferences:
  - preference: "Champion-specific mastery recommendations must account for the actual masteries available to that champion"
    evidence: "User corrected the Predator Cycle of Violence recommendation"

uncertainties:
  - item: "Champion ownership is not established for any champion in this conversation"
  - item: "Ronda's actual rank/6-star status is unknown"
  - item: "Broadmaw completion status is unknown"
  - item: "Rhazin completion status is unknown"
  - item: "Current fusion component inventory is unknown"
  - item: "RAID Node/Capacity schema implementation is unknown"
  - item: "Rhazin campaign farming claims need verification"
  - item: "Current Predator mastery setup is unknown"
  - item: "Current Draconis build is unknown"
  - item: "Current RAID mechanics may differ from historical recommendations"

tools:
  - tool: "HellHades"
    purpose: "Historical champion, fusion, artifact and build references"
  - tool: "AyumiLove"
    purpose: "Historical champion, mastery, skill and artifact references"
  - tool: "RaidNinja"
    purpose: "Historical Predator build/mastery references"
  - tool: "Inteleria"
    purpose: "Historical mastery and artifact information"
  - tool: "Plarium/RAID Support"
    purpose: "Historical fusion rules"
  - tool: "Reddit"
    purpose: "Historical community discussion"

end_state:
  current_team: "NONE"
  current_goal: "Latest substantive topic was Draconis gear recommendations"
  current_priority: "No account-wide priority established"
  next_action: "Reconcile historical recommendations with current roster, current RAID mechanics, and current database implementation"
```

**Archival note:** The most important thing for Claude Cowork is to preserve the distinction between **facts supplied by you**, **recommendations made by the previous assistant**, and **things actually implemented/tested**. In this conversation, there is surprisingly little confirmed account-state information; most of the useful durable knowledge is the **Predator correction, fusion trees, campaign data-model discussion, and the historical Ronda/Draconis recommendations**.
