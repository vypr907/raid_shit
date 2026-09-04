---
tags: [history, archive]
---

# Historical Knowledge Archive

> [!info] What this is
> This note merges 21 historical ChatGPT conversations (migrated from a prior RAID project, roughly May 2025 - Aug 2026) plus this vault's own Aug 28, 2026 roster export into one coherent history and current-state picture. It is **not** a folder of summaries — contradictions were reconciled with **later conversations weighted more heavily**, and champion ownership was cross-checked against the actual `01 Champions/` roster. Two conversations referenced in the source material could not be located in the provided export and are logged as gaps at the bottom: a "best blessing for Skeletor" discussion, and the full historical Lizardmen/Dwarves Faction Wars team picks.
>
> A parallel dev side-project (`raid_roster`, a Flask roster-tracker web app) is **not** RAID game history — see [[../06 Dev Projects/raid_roster status|raid_roster status]].

---

## 1. Current State (as of Aug 31, 2026 — the most recent conversation)

This is the authoritative "where things stand" snapshot. It comes from the single most recent conversation (Aug 28-31, 2026), which is also the same date as this vault's champion CSV export — so champion stats elsewhere in this vault and the facts below describe the same moment.

### Priorities (user-stated ranking)
1. **Clan Boss** — #1, by a wide margin
2. **Ice Golem** — #2
3. **Fire Knight** — #3
4. Everything else (Hydra, Doom Tower, Cursed City, Sintranos) is lower priority; **Arena is explicitly low priority** — "I really only do it for quest/events."
5. Long-term: wants to collect all champions, but **account strength takes priority over collecting or keeping favorites**.

### Progression snapshot (Aug 28, 2026)
| Content | Status |
|---|---|
| Clan Boss | Nightmare **unlocked**, but current team not strong enough to use it. Farming Brutal at ~7M dmg/key, 2 keys/day. |
| Hydra | Normal, **cannot clear it**, no chest yet. ~1M damage across 3 keys. Deliberately deprioritized until PvE foundation is stronger. |
| Dragon's Lair | Stage 17, best time 3:03, 98 turns. |
| Fire Knight | Stage 12, best time 1:49, 40 turns. |
| Spider's Den | Stage 13, best time 3:40, 92 turns. |
| Ice Golem's Peak | Stage 15, best time 2:38, 85 turns. |
| Doom Tower | Normal difficulty. |
| Cursed City | Not attempted. |
| Sintranos | Not attempted. |
| Arena | Low priority — only for quests/events. |

### Current team (Clan Boss, Brutal)
**Alice the Wanderer (lead) / Kael / Predator / Miscreated Monster / Runekeeper Dazdurk** — ~7M dmg/key. This is judged well below what the roster can realistically produce; the account has several specialized Clan Boss champions sitting unbuilt.

### Open investigation — Nightmare Clan Boss "Unkillable" (UNRESOLVED, next priority)
The most recent conversation was mid-investigation of an Alsgor Crimsonhorn-anchored Unkillable-style Nightmare team, using the DeadwoodJedi Clan Boss calculator:

- **First calculator test (TESTED, not validated):** Alsgor Crimsonhorn (230 SPD) / Torturehelm (187 SPD) / Corvis the Corruptor (160 SPD) / Anax (160 SPD) / Marked (~160 SPD), Nightmare/Void. The rotation looked coherent, but **Marked took the Clan Boss stun instead of the intended target, Torturehelm** — so the composition is not validated.
- **Planned second test (NOT YET RUN as of the last conversation):** swap Anax → Hotatsu (~159-160 SPD), keeping Alsgor 230 / Torturehelm 187 / Corvis 160 / Marked 160, to isolate whether the defensive rotation (stun landing on Torturehelm) works without Anax's extra-turn mechanics complicating it.
- **Explicit standing instruction: do not book Alsgor, do not 6★ anyone, do not spend the 42 gems, and do not do a major gear rebuild until this composition is calculator-validated.** Only 5 Legendary books are available — too scarce to risk on an unvalidated tune.
- Steven confirmed (Sept 2, 2026) this is **still unresolved** — the second test has not been run. This remains the single most important open thread in the account.
- Champions confirmed **NOT** owned that a classic Unkillable build normally wants: Doompriest, Maneater, Demytha, Seeker, Skullcrusher, Warcaster, Roshcard the Tower, Emic Trunkheart, Sir Nicholas, Helicath, Godseeker Aniri, Duedan the Runic, Renegade, Kymar, Nia. Only **Pain Keeper** is owned from that traditional candidate list, and he was set aside from the first test in favor of the Alsgor/Torturehelm approach (not rejected — just not part of the current experiment).

