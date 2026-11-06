---
name: melt-dev-link
description: Connect and verify required integrations (ticket tracker, browser testing). Use after melt-dev:setup, when tools aren't working, or when a skill reports missing MCP connections. Verifies each tool works and updates AGENTS.md.
---

# melt-dev-link

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-dev:link"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-dev:link"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
