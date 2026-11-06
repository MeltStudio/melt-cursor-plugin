---
name: melt-pm-process-client-communication
description: Processes client input that isn't a full meeting transcript. Use when the PM says "client sent me an email", "paste this Slack thread", "here are my notes from the call", "client answered the question I filed", or drops an email, a Slack/WhatsApp/Teams paste, meeting notes, a transcript fragment, a standup summary, a returned roadmap or a tech-investigation answer. Walks each item with the PM; new asks become items for the next meeting. For a full transcript, use melt-pm:process-meeting.
---

# melt-pm-process-client-communication

This skill's instructions live on Melt's meltctl MCP server, so they stay current and private.

1. Call the meltctl MCP tool `get_skill` with `name: "melt-pm:process-client-communication"` and `client: "cursor"`.
2. Follow the instructions it returns exactly, as if they were this skill.
3. When they say to read a file (for example `references/standards.md`), fetch it with the meltctl
   `get_skill_reference` tool (`name: "melt-pm:process-client-communication"`, `path`: that file). The files are not on disk.

If the meltctl tools aren't available or return a 401, stop and tell the user to sign in to the
meltctl MCP server in Cursor (Settings → MCP → meltctl) with their @meltstudio.co Google account,
then run this skill again.
