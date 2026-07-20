---
api_key_in:
- header
- connection-param
api_specs:
- filename: highrise-bot-api-asyncapi.yml
  format: yaml
  label: Highrise Bot API
  slug: highrise-bot-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/highrise/refs/heads/main/asyncapi/highrise-bot-api-asyncapi.yml
- filename: highrise-web-api-openapi.yml
  format: yaml
  label: Highrise Web API
  slug: highrise-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highrise/refs/heads/main/openapi/highrise-web-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Highrise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highrise secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Highrise
provider_slug: highrise
scheme_count: 1
schemes:
- description: Per-bot API token generated in Highrise account settings, bound to a specific room ID. Presented when opening the wss://highrise.game/web/botapi WebSocket connection.
  in: header
  name: BotApiToken
  provisioning: https://highrise.game/account/settings
  scheme: token
  sources:
  - https://create.highrise.game/learn/guides/bots/creating-a-bot
  type: apiKey
slug: highrise-authentication
source_filename: highrise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://create.highrise.game/learn/guides/bots/creating-a-bot\ndocs: https://create.highrise.game/learn/guides/bots/creating-a-bot\nsummary:\n  types: [apiKey]\n  api_key_in: [header, connection-param]\n  oauth2_flows: []\n  notes: >-\n    Highrise uses a static API token (not OAuth). Bot developers mint an API token from the Highrise\n    account settings (\"Bots & API Keys\") and pair it with a room ID. The token is passed when\n    establishing the Bot API WebSocket connection (and by the CLI: `highrise mybot:Bot <room_id>\n    <api_token>`). The read-only Web API serves public data.\nschemes:\n- name: BotApiToken\n  type: apiKey\n  in: header\n  scheme: token\n  description: >-\n    Per-bot API token generated in Highrise account settings, bound to a specific room ID. Presented\n    when opening the wss://highrise.game/web/botapi WebSocket connection.\n  provisioning: https://highrise.game/account/settings\n  sources: [https://create.highrise.game/learn/guides/bots/creating-a-bot]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highrise/refs/heads/main/authentication/highrise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Virtual World
- Metaverse
- Social
- Gaming
- Avatars
- Bots
- Developer Platform
- Chat
---