### Resource snapshot (Aug 28, 2026)
Silver 7.69M · Energy 660 · Gems 42 · Rare books 2 · Epic books 3 · **Legendary books 5** (scarce — see above) · Rank-5 chickens 0 · Rank-4 chickens 1 · Ancient shards 13 · Void shards 6 · Primal shards 6 · Sacred shards 4 · Brews: 46 Magic / 131 Force / 30 Spirit / 110 Void.

### Player philosophy / standing preferences
- **Auto-compatibility matters** — "almost everything needs to work on Auto." Manual-only strategies are undesirable.
- **Willing to rebuild, but only for substantial gains** — not interested in marginal tweaks.
- **Prefers the stronger long-term investment over the cheaper one**, even at higher resource cost.
- **Wants a strict, sequential roadmap** — "do this → spend these resources → build this → don't build this → then the next milestone" — not just a champion tier list.
- **Likes the promo champions** (Alice the Wanderer, Ronda, Predator, Ezio Auditore) but explicitly said account strength comes first: "I don't care if the account gets stronger first" [than keeping them in top teams].
- **Masteries: saves gems, then buys masteries** rather than farming Minotaur's Labyrinth for mastery scrolls. Only Predator, Ezio, and Fellhound have fully-maxed masteries as of Aug 2026.
- **No gear-export capability** — neither RSL Helper nor RSL X-Tender exports the artifact inventory, so builds have to be reasoned about from known champion stats, not a full gear database.
- Wants recommendations grounded in the **actual owned/built roster**, not generic tier lists or theoretical "best-in-game" comps — repeatedly corrected recommendations that assumed ownership or build-readiness that wasn't there.
- Wants event/tournament optimization to target the **actual scoring mechanic** (e.g., "least turns" for Turn Attack tournaments, not energy efficiency — this was corrected more than once across different conversations).
- Proposed champion classification system (not yet adopted, worth revisiting): 🔴 BUILD · 🟠 KEEP/FUTURE BUILD · 🟡 FUSION/GUARANTEE/EVENT HOLD · 🟢 FACTION GUARDIAN · ⚪ SAFE FOOD · 🔵 PROMO/COLLECTOR — proposed specifically to solve the recurring uncertainty around duplicates, Faction Guardians, and fusion requirements.

---

## 2. Chronological History

Ordered by actual conversation date (not the order the source files were numbered in — the file numbering was topical, not chronological).

### May 30, 2025 — Roster-recognition tooling idea (pre-dates gameplay history)
Explored building a CNN/image-recognition pipeline (screenshot → detect champion icons → classify → export to Sheets/AppSheet) to solve collection tracking on a Mac (no RSL Helper/HellHades Optimizer access, both Windows-only). Considered and rejected: OCR (reads text, not icons), generic cloud vision APIs (no RAID-specific mapping), fully manual entry. Settled on a custom CNN (TensorFlow/Keras or PyTorch), OpenCV for screenshot cropping, Google Colab for free training compute. **Never built** — no dataset, model, or pipeline exists from this conversation. General keep/fodder framework proposed but not formalized: Legendary = keep, Epic = keep/evaluate, Rare = evaluate individually, Uncommon/Common = generally fodder.

### Sept 3-8, 2025 — F2P foundations, Dragon team, and the software-project decision
Established as F2P from the start — resource efficiency is a running theme throughout the entire history. Confirmed roster at this point: Kael, High Khatun, Valerie, Warmaiden, Apothecary, Pain Keeper (early Clan Boss candidates, team never finalized this conversation), plus Alice the Wanderer, Ronda, Runekeeper Dazdurk, Shaman, Fellhound, Elhain, Michelangelo (the "strong" tier). Dragon's Lair team **tested**: Alice the Wanderer / Kael / Ronda / Elhain / Runekeeper — Stage 13, best time 1:12, 30 turns minimum. Corrected the assistant's assumption that a *regular* Dragon Tournament should be turn-optimized — "no, it's a regular tourney," meaning farm the highest reliable stage instead. High Khatun built Speed-first for Ice Golem. This is also where the **raid_roster software project** began: chose Flask over Streamlit specifically for DevOps portfolio value, defined the RAID progression schema (Level 1-60/Rank 1-6/Awoken 1-6/Perfect 1-6), and scoped an AWS architecture (RDS Postgres, ECS/Fargate, Lambda, S3, IAM, CloudWatch, CI/CD) — see [[../06 Dev Projects/raid_roster status|raid_roster status]] for what actually got built.

