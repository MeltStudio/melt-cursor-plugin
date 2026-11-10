---
name: melt-pm-plan-my-day
description: Start-of-day orchestrator for a PM. Use when the PM says "plan my day", "what should I work on today", "what's on my plate", or starts their morning. Checks calendar and meltctl, closes the previous working day first if close-my-day was skipped, then builds one sequenced agenda from portfolio health, today's meetings, carried items, open PM Blockers, recent Changelog entries and stale Add-Task drafts, each tagged with the skill to run. Week-opener mode; holiday and OOO aware.
---

# melt-pm-plan-my-day

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-pm:plan-my-day"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-pm:plan-my-day"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
