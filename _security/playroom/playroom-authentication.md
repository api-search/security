---
api_key_in: []
auth_types:
- gameId
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Playroom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Playroom secures its APIs with gameId and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Playroom
provider_slug: playroom
scheme_count: 3
schemes:
- docs: https://docs.joinplayroom.com/errors/no-game-id
  issued_by: https://dev.joinplayroom.com
  name: gameId
  read_only: true
  type: application-identifier
  where: insertCoin({ gameId })
- context: Discord Activities embedding
  docs: https://docs.joinplayroom.com/features/integrations/discord
  helpers:
  - getDiscordAccessToken
  - getDiscordClient
  - getDiscordSDK
  name: discord-oauth
  type: oauth2
- context: TikTok Live embedding
  docs: https://docs.joinplayroom.com/features/integrations/tiktok
  helpers:
  - onTikTokLiveEvent
  name: tiktok
  type: platform-session
slug: playroom-authentication
source_filename: playroom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.joinplayroom.com/errors/no-game-id\nsummary:\n  types: [gameId, oauth2]\n  model: client-side-sdk\n  note: >-\n    Playroom Kit is a client-side SDK. There is no server API key. Each app is\n    identified by a read-only gameId issued when a project is created in the Dev\n    Portal, passed to insertCoin({ gameId }). Realtime connections are brokered\n    by Playroom's hosted infrastructure keyed on that gameId. OAuth is only\n    involved when embedding into host platforms (Discord Activities, TikTok Live),\n    where the platform's OAuth/token surface is used via the bundled SDK helpers.\nschemes:\n  - name: gameId\n    type: application-identifier\n    where: insertCoin({ gameId })\n    issued_by: https://dev.joinplayroom.com\n    read_only: true\n    docs: https://docs.joinplayroom.com/errors/no-game-id\n  - name: discord-oauth\n    type: oauth2\n    context: Discord Activities embedding\n    helpers: [getDiscordAccessToken,\
  \ getDiscordClient, getDiscordSDK]\n    docs: https://docs.joinplayroom.com/features/integrations/discord\n  - name: tiktok\n    type: platform-session\n    context: TikTok Live embedding\n    helpers: [onTikTokLiveEvent]\n    docs: https://docs.joinplayroom.com/features/integrations/tiktok\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playroom/refs/heads/main/authentication/playroom-authentication.yml
summary_line: gameId/oauth2 · 3 schemes
tags:
- Company
- Multiplayer
- Gaming
- Game Development
- Real-time
- SDK
- State Synchronization
- Developer Tools
---
