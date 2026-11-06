---
name: melt-dev-help
description: Answer questions about the AI-First Development Playbook and team workflow. Use when the developer asks about the development process, what step they're on, or how validation works. Reference skill — it explains, doesn't execute.
---

# melt-dev-help

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-dev:help"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-dev:help"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