### Sept 8-16, 2025 — Dungeon core established, Turn Attack rules corrected, Banner Lords FW planned
Confirmed developed core: **Alice the Wanderer, Kael, Ronda, Runekeeper Dazdurk, Fellhound** (plus Elhain and Shaman as secondary). Concrete stat snapshot at this point: Alice 118 SPD (flagged as a major weakness — later fixed, see Nov 2025 below), Kael 69 ACC (flagged low), Runekeeper 181 SPD (fastest core member), Ronda 6-piece Savage at level 16 but Crit Rate not yet optimized. **Tested**: Ice Golem Stage 14 cleared with the core team, but **only Alice survived** — used as the reason to farm Stage 13-14 rather than force Stage 16+. Fire Knight turn-count history recorded: Stages 7-12 took 7/17/32/28/36/40 turns; Stage 10 flagged as the practical farming target. Sharp correction from Steven: "NO! in a Turn Attack tournament, you want to clear in as few turns as possible!" — the assistant had it backwards. Also corrected: Shredder's Wrath is its **own** dungeon/event, not a Dungeon Divers-style tournament — Spider farming doesn't double-dip into it. Banner Lords Faction Wars team **planned** (not tested, 3 of 5 members explicitly too undeveloped at the time): Michelangelo / Ronda / Oathbound / Lady Annabelle / Valerie, in that investment priority order; Lordly Legionary and Steadfast Marshal noted as alternates. Sept 11 resource snapshot: 442 energy, 1.2M silver.

### Sept 9, 2025 - Dec 30, 2025 — Alice's speed fixed, Ice Golem core validated, Clan Boss roster expanded
Alice the Wanderer's Speed problem (118 SPD) was addressed with a goal of >150 SPD, using heavy Savage gear including a 6★ Legendary Savage HP% boots piece later considered for transfer to Fellhound once Michelangelo's 6★ Speed boots became available as Alice's replacement. High Khatun's actual kit was corrected on the record: **Shamanic Lightning, Imperial Grace, Rally the Horde** — she does *not* have a "Tailwind" ability as the assistant once claimed. Compared at 192 SPD, her aura was judged not worth losing Alice's ATK aura for min-turn farming, so **Alice stayed leader**. Locked in **Alice / Kael / Ronda** as the fixed Ice Golem/Spider/Fire Knight core, with **Predator + Miscreated Monster** filling the remaining two slots (recommended, not confirmed tested in this conversation). Clan Boss test data: Leminisi 4.89M vs Shaman 6.41M in the support slot — **Shaman preferred**. Fellhound's target build (6,200 ATK+DEF / 100% CR / 105 SPD / 225% CD) was set with books already maxed. Orc Faction Wars roster identified as broad but mostly unbuilt (Torturehelm, Galek, Raider, Pigsticker, and ~10 others). Champion Training event guidance: prioritize 4★ food to level 39/40 and rank up during the event window (over 3★ food).

### Oct 9-16, 2025 — Gem priority, Spider farming stage, and a costly mislabeling ("Chimera")
Gem-spending priority established: **masteries → energy refills → Gem Mine → Sparring Pit**; advised against gems on summons/market shards/most shop offers. Spider's Den farming data: Stage 9 0:53/12t, Stage 10 1:02/18t, Stage 11 4:20/90t, Stage 12 3:35/68t (highest completable at the time) — **Stage 10 recommended for event/accessory farming** on efficiency grounds. A 6-man Hydra team was recommended (Runekeeper Dazdurk / Kael / Ronda / High Khatun / Fellhound / Alice) but never tested. **Important error to not repeat:** when asked about a "Chimera" team, the assistant incorrectly treated "Chimera" as synonymous with Clan Boss/Demon Lord and produced an invalid 6-champion "Clan Boss" team — Clan Boss/Demon Lord is a 5-champion fight; that 6-man composition is not a valid reference for CB planning.

### Oct 31, 2025 — Mordecai/Magnarr summons and the Spider core that led to Miscreated Monster's addition
Steven summoned six new champions in one pull: Goremask, Sentinel, **Mordecai**, **Magnarr**, Petrifya Rockroot, Gloril Brutebane. Asked for a Spider's Den team built specifically around Mordecai (AoE HP Burn) and Magnarr (HP-based AoE nuker). Initial proposal used Runekeeper Dazdurk/Kael/Alice/Valerie/Fellhound as filler (ownership of those wasn't actually re-confirmed in this exchange) — then Steven volunteered "I do have a Miscreated Monster," which **changed the recommended core to Mordecai + Magnarr + Miscreated Monster**, with Runekeeper and Kael as the (unverified-here) 4th/5th. Strategy: open with Mordecai's A3 manually, use MM for control/shields, keep spiderlings alive to sustain the HP Burn tick. **Never tested in this conversation.** *(Note: Petrifya Rockroot does not appear in the current Aug 2026 roster export — likely fed or dismissed since; flagged as a gap, not a contradiction.)*

