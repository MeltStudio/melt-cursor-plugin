---
name: melt-pm-prepare-for-meeting
description: Meeting prep for the PM, built from the meeting's own history. Use when the PM says "prep me for the meeting with X", "prep me for the Strategic Review", "prep the Preplan with the tech lead", "one-pager for Monday's Plan", "draft the demo plan", "prep the PM Briefing", "prep the W1/W2/W3/W4 Foundation meeting", or mentions a kickoff, status sync, review or other meeting they're about to run.
---

# melt-pm-prepare-for-meeting

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-pm:prepare-for-meeting"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-pm:prepare-for-meeting"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
