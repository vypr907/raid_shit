---
name: "Marked"
faction: "Barbarians"
affinity: "Magic"
rarity: "Rare"
rank: 3
level: 1
hp: 4602
atk: 210
def: 207
crit_rate: 15
crit_dmg: 52
spd: 95
acc: 27
res: 37
books_missing: 12
blessing_grade: 0
tags:
  - champion
  - "faction/Barbarians"
  - "affinity/Magic"
  - "rarity/Rare"
---

# Marked

`= this.faction` · `= this.affinity` · `= this.rarity` · Rank 3 · Level 1

![Marked](https://ayumilove.net/files/games/raid_shadow_legends/champion/Marked.jpg)

## Current Stats
| Stat | Value |
|---|---|
| HP | 4602 |
| ATK | 210 |
| DEF | 207 |
| SPD | 95 |
| C.RATE | 15% |
| C.DMG | 52% |
| ACC | 27 |
| RES | 37 |
| Books Missing | 12 |
| Blessing Grade | 0 |

## Best For
- Clan Boss - Block Debuffs / Increase DEF, for the Unkillable investigation

## Build Priority
- ~160 SPD test value

## Notes
- Took the Clan Boss stun in the first test instead of the intended target (Torturehelm) - comp not yet validated
- Likely why: at 4,602 max HP (vs Torturehelm's 18,731), Marked is probably the team's lowest-HP% champion under sustained boss damage - the Clan Boss's stun-targeting AI falls back to lowest HP% when no one has an affinity or protective-buff match. See the diagnosis in [[../02 Teams/Clan Boss - Nightmare Unkillable (In Progress)]].
- Full history: [[../05 History/Historical Knowledge Archive]]

## Teams Used In
```dataview
LIST
FROM "02 Teams"
WHERE contains(champions, this.file.link)
```
