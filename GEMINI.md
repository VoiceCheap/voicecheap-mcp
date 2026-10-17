# VoiceCheap

Use the VoiceCheap skill in `skills/voicecheap/SKILL.md` when the user asks for
VoiceCheap media or project work. Discover the current tools and their schemas;
never infer permission from the presence of this extension. Authenticate with
`/mcp auth voicecheap` when the server requests browser OAuth. The user completes
sign-in and chooses the permissions. Do not ask for credentials in conversation.

Start with an authorized account or project read. Generation spends the user's
existing media credits and requires their request. The extension has no trusted
tool bypass and does not automatically approve actions.
