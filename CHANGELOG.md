# Roar Guild Addon Wrath — changelog and dated evidence

**Project author:** Babuni. The following dates are **Git commit dates**, not claimed public releases or runtime verification.

## 2026-10-26 — full project documentation

- Expanded README, concept, roadmap, architecture, design, content inventory, decisions, narrative journal, attribution and development rules.
- Documented the two distinct repository/install names, Wrath interface 30300, action-button (not spell-success) trigger behavior and the secure-hook/fallback-wrapper architecture.
- Counted 33 current recruitment messages and recorded the absence of Roarboard from this codebase.
- Preserved the April 2026 adaptation and later documentation/compatibility wording changes.
- **Docs-only:** no Lua/TOC/LICENSE edits, no WoW client tests.

## Prior history recovered from Git

| Date | Commit | Demonstrable change |
| --- | --- | --- |
| **2026-04-27** | `b1077ec`, `c1cce7d` | Repository created; large initial `ROARTrigger.lua` added with `RoarGuild v1.32-Epoch` / Project Epoch-Wrath 3.3.5 header, `/rogu` commands, profiles, fallback and guild copy. |
| **2026-04-27** | `378e511`, `6a6f8f5` | TOC created with `Interface 30300` and `1.32-Epoch`; displayed addon title adjusted from RoarGuild to RoarTrigger. |
| **2026-05-13** | `e081668`, `5672063` | Guild invitation text revised in Lua; README greatly expanded with installation, commands, behavior, troubleshooting, and explicit warning that action use does **not** prove spell success. |
| **2026-09-18** | `37130e3` | Removed Project Epoch-specific wording from README and Lua header; version standardized to **1.32**, client described as Wrath 3.3.5, without changing the interface target. |
| **2026-10-26** | Earlier credit/docs commits | Standardized author credit and added a short documentation scaffold prior to this deeper audit. |

The early file used the internal **RoarGuild** header, while this repository now has its own display name and client target. The source establishes close implementation relationship, but the inspected commit history does not include a complete original conversation, exact copy/port commit relationship, or all motivations.

## 2026-11-01 — EmoteTrigger repository name

- The GitHub repository was renamed from `ROARemoteTrigger` to **EmoteTrigger**.
- At my direction, AI revised documentation, first-person narrative and attribution while retaining the **ROARTrigger** runtime names and original MIT license.
- No Lua, TOC, license or in-game test was changed.

## 2026-11-01 — Roar Guild Addon Wrath

- Renamed the GitHub project to `RoarGuildAddonWrath` at my direction.
- AI updated documentation with my clarification of the Wrath port and later 1.12 Roarboard development.
- No runtime files or tests changed.

## 2026-11-01 — documented the family lineage

- Recorded the current name **Roar Guild Addon Wrath**, its earlier ROARemoteTrigger/EmoteTrigger identities and the preserved ROARTrigger installation name.
- Linked [the expressive-addon history](docs/EMOTE_FAMILY_HISTORY.md) and clarified its user-added emote registry; no runtime changes.