### Nov 10-13, 2025 — Clan Boss rebuilt around Alice as lead, Warmaiden brought in
Baseline Clan Boss result **recorded**: 4.5-6M damage/key on Brutal with Alice/Kael/Fellhound/Ronda/Runekeeper. The assistant initially proposed benching Alice for High Khatun as lead — Steven explicitly rejected this: he wanted **Alice the Wanderer as Clan Boss lead**, corrected the assistant's wrong claim that her kit had an ATK Down effect, and supplied her authoritative kit and stats himself (Level 60/Rank 6/Ascension 6/Perfect Soul 5, Brimstone blessing, 173 SPD, 4,150 ATK, 2,935 DEF, 41,299 HP, 205 ACC, 80% CR, 145% CD, 149 RES — this matches the current vault export almost exactly, confirming it's been stable since). Final requested composition: **Alice (lead) / Kael / Warmaiden / Ronda / Runekeeper**, replacing Fellhound with the un-geared Warmaiden for Decrease DEF. At the time: Warmaiden only 97 SPD (major dev target, goal ~160-170), Ronda only 119 SPD (goal ~160-168), Kael fully booked at 159 SPD, Runekeeper almost fully booked at 181 SPD. Tome allocation plan: 5 Rare tomes → Warmaiden, 4 Epic tomes → Runekeeper, future Epic tomes saved for Pain Keeper rather than partially booking him. This proposed 181/173/165/162/160 speed ordering was **never calculator-validated** — treat as a loose plan, not a proven tune. Pain Keeper and Maneater were floated as a future "unkillable" combo; Maneater is **not owned**.

### Nov 3, 2025 - Feb 25, 2026 — Long-running roster/dungeon-team thread (spans the widest date range)
Miscreated Monster reached **Rank 6 on Nov 24, 2025** — a major milestone that reshaped several team recommendations. Jan 2026: unlocked Predator and Xenomorph together with a full 6★ Instinct gear set; Instinct was given to **Predator, not Ronda** (better DEF-ignore synergy per the assistant, unverified mechanically). Predator's kit was fully supplied by Steven (Legendary Lizardmen: Wrist Blades/Smart Disc/Combistick Throw/Yautja Cloak, HP-based AoE double-hit, MAX HP destruction, Veil/Perfect Veil, Evasion, +35% Ally HP aura) — treat this as the authoritative source for his kit, not later assistant guesses. **Alsgor Crimsonhorn** and **Tainix Hateflower** unlocked Dec 19, 2025; Steven corrected the assistant's misclassification — Alsgor is a **Legendary Barbarian**, not Ogryn. Alsgor became a recurring high-priority defensive/support pick across Dragon, Hydra, and Doom Tower recommendations throughout this period (and, per the Aug 2026 conversation above, ultimately became the anchor of the current Nightmare Clan Boss investigation). Recommended team snapshots from this period (**mostly untested in-conversation**): Dragon = Miscreated Monster/Kael/Predator/Runekeeper/Alsgor; Spider = Miscreated Monster/Kael/Ronda/Runekeeper/Alice; Hydra (6-man) = Alsgor/Predator/Miscreated Monster/Runekeeper/Kael/Tainix; Phantom Shogun's Grove = Miscreated Monster/Predator/Alsgor/Kael/Runekeeper. Fusion trees researched but not confirmed completed: Broadmaw = Arbalester + Rockbeast + Huntress + Bloodhorn; Rhazin Scarhide = Lich + Erinyes + Bloodfeather + Torturehelm (each Epic itself built from 4 named Rares — full tree preserved in the raw source if ever needed). Rare-book priority order settled: **Apothecary > Warmaiden** > (save books) > Galek/Skink/Pigsticker. Apothecary's 2★ blessing recommendation was **Phantom Touch** (selection not confirmed). Tag Team Bazaar priority: Drexthar Bloodtwin (not owned) > Rare Skill Tomes > Ancient Shards, skipping Huntress/Bloodhorn. This conversation's final open question (Feb 25, 2026) was the Reliquary Tender/Apothecary blessing/book decision.

