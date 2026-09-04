---
title: Raid Toolkit - Metadata v31 Fix
status: blocked-external / future-me project
priority: low
tags: [project, tooling, raid-toolkit, future]
created: 2026-09-04
related: [[00 Dashboard]]
---

# Raid Toolkit - Metadata v31 Fix

## Summary
Raid Toolkit (RTK) is currently broken for the latest Raid: Shadow Legends game update. It installs and launches, but hangs at the title screen showing "Processing" / "An error occurred" with no further detail. This blocks refreshing the CSV export used to update the champion vault.

## Root Cause
Confirmed via [GitHub Issue #133](https://github.com/raid-toolkit/raid-toolkit-sdk/issues/133) (opened Jul 9, 2026, same version I'm running):

- Game updated to v151571, which bumped the IL2CPP metadata format to **version 31**
- RTK v2.8.22.23238 (latest as of July 2026) throws:
  ```
  System.NotSupportedException: ERROR: Metadata file supplied is not a supported version[31].
  ```
- A symlink workaround (pointing RTK at the correct `global-metadata.dat` path) does **not** fix it — the parser genuinely doesn't understand the new format version, it's not just a path issue.
- This is an upstream bug, not a local install problem. No fix released yet as of Sept 2026.

## Where the actual fix would need to happen
Two repos are involved, not just one:

1. **[raid-toolkit/raid-toolkit-sdk](https://github.com/raid-toolkit/raid-toolkit-sdk)** — the main app/service that hangs on title screen
2. **IL2CPP-Toolkit/Core** — separate repo, ships the `Il2CppToolkit.Metadata` NuGet package that raid-toolkit-sdk depends on for actually parsing `global-metadata.dat`. The version-check/parsing logic likely lives here, not in the main repo.

Forking just raid-toolkit-sdk may not be enough — may need to fork/patch the metadata library too (or reference a patched fork of it).

## Feasibility if I tackle this with Claude Code
- **Best case**: v31 is just a version-number bump with the same underlying struct layout → patch the version allowlist, rebuild, test against my own local `global-metadata.dat`. Could be an hour or two.
- **Worst case**: Unity actually changed the binary struct layout in the new metadata version → needs real reverse engineering (diffing old vs. new metadata structurally, possibly using Il2CppInspectorRedux) before any code fix is possible. Slower, more iterative.
- I have a real advantage here: my own local copy of the v31 `global-metadata.dat` (game is installed via Plarium Play) to test against immediately, rather than working blind.

## Next steps (whenever I pick this up)
1. Check [issue #133](https://github.com/raid-toolkit/raid-toolkit-sdk/issues/133) — see if the maintainer or another contributor has already found/shipped a fix (check this first, may make the whole rest of this moot)
2. If not fixed upstream: fork both repos
3. Have Claude Code locate the version-check code in the metadata parser first — this alone reveals whether it's the easy case or the hard case
4. Locate local metadata file for testing:
   `C:\Users\<username>\AppData\Local\PlariumPlay\PlariumPlay\StandAloneApps\raid-shadow-legends\build\Raid_Data\il2cpp_data\Metadata\global-metadata.dat`

## Impact on vault
Until this is resolved (upstream or self-patched), I can't pull a fresh RSL Helper CSV export to update the champion roster vault. Current vault data reflects the roster as of the last successful export.
