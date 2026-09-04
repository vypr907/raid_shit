---
name: "Torturehelm"
faction: "Orcs"
affinity: "Force"
rarity: "Epic"
rank: 4
level: 40
hp: 18731
atk: 692
def: 1227
crit_rate: 40
crit_dmg: 52
spd: 96
acc: 42
res: 86
books_missing: 8
blessing_grade: 0
tags:
  - champion
  - "faction/Orcs"
  - "affinity/Force"
  - "rarity/Epic"
---

# Torturehelm

`= this.faction` · `= this.affinity` · `= this.rarity` · Rank 4 · Level 40

![Torturehelm](https://ayumilove.net/files/games/raid_shadow_legends/champion/Torturehelm.jpg)

## Current Stats
| Stat | Value |
|---|---|
| HP | 18731 |
| ATK | 692 |
| DEF | 1227 |
| SPD | 96 |
| C.RATE | 40% |
| C.DMG | 52% |
| ACC | 42 |
| RES | 86 |
| Books Missing | 8 |
| Blessing Grade | 0 |

## Best For
- Clan Boss - intended stun-absorption target via self-revive, for the Unkillable investigation

## Build Priority
- ~187 SPD test value

## Notes
- First calculator test failed to route the stun to him (it hit Marked instead) - see [[../02 Teams/Clan Boss - Nightmare Unkillable (In Progress)]]
- The Hotatsu-swap rotation test (Sept 3, 2026) confirmed stable turn timing, but still doesn't confirm he's the stun target - the calculator doesn't simulate targeting. His much higher HP pool than Marked's (18,731 vs 4,602) is likely why he SHOULD take it under the game's lowest-HP% fallback rule, but this needs an in-game test to confirm.
- Full history: [[../05 History/Historical Knowledge Archive]]

## Teams Used In
```dataview
LIST
FROM "02 Teams"
WHERE contains(champions, this.file.link)
```
