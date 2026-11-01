# Roar Guild Addon Wrath — evidence-based decisions and open questions

**Decision-maker:** Babuni. Code and commits can show implementation, not hidden approval dialogues.

## What source and history demonstrate

| Design area | Observable evidence | Status |
| --- | --- | --- |
| Wrath 3.3.5 compatibility target | TOC `30300`; Apr 27 `1.32-Epoch` source header | Explicit target; runtime testing not verified |
| Installable title distinct from repo | `6a6f8f5` changed TOC title to RoarTrigger | Historical naming revision |
| React to player intent, not spell success | `UseAction` callback and README warning | Source implementation, not cast-result verification |
| Secure post-hook when available | `hooksecurefunc` branch, post-delegation fallback | Present since initial source upload |
| Per-character profiles | `ROGUDB.profiles[name-realm]` | Implemented |
| Independent chance/cooldown and fallback | `ROGU_DoBattleEmoteForCfg`, `ROGU_TryFallback` | Implemented with different timestamp semantics |
| Guild recruitment | `inviteText`, `/rogu invite` | Explicit player action, 33 current messages |
| Manual ROAR | `/rogu roar` calls `performEmote("ROAR")` | Guaranteed token independent of configured instance |
| No Roarboard | Absence of `/roarboard`, `RB1`, channel receiver and board state | Distinguishes this version from RoarGuild 1.33 |

## Historical interpretation limits

An April 27, 2026 source file begins **“RoarGuild v1.32-Epoch”** and carries a broad `/rogu` command system. That demonstrates a close implementation relationship to the RoarGuild family, but this separate repository does not show a full cross-repository merge graph or a preserved original discussion of the adaptation. Avoid inventing whether this was intended as a permanent fork, a personal experiment, or a formal compatible release.

On May 13 the README was massively expanded to spell out installation and the action-versus-spell-success distinction. On September 18, client-specific provider labels and `-Epoch` suffix were removed from README/source/TOC, while the explicit Wrath interface number remained.

## Questions needing actual creator answers

- The project is now named `RoarGuildAddonWrath`; any future code consolidation with the separate `RoarGuildAddon` requires a new decision.
- Should the global fallback and configured instances both react on the same button press?
- Should user-facing naming be simplified without breaking folder, TOC, slash command, or saved-data compatibility?
- Should the reminder/statistics remain default behavior in a purely expressive addon?
- Which exact client variant(s) will Babuni explicitly support after verification?
- Does a future UI need to surface configuration IDs to casual players?

Document each decision when Babuni actually makes it; this analysis authorizes no runtime changes.

## November 2026 — repository identity

**EmoteTrigger** was an intermediate name after **ROARemoteTrigger**; the current name is **Roar Guild Addon Wrath**. Its installed addon remains **ROARTrigger**. This distinguishes the repository's descriptive identity from the historical runtime files, slash commands and saved variables. No gameplay migration or testing was performed.

## November 2026 — current project name

I chose **Roar Guild Addon Wrath** for this client port, rather than presenting it as a numbered sequel. The repository is **RoarGuildAddonWrath**. Roarboard was developed after my return to 1.12 and is absent here. The installed **ROARTrigger** files and runtime identifiers remain unchanged.
