# Roar Guild Addon Wrath — human–AI collaboration and provenance

Follow [the documentation standard](DOCUMENTATION.md) for first-person author voice throughout project documentation, factual changelogs, and naming the AI tool and verified model for each contribution.

**Creator and creative director:** Babuni.

## Creative ownership

The repo's theme—using action presses to give a player's character more spontaneous expression—comes from the creator's ROAR-family work, not from this documentation audit. Its guild voice values exploring, curiosity, kindness, and shared stories. The uploaded source bears the internal header `RoarGuild v1.32`; that is evidence of conceptual/code proximity to neighboring projects, but it does not attribute original human ideas to AI or prove a specific cross-repository merge.

Do not mistake native WoW emote tokens for uniquely AI-generated or creator-recorded audio/animations.

## What this AI session contributed

On 2026-10-26 the assistant:
- Inspected the live README, `ROARTrigger.lua`, `ROARTrigger.toc`, LICENSE and existing short docs.
- Read relevant April, May and September commit diffs.
- Distinguished repository name, installed addon name, TOC title, slash command and saved-data identifiers.
- Explained source-supported behavior: post-action hook, configured instance odds, success-only fallback throttle, character profiles, statistics and manual guild invitations.
- Counted **33** current recruitment lines and confirmed the source does **not** include Roarboard.
- Rewrote/created eleven Markdown development files and identified unverified compatibility and user-experience questions.

This is an **editorial, analytic and documentation contribution**. It is **not** evidence that the assistant originally conceived the addon, wrote every prior source revision, tested the game client, merged RoarGuild, or received approval to change runtime behavior.

## Standards for the next change

For each substantial implementation, write a documentation-ready record that preserves:
1. **User direction** — goal, reasoning, constraints and creative authorship.
2. **AI proposal** — designs, assumptions, limitations and alternatives.
3. **Iteration** — experiments, misunderstandings, rejected paths and corrections.
4. **Explicit decision** — what Babuni chose, rejected or postponed.
5. **Implementation** — changed files, commit/PR and compatibility effects.
6. **Verification** — what was tested in which game client, outcome and remaining unknowns.

When an original conversation is unavailable, label the result **retrospective source reconstruction** and do not invent quotes. Do not publish private guild messages, credentials, or players' identifying information in a public portfolio journal. Preserve external URLs and MIT credit.

## November 2026 — documenting my rename

In the intermediate naming pass, I renamed the repository from **ROARemoteTrigger** to **EmoteTrigger**. It has since been renamed **RoarGuildAddonWrath**. Its work in this session consisted of reviewing existing documentation and revising titles, links and attribution. The historical installed **ROARTrigger** addon and MIT license were preserved. No live game tests were carried out.

## November 2026 — my clarification of the client history

The client chronology is my recollection: the Wrath 3.3.5 port came first, then a return to 1.12 and later Roarboard development in the separate guild addon. The current repository name is **RoarGuildAddonWrath**; the installed addon remains **ROARTrigger**. AI revised the documentation at my request rather than changing gameplay.

## Related development history

Roar Guild Addon Wrath is the Wrath 3.3.5 port of the earlier Roar Guild emote system, not a numbered sequel. Its repository was formerly ROARemoteTrigger, briefly EmoteTrigger; the installed addon remains ROARTrigger (`/rogu`, ROGUDB). It retains a **player-extensible native-emote registry** starting with ROAR, multiple configured action-slot triggers and a manually invoked guild-recruitment chat command. It does **not** include the Roarboard added to the separate Vanilla guild-addon project after returning to that client. See the [complete source-grounded timeline](EMOTE_FAMILY_HISTORY.md) for its relationship to the other emote addons.
