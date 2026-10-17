# VoiceCheap MCP

Connect your AI agent to VoiceCheap for video translation, dubbing, transcripts, subtitles and speech. This repository contains client configuration, a workflow skill and VoiceCheap branding.

## Connection

Remote endpoint: `https://api.voicecheap.ai/mcp` (Streamable HTTP). Sign in through VoiceCheap OAuth and begin with Read Only permissions. Grant additional permissions only for workflows you request. Do not paste tokens, passwords or API keys into a chat or this repository.

First prompt: “Show my VoiceCheap credits and list my five most recent projects.”

API/MCP access requires a VoiceCheap plan with API access. Media generation uses existing account credits. Subscriptions and credit purchases take place on the VoiceCheap website.

## Clients

- Cursor: plugin manifest in `.cursor-plugin/plugin.json`, remote connection in `mcp.json`.
- Grok Build: plugin manifest in `.grok-plugin/plugin.json`, connection in `.mcp.json`.
- Gemini CLI: `gemini extensions install https://github.com/VoiceCheap/voicecheap-mcp`
- Other MCP clients: add the remote endpoint and complete OAuth.
- OpenClaw: the standalone workflow skill is in `openclaw/`.

Marketplace approval and indexing are managed by each platform. The presence of these files does not establish approval or completed client testing.

## What is included

Configuration, documentation, the VoiceCheap workflow skill and branding. Requests go to VoiceCheap’s hosted API. There are no executable hooks or embedded credentials. Generated result URLs may point to storage locations returned by the service. No additional telemetry is introduced by this repository.

## Links

- [VoiceCheap](https://www.voicecheap.ai/en)
- [MCP guide](https://www.voicecheap.ai/docs/ai/model-context-protocol)
- [Documentation and support](https://www.voicecheap.ai/docs/introduction)
- [Privacy](https://www.voicecheap.ai/en/privacy)
- [Terms](https://www.voicecheap.ai/en/terms)
- [Manage or revoke connections](https://app.voicecheap.ai/page-api)

Published by VOICECHEAP, SAS, France.

## License

Client configuration, documentation and skills are distributed under the MIT license. No trademark rights to the VoiceCheap name or logo are granted. The hosted VoiceCheap service remains subject to its own terms.
