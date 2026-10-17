---
name: voicecheap
description: Use when the user asks to manage their VoiceCheap projects, translate or dub their media, export transcripts or subtitles, or generate speech with their VoiceCheap account.
---

# VoiceCheap workflows

Use the connected VoiceCheap MCP tools for the user's requested media or account
workflow. Read [the workflow reference](references/workflows.md) before acting.
The actual tool catalog and schemas are authoritative; available tools depend
on the granted permissions. A skill does not grant additional permissions.

If the server is unavailable, use the client's supported connection flow for
`https://api.voicecheap.ai/mcp`. Let the user complete browser authentication.
Do not read local credential files or ask for secrets in chat. Preserve other
connections. Verify the connection with an authorized read before reporting
success. Report missing access neutrally without initiating checkout.