### Jan 9, 2026 — Broadmaw pull, general assessment only
Pulled Broadmaw from a shard. Verdict: **keep him** — useful for revive/support/TM buffs in Faction Wars, dungeon progression, and Doom Tower/Secret Rooms, but "not a standout late-game champion" and limited in Arena. No build, team, or resource investment was ever attached to him in this conversation; the Aug 2026 vault snapshot still shows him lightly developed (Rank 4/Level 40, no blessing).

### Jan 15, 2026 — Ezio Auditore gear framework (name-collision resolved)
First message was answered as if about Assassin's Creed's Ezio before Steven clarified: **"the new RAID character, Legendary Sacred Order Attacker."** Recommended gear direction: Relentless as the general-purpose set, Savage+Cruel or Lethal as raw-damage alternatives, with the explicit principle **"stats > sets every time."** Stat priority: 100% Crit Rate → Crit Damage → ATK, with Speed/Accuracy content-dependent. Suggested PvE targets (~180-220 SPD, ~250-300% CD, 4.5k+ ATK, ~230 ACC) were never tested against his actual gear in this conversation.

### Jan 22-27, 2026 — Turn Attack optimization and benching Ezio for gear reasons
Re-confirmed the "fewest turns wins" objective for Turn Attack tournaments. **Ezio Auditore was explicitly benched from Fire Knight** for being under-geared at the time (3,068 ATK / 108 SPD / 65% CR / 88% CD) — Predator was used in his place. Recommended: save the Mythical skill tome rather than spend it on Ezio (Steven had zero Mythical champions at the time); improve him through gear instead. Final Fire Knight recommendation from this conversation: **Ronda / Fellhound / Kael / Alice / Predator**. Established that the in-game Team Setup AI only supports Round 1/2/3 presets — there is no shield-state-conditional toggle, which matters for any Fire Knight shield-break sequencing plan.

### Dec 19, 2025 - Feb 2, 2026 — Fusion research and a mastery correction for Predator
Steven corrected the assistant: **"he doesnt have cycle of violence"** — Predator's mastery build should not include Cycle of Violence; the corrected path is Deadly Precision/Keen Strike/Shield Breaker/Single Out/Ruthless Ambush/Bring It Down/Methodical/Kill Streak/Helmsmasher (with Warmaster as a PvE/boss alternative). Ronda's 6★ was judged worthwhile "if she'll actually be used." Full Broadmaw and Rhazin Scarhide fusion trees were documented here (see Nov 2025 entry above for the components) — completion not confirmed. A `RAID_Node`/`Capacity` database-object design was proposed for tracking farmable locations against a character, separate from an existing SWGOH-oriented schema — proposed only, not confirmed built (this predates and is distinct from the later `raid_roster` Flask project).

### Feb 9, 2026 — Relic placement and Ice Golem tournament math
Steven corrected three relic mechanics the assistant had wrong — treat these as authoritative: **Unholy Grail** = wearer deals 2% more damage to any debuffed target; **Hatter's Reserve** = 5% less damage taken from lower-ATK enemies, 5% more damage to lower-MAX-HP enemies; **Wand of Submission** = 25% chance to reflect Stun/Sleep/Fear/True Fear/Freeze/Provoke/Petrification/Sheep back at the caster. Final recommended (untested) placement: Alice → Unholy Grail (kept), Runekeeper Dazdurk → Hatter's Reserve (moved off Ronda), Morag Bronzelock → Wand of Submission. Steven pushed back that Fellhound — his main Campaign Farmer — might suit Hatter's Reserve better than Runekeeper; this was never resolved. Pierce Defenses recommended as the Hatter's Reserve triangle gem (Steven had no square gems at the time). Ice Golem Stage 10 recommended over Stage 13 for tournament-point efficiency (≈50.8 vs ≈16.2 pts/min under an assumed-equal artifact-rank-probability model).

### Feb 25, 2026 — Fire Knight Stage 12 rebuild toward Stage 20+
Recorded baseline with the original team (Alice-lead/Ronda/Kael/Predator/Fellhound): Stage 9 1:00/32t, Stage 10 0:39/14t, Stage 11 1:34/36t, Stage 12 1:49/40t. Steven supplied his full 28-champion "most-built to least-built" ranking (preserved in the raw source if needed for future reference). Central decision, still only partially resolved: **Miscreated Monster vs. Ronda** for the 5th Fire Knight slot — MM recommended for pushing Stage 20+ (survivability/wave control/shields), Ronda kept for raw damage/faster farming once stable. Final recommended Stage 20+ team: **High Khatun / Warmaiden / Apothecary / Scyl of the Drakes / Miscreated Monster** (Ronda as an alternate 5th). Detailed stat targets were set for High Khatun, Apothecary, Warmaiden, Scyl, and MM at both Stage 12 and Stage 20+ tiers (see the raw conversation for exact numbers if regearing). Armiger, Coldheart, Alure, and Deacon Armstrong were discussed as theoretical upgrades — **none were owned at this point** (Alure and Deacon were later pulled March 4, 2026 — see below).

