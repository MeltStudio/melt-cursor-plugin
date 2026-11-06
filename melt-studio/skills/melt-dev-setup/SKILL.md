---
name: melt-dev-setup
description: "Set up or migrate a repo onto Melt's current model: remove any legacy per-repo melt-* skill files, customize AGENTS.md, and propose a baseline .mcp.json. Use when setting up a new project, when AGENTS.md has placeholder markers, when the developer says \"update melt\" or \"migrate melt\", or when a repo still has old .claude/skills/melt-* files. The entry point — no separate init or update step."
---

# melt-dev-setup

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-dev:setup"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-dev:setup"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
