---
name: melt-pm-close-my-day
description: End-of-day check for a PM. Use when the PM says "close my day", "wrap up", "end-of-day check", "what didn't I get to", or finishes their day. Reads back the morning's plan and checks what got done, blocked or slipped, confirms every client meeting today was processed (recap and Changelog), reviews tracker activity and client Slack for unhandled items, helps close PM Blockers with notes, drafts the client-asks digest, and on the week's last working day checks next sprint's readiness.
---

# melt-pm-close-my-day

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-pm:close-my-day"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-pm:close-my-day"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