### March 2, 2026 — Champion Training Tournament efficiency (generic, no roster specifics)
F2P point-maximization guide: rank-ups (especially a 6★) are the biggest point source; farm 12-3 Brutal for XP+Silver with 1 farmer + 3 food champions; stockpile Mystery Shards and food pre-event; use 1-3 brews only to accelerate early levels, finish leveling via campaign XP; **do not spend Legendary Books purely for tournament points**; double-dip with Dungeon Divers/Artifact Enhancement/CvC when they overlap. No champions were named in this conversation.

### March 4, 2026 — Alure and Deacon Armstrong pulled; Fire Knight and Clan Boss both reworked
Two significant pulls: **Alure** and **Deacon Armstrong**, plus two more copies of Enda Moonbeam. Alure was earmarked for Fire Knight Turn Meter control (target 220+ SPD, ~250 ACC, 100% CR); Deacon for general speed/TM/AoE DEF-Down/Leech utility (target 230+ SPD, ~250 ACC). Explicit and important standing caveat from Steven: **"my 'current' teams are my most built characters in general, most of my other characters have not been built up, other than regular leveling"** — i.e., what's currently fielded is not the same as what's optimal. Fire Knight direction shifted away from the original support-heavy goal team (High Khatun/Warmaiden/Apothecary/Scyl/Miscreated Monster) toward a mechanic-specialized team: **Deacon (lead) / Alure / Fellhound / Ronda / Scyl** (recommended, untested), with Ruella/Visix the Unbowed floated as a more control-focused alternative once further developed. Clan Boss direction: two theoretical comps compared — a "survival" build (Corvis/Rearguard Sergeant/Kunoichi/Hotatsu/Alsgor) vs. a "damage" build (Corvis/Rearguard Sergeant/Anax/Hotatsu/Deacon) — the **damage build was favored** at the time (gear still developing, wanted immediate output), but this was explicitly theoretical and never empirically compared. *(By Aug 2026, the Clan Boss direction had evolved again toward the Alsgor/Torturehelm Unkillable approach described in Section 1 — treat that as superseding this March comparison.)*

### March 11, 2026 — Magic Keep Stage 14, leader-aura tradeoff
Confirmed **current** Magic Keep team at Stage 14: **High Khatun / Alice / Kael / Ronda / Leminisi the Gold-wing**. Central open question: keep High Khatun as leader for her +19% Ally SPD aura, or switch to Alice for +30% Ally ATK? Fellhound was proposed to replace High Khatun; Predator, Morag Bronzelock, and Ezio were also floated as possible swaps for Leminisi or High Khatun. The conversation's final lean was toward **Alice as leader + Alice/Kael/Ronda/Fellhound/Leminisi**, but **this was never tested** — Stage 14 remains the last confirmed clear, and no Stage 15 failure was ever diagnosed.

### April 8-13, 2026 — Tainted Demon Lord (Clan Boss) and a hard-restricted Stage V
Steven clarified that his strongest theoretical Clan Boss core (**Corvis the Corruptor / Rearguard Sergeant / Hotatsu / Anax / Deacon Armstrong**) was owned but **completely unbuilt** at the time — "none of them are leveled/geared up at all right now." Practical baseline **tested**: Alice/Predator/Ronda/Kael/Miscreated Monster = **~3.5M damage**. Second-string proposal (Ronda → Apothecary, for more speed/healing/Kael uptime) was **never tested**. Separately, a severely restricted Stage V (Magic/Void affinity only, Barbarians/Ogryn/Demonspawn/Knights Revenant factions only) forced a weaker lineup — **Alure / Dervish / Scyl / Fellhound / Miscreated Monster**, which was actually **tested and produced only 177k damage against a 500k requirement** — a 2.82x shortfall that was never closed in this conversation. This remains an unresolved problem unless it's since been solved outside these 21 conversations.

