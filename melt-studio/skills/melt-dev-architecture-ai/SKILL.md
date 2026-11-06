---
name: melt-dev-architecture-ai
description: Design and make architecture decisions for AI and agentic systems. Use when designing an LLM/agent feature, choosing single-agent vs multi-agent, picking an agentic pattern (ReAct, coordinator, hierarchical, swarm, human-in-the-loop, …), deciding RAG vs tools vs just-in-time retrieval, planning context/memory, or asking "should this even be an agent?" — any LLM-system trade-off, even when the word "architecture" isn't used.
---

# melt-dev-architecture-ai

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-dev:architecture-ai"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-dev:architecture-ai"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
