---
tags: [meta]
---

# RAID: Shadow Legends Vault — Setup & Structure

## Folder Structure
- **00 Dashboard.md** — start here. Live roster stats via Dataview.
- **01 Champions/** — one note per champion (376 notes), generated from your RSL Helper export dated 2026-08-28. Frontmatter has faction, affinity, rarity, rank, level, and current stats — this is what Dataview queries against.
- **02 Teams/** — team comps you build. Copy `_Team Template.md` for each new team.
- **03 Strategies/** — build priorities and general account strategy.
- **04 Progress/** — one tracker each for Clan Boss, Dungeons, Faction Wars, Arena, Doom Tower, and Hydra.
- **05 History/** — the canonical Historical Knowledge Archive: current state + a full chronological merge of every past strategy conversation, reconciled and cross-referenced against the roster.
- **06 Dev Projects/** — status notes for related side projects (currently: raid_roster, the local roster-tracking web app).
- **Templates/** — reusable note templates.

## One-Time Setup
1. **Install Dataview**: In Obsidian, Settings → Community Plugins → turn off Restricted Mode → Browse → search "Dataview" → Install → Enable. This powers the live tables on the Dashboard and in champion notes.
2. This folder was placed inside your existing "Second Brain" vault, so no new vault setup is needed — it'll show up in your file explorer automatically once synced.

## Keeping Champion Data Current
The 376 champion notes were generated once from your CSV export. They are **not** auto-updating. When you rank up, level up, or re-gear a champion:
- Manually edit that champion's frontmatter (rank, level, stats), **or**
- Re-export from RSL Helper and ask Claude to regenerate the `01 Champions/` notes from the new CSV (this will overwrite stat fields but won't touch anything you've written in Best For / Build Priority / Notes, as long as you ask for a merge rather than a full overwrite).

## Faction / Affinity / Rarity Legend
| Code meaning | Values |
|---|---|
| Affinity | Magic, Force, Spirit, Void |
| Rarity | Common, Uncommon, Rare, Epic, Legendary |
| Factions | Banner Lords, High Elves, Sacred Order, Barbarians, Ogryn Tribes, Lizardmen, Skinwalkers, Orcs, Demonspawn, Undead Hordes, Dark Elves, Knights Revenant, Dwarves, Shadowkin, Sylvan Watchers, Argonites |

These were decoded from your CSV's numeric codes and cross-checked against multiple champion databases (HellHades, AyumiLove, InTeleria) champion-by-champion, so they should be accurate — flag anything that looks wrong.
