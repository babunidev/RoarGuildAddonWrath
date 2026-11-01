# Roar Guild Addon Wrath — AI and human developer rules

**By:** Babuni.

## Naming and writing conventions

**RoarGuildAddonWrath** is the current repository (previous names `ROARemoteTrigger` and `EmoteTrigger`). It is the Wrath 3.3.5 port of Roar Guild Addon; Roarboard was developed after the return to 1.12 and does not exist in this version. The installed addon remains `ROARTrigger`, using `ROARTrigger.lua`, `ROARTrigger.toc`, `/rogu` and `ROGUDB`. Never silently change these names in a documentation update.

Write public development narratives from my first-person viewpoint without beginning sentences with `I` or `My`. The person is **Babuni** and the development portfolio is **babuni.dev**. Use “creative”, not “creator”, for the human role. Distinguish my decisions and original concepts from AI research, code edits and documentation; do not invent unrecorded motivations or test results. Technical references may remain neutral.

## Never collapse identities or attribution

The **current GitHub repo** is `RoarGuildAddonWrath` (formerly `ROARemoteTrigger` and `EmoteTrigger`); the **installable addon** is `ROARTrigger`; the slash command and SavedVariables deliberately remain `/rogu` and `ROGUDB`. The Lua still has a `RoarGuild v1.32` comment. Preserve these observed names and do not silently rename files, the TOC title or protocol identifiers in a documentation pass.

This is a **Wrath 3.3.5 / interface 30300** artifact and has **no Roarboard**. Do not copy RoarGuild 1.33 feature claims into this repository. A neighboring RoarGuild project exists, but exact port authorship/history needs source evidence.

## Code behavior to protect

- The code observes action-bar use **whether or not a spell succeeds**.
- Use `hooksecurefunc` when available, else its existing post-delegation `UseAction` wrapper; test on the actual supported client.
- A configured instance consumes its cooldown on an eligible attempt, even when its chance roll fails.
- Global fallback is independent, limited to slots 1–200, and consumes its cooldown **only when it successfully emotes**.
- The master emote registry lives in account-wide `ROGUDB`, profiles under name-realm keys; loading resets cooldowns on login.
- `/rogu roar` always emits ROAR and is not dependent on random instance selection.
- Recruitment messages are dispatched only by explicit `/rogu invite` to a numeric channel, which might not be General.
- Last-hour statistics and reminders are tied to action activity; they are not background scheduled tasks.

## Collaboration, verification and safety

1. Respect Babuni's ownership of the concept and all explicitly recorded user decisions.
2. Clearly distinguish AI-proposed features, implementation, retrospective interpretation, rejected alternatives, and in-game verification.
3. Maintain `README.md`, `CONCEPT.md`, `ROADMAP.md`, `CHANGELOG.md`, `AGENTS.md`, and `docs/DEVLOG.md`, `docs/DECISIONS.md`, `docs/DESIGN.md`, `docs/CONTENT.md`, `docs/ARCHITECTURE.md`, `docs/AI_COLLABORATION.md`.
4. Test against the exact Wrath 3.3.5 environment before declaring API support. Preserve `UseAction` execution and check coexistence with other action-hook addons.
5. Do not expose private conversations, credentials or actual player chat in a public portfolio narrative.
6. Preserve MIT license, author credit and existing source identifiers; avoid runtime edits in documentation-only changes.

This 2026-10-26 session **only** adds/rewrites Markdown documentation and reports unverified behavior honestly.
