---
team_name: "Clan Boss - Nightmare Unkillable (In Progress)"
purpose: "Clan Boss Nightmare - Unkillable-style composition, under active investigation"
champions:
  - "[[Alsgor Crimsonhorn]]"
  - "[[Torturehelm]]"
  - "[[Corvis the Corruptor]]"
  - "[[Marked]]"
  - "[[Anax]]"
  - "[[Hotatsu]]"
tags:
  - team
  - in-progress
---

# Clan Boss - Nightmare Unkillable (In Progress)

**Purpose:** Push from Brutal into reliable Nightmare (and eventually Ultra-Nightmare) Clan Boss farming
**Content:** Clan Boss - Nightmare

> [!warning] Status: UNRESOLVED as of Sept 4, 2026
> This is the account's #1 open priority. Rotation timing is confirmed stable (Hotatsu-swap calculator test, Sept 3). A real ungeared Nightmare CB pull (Sept 4) shows the stun rotating between multiple champions (Hotatsu, Alsgor, Torturehelm) rather than sitting on Marked - see the live-test log below. Two of the four data points still need re-verification. Do not book [[Alsgor Crimsonhorn]], 6★ anyone into this comp, or spend the 42 gems on it until that's resolved - only 5 Legendary books are available.

## Roster (first tested version)
| Slot | Champion | Role | Test speed |
|---|---|---|---|
| 1 | [[Alsgor Crimsonhorn]] | Block Damage anchor | 230 SPD |
| 2 | [[Torturehelm]] | Intended stun target (self-revive) | 187 SPD |
| 3 | [[Corvis the Corruptor]] | Poison / debuff engine | 160 SPD |
| 4 | [[Anax]] | Damage | 160 SPD |
| 5 | [[Marked]] | Block Debuffs / Increase DEF | ~160 SPD |

**Result of first test:** Rotation looked coherent/repeating, but **Marked took the Clan Boss stun instead of Torturehelm** - not validated.

## Roster (second tested version - Hotatsu swap)
| Slot | Champion | Role | Test speed |
|---|---|---|---|
| 1 | [[Alsgor Crimsonhorn]] | Block Damage anchor | 230 SPD |
| 2 | [[Torturehelm]] | Intended stun target (self-revive) | 187 SPD |
| 3 | [[Corvis the Corruptor]] | Poison / debuff engine | 160 SPD |
| 4 | [[Hotatsu]] | Damage / Decrease ATK / Leech | 159 SPD |
| 5 | [[Marked]] | Block Debuffs / Increase DEF | 160 SPD |

## Second test: Hotatsu swap - RUN Sept 3, 2026
Swapped **Anax → [[Hotatsu]]** (159 SPD) and ran the full lineup through the DeadwoodJedi Clan Boss Calculator (Nightmare, Void, boss SPD 170).

**Result:** Turn order is clean and stable - the boss cycles AOE1 → AOE2 → STUN on repeat with no breaks or desyncs across every cycle checked (0 through 8). Speed-tuning itself is solid.

**This does NOT confirm the stun lands on Torturehelm.** The calculator only shows *when* the boss uses its stun in the rotation, not *who* it targets - per DeadwoodJedi's own calculator guide, target simulation isn't built in; you're meant to manually pad a suspected target's cooldowns by +1 to model them missing a turn, which this run didn't do. See the diagnosis below for a much more likely explanation than "wrong 5th slot member."

## Live Nightmare CB test log (ungeared) - Sept 4, 2026
Ran an actual Nightmare Clan Boss pull with the second (Hotatsu) lineup at **current, ungeared stats** (not the speed-tuned targets - real SPD was ~95-99 for Corvis/Marked/Hotatsu/Torturehelm and 151 for Alsgor, all well under the 160-230 test values). Purely a stun-targeting data-gather, not a real clear attempt.

**Outcome:** Near-total wipe, as expected for ungeared champions vs. Nightmare - team dealt 60.0K damage against the boss's 652.7M HP pool. Only [[Torturehelm]] survived, at 19% HP (3,640 / 19.1K). Everyone else died.

**Stun targets, read from the battle log's per-cast tooltips (boss used A1 four times: R3, R6, R9, R12):**
| Boss cast | Target shown |
|---|---|
| R3 (Turn 9) | [[Hotatsu]] - confirmed via tooltip |
| R6 | [[Alsgor Crimsonhorn]] **and** [[Torturehelm]] - re-checked in-game (Sept 4), same result both times. Still unresolved: every source describes Crushing Force as strictly single-target, so this doesn't match documented mechanics. Best guess is a display quirk in RSL Helper's battle-log feature (confirmed newly added, undocumented anywhere yet) rather than a real double-hit - possibly related to parsing Torturehelm's self-revive passive on the same turn. Worth asking in RSL Helper's own Discord/GitHub if a definitive answer matters later; not blocking for now. |
| R9 | No champion name shown - **likely explained**: a Plarium forum moderator states the Clan Boss's stun target needs at least 16% HP remaining to be eligible. By R9, only [[Alsgor Crimsonhorn]] and [[Torturehelm]] were still alive (Corvis/Hotatsu/Marked already dead) - if both had dropped below that 16% floor at that moment (very plausible mid-wipe, ungeared), there'd be no eligible target and the cast would show nothing. Not 100% confirmed (community source, not official Plarium documentation) but fits the data. |
| R12 | [[Torturehelm]] - confirmed via tooltip |

