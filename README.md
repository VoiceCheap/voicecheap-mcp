# VoiceCheap MCP

Connect an agent to your VoiceCheap account for audio, video, voice and visual
workflows. Available tools depend on the permissions you grant and your account
access.

- Transcribe audio or video and retrieve or generate YouTube transcripts and
  timestamped chapters.
- Create SRT subtitles, translate SRT/VTT while preserving timing, export saved
  subtitles, and burn subtitles into uploaded or YouTube videos.
- Generate speech, design voices, and clone voices with explicit speaker permission.
- Generate images and thumbnails, then retrieve your saved results.
- Translate and dub projects, generate lip sync, and add dynamic subtitles to
  completed translated or lip-synced videos.
- Manage permitted publishing to connected channels, account usage and settings,
  team access, glossaries, workspace folders and supported webhook settings.

This is a client configuration package. Each marketplace manages its own review
and indexing. Package validation does not establish that the current production
deployment contains the same code as this checkout, or that a provider connection
has been tested.

## Connection

The package connects to `https://api.voicecheap.ai/mcp` using Streamable HTTP.
Authentication happens through VoiceCheap's browser-based OAuth consent flow.
For a basic connection check, approve only `account:read`. Add only the read or
write permissions needed for a requested workflow; a Read Only preset may also
expose project and media data. Never paste passwords, API keys, authorization
codes or tokens into the conversation or this package.

A VoiceCheap account with API and MCP access is required. API/MCP calls share
the account's allowance; generation uses the applicable existing credits and
allowances. The package does not initiate purchases or manage card payments.

First ask: "Show my VoiceCheap credits and the tools available to this connection."
Check the actual tool response before treating the connection as working.
Generating media, changing account data and publishing media require a user
request that authorizes those actions. Voice cloning also requires explicit
permission from the speaker.

Keep account data and media private. Public listings, examples and demo recordings
must not disclose account or project identifiers, credentials or media links.
Use synthetic content for reviews and grant only the permissions each review
needs. Publishing or sharing an output requires the user's explicit destination
and privacy choice; connecting an account does not make its videos public.

## Clients

- Cursor: plugin manifest in `.cursor-plugin/plugin.json`, remote connection in `mcp.json`.
- Grok Build: plugin manifest in `.grok-plugin/plugin.json`, connection in `.mcp.json`.
- Gemini CLI: `gemini extensions install https://github.com/VoiceCheap/voicecheap-mcp`
- Other MCP clients: add the remote endpoint and complete OAuth.
- OpenClaw: the standalone workflow skill is in `openclaw/`.

Marketplace approval and indexing are managed by each platform. The presence of these files does not establish approval or completed client testing.

## Links

- [VoiceCheap](https://www.voicecheap.ai/en)
- [MCP connection guide](https://www.voicecheap.ai/docs/ai/model-context-protocol)
- [Documentation and Support link](https://www.voicecheap.ai/docs/introduction)
- [Privacy policy](https://www.voicecheap.ai/en/privacy)
- [Terms of service](https://www.voicecheap.ai/en/terms)

Manage and revoke connections from
[VoiceCheap Integrations](https://app.voicecheap.ai/page-api).

## What is packaged

Client configuration, a workflow skill, documentation and existing VoiceCheap
branding. There are no local executable hooks, backend source files or embedded
credentials. Requests go to VoiceCheap's hosted service; generated result URLs
may point to the storage locations returned by that service. No additional
telemetry is introduced by this package.

The icon is the existing 512-pixel VoiceCheap landing icon, converted from its
actual JPEG encoding to PNG without changing the design. The official public wrapper is
[VoiceCheap/voicecheap-mcp](https://github.com/VoiceCheap/voicecheap-mcp). Its client
configuration, skills and documentation use the included MIT license. No trademark
rights to the VoiceCheap name or logo are granted. Marketplace approval is separate
from publication of this repository.

The separate ClawHub skill release uses that platform's required MIT-0 license.

Published by VOICECHEAP, SAS, France.

## License

Client configuration, documentation and skills are distributed under the MIT license. No trademark rights to the VoiceCheap name or logo are granted. The hosted VoiceCheap service remains subject to its own terms. The separate ClawHub skill release is offered under that platform’s required MIT-0 license.
