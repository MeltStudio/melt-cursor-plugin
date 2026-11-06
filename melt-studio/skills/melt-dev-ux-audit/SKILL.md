---
name: melt-dev-ux-audit
description: Review the project's UI against usability heuristics using Chrome DevTools MCP. Use when the developer wants to check UX quality, says "review the UI", or "UX audit". Full audit, or feature-scoped during an active plan.
---

# melt-dev-ux-audit

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-dev:ux-audit"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-dev:ux-audit"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
