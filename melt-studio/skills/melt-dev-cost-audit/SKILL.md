---
name: melt-dev-cost-audit
description: Run a comprehensive AWS cost optimization audit across the project's cloud infrastructure. Use when the developer wants to reduce AWS spend, says "cost audit", "AWS cost review", or is trying to hit a cloud budget target. Produces a per-service findings report, a PM memo for right-sizing decisions, and a sequenced execution plan.
---

# melt-dev-cost-audit

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-dev:cost-audit"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-dev:cost-audit"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
