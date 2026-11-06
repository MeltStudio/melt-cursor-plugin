---
name: melt-pm-add-task
description: Frictionless task capture for the PM. Use when the PM says "add a task", "note this down", "remember this", "ask X about Y", or describes a thought worth capturing without naming a skill. One paragraph in, one draft Linear issue out in the "Project Managers CheckList" team, assigned to the PM. No required fields; a one-liner or a fully structured task both work. Also called from the intake skills for the PM's own commitments, on the PM's yes.
---

# melt-pm-add-task

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-pm:add-task"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-pm:add-task"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
