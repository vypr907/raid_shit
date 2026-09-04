---
tags: [dashboard]
---

# RAID: Shadow Legends — Command Center

> [!info] Setup
> This dashboard uses the **Dataview** community plugin. Install it via Settings → Community Plugins → Browse → search "Dataview" → Enable. Until then, the query blocks below will show as plain code instead of live tables.

## Roster Snapshot
```dataview
TABLE length(rows) as "Champions"
FROM "01 Champions"
GROUP BY rarity
SORT rarity DESC
```

## By Faction
```dataview
TABLE length(rows) as "Champions"
FROM "01 Champions"
GROUP BY faction
SORT length(rows) DESC
```

## Legendaries — Rank 6, Not Yet Fully Booked
```dataview
TABLE faction, affinity, rank, books_missing
FROM "01 Champions"
WHERE rarity = "Legendary" AND rank = 6 AND books_missing > 0
SORT books_missing ASC
```

## Speed Leaderboard (Top 15)
```dataview
TABLE faction, affinity, spd, rank
FROM "01 Champions"
SORT spd DESC
LIMIT 15
```

## Quick Links
- [[03 Strategies/Build Priorities|Build Priorities]]
- [[03 Strategies/General Strategy Notes|General Strategy Notes]]
- [[04 Progress/Clan Boss|Clan Boss Progress]]
- [[04 Progress/Dungeons|Dungeons Progress]]
- [[04 Progress/Faction Wars|Faction Wars Progress]]
- [[04 Progress/Arena|Arena Progress]]
- [[04 Progress/Doom Tower|Doom Tower Progress]]
- [[04 Progress/Hydra|Hydra Progress]]
- [[02 Teams/_Team Template|New Team]]
- [[Templates/Champion Template|Champion Note Template]]
- [[05 History/Historical Knowledge Archive|Historical Knowledge Archive]]
- [[06 Dev Projects/raid_roster status|raid_roster Dev Status]]

## How to Query Your Roster
Examples you can paste into any note inside a ```dataview``` block:

Find all Void champions from Dark Elves:
```
TABLE rank, level, spd
FROM "01 Champions"
WHERE faction = "Dark Elves" AND affinity = "Void"
```

Find champions with Speed over 200:
```
TABLE faction, spd
FROM "01 Champions"
WHERE spd > 200
SORT spd DESC
```