### June 12, 2026 - Aug 28, 2026 — Duplicate management, then back to Clan Boss planning
On June 12, Steven supplied a large duplicate-champion list (Boughsmith Flannan, Enda Moonbeam ×2+, Riscarm, Pathfinder Cait, Castigator, Avir the Alchemage, Warmaiden, Diabolist, Spirithost, Heiress, and ~50 more lower-priority rares) and got a keep/food framework: keep one copy of anything with Faction Wars depth or niche utility, use Warmaiden duplicates specifically for skill-booking rather than feeding them, treat Enda Moonbeam (an Epic) with more caution than ordinary rare duplicates, and food the rest once faction/book needs are covered. **No confirmation this cleanup was ever actually carried out.** By Aug 28, conversation shifted back to Clan Boss: confirmed Nightmare unlocked but the team too weak, confirmed **only Pain Keeper** owned from a list of classic Clan Boss candidates, and confirmed access to the DeadwoodJedi calculator — directly setting up the Aug 28-31 conversation covered in Section 1. A separate mention in this conversation of a **"best blessing for Skeletor" discussion is not among the 21 conversations available** — its conclusion is a gap (see Section 6).

---

## 3. Team Quick-Reference by Content Type

Cross-cut view of how each team evolved. "Latest" = the most recent version across all 21 conversations; check Section 2 for the reasoning and test results behind each change.

