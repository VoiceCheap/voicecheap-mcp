---
name: voicecheap
description: Use when the user asks to connect to or work with their VoiceCheap account for audio/video or YouTube transcription, subtitles and chapters, speech and permitted voice creation, images and thumbnails, dubbing and lip sync, or authorized publishing and workspace actions.
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

Keep private account details, project identifiers, media links and credentials
out of public listings and demonstrations. Use synthetic review content and
only the permissions needed for that review. Never publish media or clone a
voice without the user's specific authorization and the speaker's permission.