**Key finding: Marked was not targeted at all in this run**, despite being the team's lowest-max-HP champion (4,602 HP). This is real evidence against a simple "always the lowest-max-HP champion" reading of the targeting rule. Since the actual rule (see diagnosis below) is based on lowest **remaining HP%** at the moment of the cast, not max HP, the target can rotate between champions depending on who's taken the most unhealed damage up to that point - which is consistent with Hotatsu getting hit early (R3) and Torturehelm later (R6, R12) rather than one fixed champion every time.

**Caveat:** this run was fully ungeared, so it doesn't validate the tuned rotation/timing - but the stun-targeting logic itself is HP%-based rather than speed-based, so who got hit is still meaningful data.

**Additional rule found (Sept 4, 2026):** per Plarium forum moderator commentary, a champion needs at least 16% HP remaining to be eligible as the Clan Boss's stun target at all - champions below that floor are skipped. This isn't in DeadwoodJedi's targeting-priority writeup and should be treated as community knowledge rather than confirmed official documentation, but it cleanly explains the R9 no-target result above. Net effect on the working theory: still HP%-based, just with a minimum-HP exclusion layered on top - doesn't change the core Marked-is-the-likely-target reasoning below, but explains why a near-dead team can produce "misses."

## Stun-targeting diagnosis (researched Sept 3, 2026)
Per DeadwoodJedi's [Stun Targetting](https://deadwoodjedi.com/stun-targetting/) reference, the Clan Boss picks its stun target with a priority list, first match wins:
1. Low HP / one-shot risk
2. Negative affinity vs. the boss
3. Has Increase DEF, Block Damage, Counterattack, or Steadfast active
4. Lowest HP% remaining on the team
5. Leader position

Applied to this comp against a **Void** boss:
- **Affinity (step 2) is a non-factor.** Per Plarium's official affinity doc, Void has no advantage/disadvantage relationship with Force or Magic - the Force>Magic>Spirit>Force cycle doesn't include Void. Nobody gets flagged here.
- **Step 3 doesn't reliably protect anyone either.** Checked both buffs' actual kits: Alsgor's Block Damage (Resounding Rally, A3, 6-turn cooldown, 2-turn duration) and Marked's Increase DEF (Totemic Power, A3, 6-turn cooldown, 2-turn duration) both apply to **all allies at once**, but only ~2 of every 6 turns. Most cycles nobody matches step 3, and when someone does, it's the whole team at once - not a way to single out Torturehelm as protected.
- **That pushes it to step 4: lowest HP%.** [[Marked]]'s max HP is **4,602**; [[Torturehelm]]'s is **18,731** - roughly 4x more. Under sustained Clan Boss damage, Marked is far more likely to sit at a lower HP% than Torturehelm, regardless of who's in the 5th slot.

**Working theory:** Marked took the stun in the first test because he's the squishiest champion on the team, not because of Anax specifically. The Hotatsu swap likely won't change that outcome. Options going forward:
- Significantly raise Marked's HP/DEF so he's no longer the team's HP-percentage floor, or
- Replace Marked's role with a tankier Block Debuffs/Increase DEF option, or
- Test this in an actual Nightmare Clan Boss pull rather than the calculator, since the calculator doesn't model targeting at all - this diagnosis is a strong hypothesis from game mechanics + roster stats, not yet a confirmed result.

## Gear Priorities
- Do not invest further (books/6★/gear) until validated in the DeadwoodJedi calculator.
- If validated: Alsgor needs significant booking for his Block Damage cooldown to work as intended (2-turn Block Damage on a 4-turn cooldown when fully booked, per assistant research - unverified in-game).

## Speed Tune Targets
See test speeds above. All provisional - not finalized builds.

## Notes / Results
- Champions confirmed NOT owned that a classic Unkillable team usually wants: Doompriest, Maneater, Demytha, Seeker, Skullcrusher, Warcaster, Roshcard the Tower, Emic Trunkheart, Sir Nicholas, Helicath, Godseeker Aniri, Duedan the Runic, Renegade, Kymar, Nia.
- [[Pain Keeper]] is owned but was set aside from the first test in favor of this Alsgor/Torturehelm approach - not rejected, just not part of the current experiment.
- Validation tool: DeadwoodJedi Clan Boss Calculator (confirmed available).
- Full history: [[../05 History/Historical Knowledge Archive|Historical Knowledge Archive]], Section 1.