| Content | Team history (oldest → latest) | Latest status |
|---|---|---|
| **Clan Boss** | Kael/High Khatun/Valerie/Warmaiden/Apothecary/Pain Keeper (unresolved, Sep'25) → Alice/Kael/Fellhound/Ronda/Runekeeper, 4.5-6M (Nov'25) → Alice/Kael/Warmaiden/Ronda/Runekeeper, untested tune (Nov'25) → Alice/Kael/Predator/MM/Runekeeper, ~7M Brutal (current fielded team) → **Alsgor/Torturehelm/Corvis/Marked (+Anax or Hotatsu), Nightmare, Unkillable concept** | **UNRESOLVED** — 2nd calculator test (Hotatsu swap) not yet run |
| **Fire Knight** | Alice/Ronda/Kael/Predator/Fellhound, Stage 12 1:49/40t (tested, Feb'26) → High Khatun/Warmaiden/Apothecary/Scyl/MM, Stage 20+ target (recommended, untested) → Deacon(lead)/Alure/Fellhound/Ronda/Scyl (recommended, Mar'26, untested) | Stage 12 is the last confirmed clear; no later result recorded |
| **Ice Golem** | Alice/Kael/Ronda/Runekeeper/Fellhound, Stage 14 clear but only Alice survived (tested, Sep'25) → Alice/Kael/Ronda/Predator/MM (recommended core, Dec'25) | Stage 15, 2:38, 85 turns (per Aug'26 snapshot) — current team composition for this result not explicitly restated in the Aug'26 conversation |
| **Spider's Den** | Alice/Kael/Fellhound/Runekeeper/Ronda (stated, Jan'26) → Miscreated Monster/Kael/Ronda/Runekeeper/Alice (recommended swap, untested) → Mordecai/Magnarr/Miscreated Monster core (recommended, Oct'25, untested) | Stage 13, 3:40, 92 turns (Aug'26 snapshot) |
| **Dragon's Lair** | Alice/Kael/Ronda/Elhain/Runekeeper, Stage 13 1:12/30t (tested, Sep'25) → Ronda/MM/Alice/Predator/Kael (stated current, Jan'26) → MM/Kael/Predator/Runekeeper/Alsgor (recommended, untested) | Stage 17, 3:03, 98 turns (Aug'26 snapshot) |
| **Hydra** | Not clearing Normal; 6-man recommended (Runekeeper/Kael/Ronda/High Khatun/Fellhound/Alice, Oct'25, untested) → Alsgor/Predator/MM/Runekeeper/Kael/Tainix (recommended, untested) | Normal, no chest, ~1M dmg/3 keys — deliberately deprioritized |
| **Magic Keep** | High Khatun/Alice/Kael/Ronda/Leminisi, Stage 14 (tested, Mar'26) → Alice(lead)/Kael/Ronda/Fellhound/Leminisi (recommended, untested) | Stage 14 is the last confirmed clear |
| **Banner Lords Faction Wars** | Michelangelo/Ronda/Oathbound/Lady Annabelle/Valerie (planned, Sep'25 — 3 of 5 members explicitly under-built at the time) | Never confirmed tested; investment order was Michelangelo → Ronda → Oathbound → Lady Annabelle → Valerie |
| **Arena** | Low priority throughout; no team ever finalized or tested | Only used for quests/events, per explicit preference |
| **Restricted Stage V (dungeon)** | Alure/Dervish/Scyl/Fellhound/Miscreated Monster — tested, **177k vs 500k required** (Apr'26) | Unresolved 2.82x shortfall; no later attempt recorded |

---

## 4. Rejected / Failed Strategies (consolidated)

- **Treating "Chimera" as another name for Clan Boss/Demon Lord** — wrong; produced an invalid 6-champion "Clan Boss" team. Clan Boss is a 5-champion fight.
- **Optimizing Turn Attack tournaments for energy efficiency instead of turn count** — corrected twice, independently, in different conversations. The scoring metric is turns, full stop.
- **Assuming a champion is owned because it was previously suggested or discussed** — this specific failure mode recurred across nearly every conversation (Doompriest/Maneater/etc. weren't owned; Apothecary's ownership was assumed at one point without confirmation; theoretical Clan Boss cores were assumed buildable when they were owned but completely unbuilt). Always check the actual roster first.
- **Keeping the existing Clan Boss/Fire Knight team just because it already exists** — repeatedly overridden by Steven's explicit willingness to rebuild for a real improvement ("even if it means starting over").
- **Automatically feeding every duplicate champion** — rejected; duplicates can have Faction Guardian value, skill-book value (Warmaiden), or Epic-rarity value (Enda Moonbeam) that a blanket "keep 1, food the rest" rule would waste.
- **Forcing Ice Golem past Stage 14-15 before survivability caught up** — the Stage 14 clear left only one champion alive; pushing higher without fixing durability first was explicitly discouraged.
- **Giving High Khatun the Clan Boss/Fire Knight lead slot over Alice** — tried, but Steven overrode it each time in favor of Alice, both for her ATK aura value and because he specifically wanted her as lead.
- **Committing Alsgor's books/6★ before the Unkillable Clan Boss tune is calculator-validated** — explicit standing rule, still in force as of Sept 2026 (only 5 Legendary books available).
- **Relying on assistant-supplied champion mechanics without user verification** — happened repeatedly (Alice's kit, High Khatun's skills, Predator's masteries, Alsgor's faction, three relic descriptions) and was corrected by Steven's own authoritative statements each time. Treat any AI-generated mechanic claim in the raw source conversations as unverified unless a direct Steven quote confirms it.

---

## 5. Tools & External Resources

- **DeadwoodJedi Clan Boss Calculator** — primary tool for validating Clan Boss speed tunes/turn order/stun targeting. Confirmed access. Central to the current unresolved Alsgor/Torturehelm investigation.
- **RSL Helper** — Windows-oriented roster export/import tool; source of this vault's `01 Champions/` notes (Aug 28, 2026 export). No gear/artifact export capability.
- **RSL X-Tender** — similar role to RSL Helper (pull roster/gear, optimize individual champions); also no usable gear-inventory export.
- **HellHades** and **AyumiLove** — referenced for champion mechanics/build research throughout; several claims sourced from these (or from assistant paraphrase of them) turned out to need correction from Steven directly, so treat them as a starting point, not gospel.

---

## 6. Known Gaps / Needs Verification

- **Skeletor's best-blessing conversation** is referenced (as having happened) in the June-Aug 2026 conversation, but is not among the 21 conversations provided in this migration. If Steven has that answer, it should be added here.
- **Full historical Lizardmen and Dwarves Faction Wars team picks** (from the Nov 2025-Feb 2026 conversation) were requested by the assistant but the responses containing the final 5-man teams were not preserved in that conversation's extraction.
- **Petrifya Rockroot** was confirmed owned on Oct 31, 2025, but does not appear in the Aug 28, 2026 roster export — most likely fed or dismissed since as a low-priority rare; not treated as a contradiction.
- **Many specific champion-mechanic claims** throughout the source conversations were generated by the assistant rather than stated by Steven (skill descriptions, set-bonus percentages, aura values, etc.) and were flagged in the originals as NEEDS VERIFICATION. Where Steven corrected one on the record, that correction is captured above as authoritative; anything not explicitly corrected should still be checked against current in-game tooltips before being relied on for a real build decision.
- **Whether several "recommended, not tested" teams were ever actually built** (the Fire Knight Deacon/Alure/Fellhound/Ronda/Scyl comp, the Stage 20+ MM-based Fire Knight team, the Hydra 6-man, the Banner Lords FW team, the restricted Stage V fix) is unknown — the current Progress notes in this vault reflect only what's confirmed, and should be filled in as these get resolved.
