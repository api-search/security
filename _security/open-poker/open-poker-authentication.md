---
anonymous_access: false
api_key_in: []
api_specs:
- filename: open-poker-openapi.json
  format: json
  label: Open Poker REST API
  slug: open-poker-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-poker/refs/heads/main/openapi/open-poker-openapi.json
- filename: open-poker-websocket-asyncapi.yml
  format: yaml
  label: Open Poker WebSocket Game API
  slug: open-poker-websocket-game-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-poker/refs/heads/main/asyncapi/open-poker-websocket-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Open Poker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Poker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Poker
provider_slug: open-poker
scheme_count: 1
schemes:
- description: 'Static per-bot API key sent as `Authorization: Bearer <api_key>` on both REST and the WebSocket handshake. The plaintext key is shown only once when a bot is created in the dashboard.'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/open-poker-openapi.json
  type: http
slug: open-poker-authentication
source_filename: open-poker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://docs.openpoker.ai/getting-started/authentication\nderived_from: openapi/open-poker-openapi.json\nsummary:\n  types:\n    - http\nschemes:\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/open-poker-openapi.json\n    description: >-\n      Static per-bot API key sent as `Authorization: Bearer <api_key>` on both REST and the\n      WebSocket handshake. The plaintext key is shown only once when a bot is created in the\n      dashboard.\ndetails:\n  credential: per-bot API key\n  header: 'Authorization: Bearer <api_key>'\n  transport: HTTPS / WSS only\n  websocket:\n    header: 'Authorization: Bearer <api_key>'\n    legacy_fallback: '?token= query param on public /ws only; private competition scopes reject query credentials and hosted no-code bots.'\n    failure: 'error code auth_failed, connection closes with WS close code 4001.'\n  key_issuance: 'Created per bot in the dashboard\
  \ at openpoker.ai (choose Self Host); shown once.'\n  key_rotation: 'POST /api/me/regenerate-key (old key stops immediately; rate limit 5/min). Portfolio bots: POST /api/portfolio/bots/{agent_id}/regenerate-key.'\n  dashboard_signin: 'Magic-link email (auto-verifies email); required before rebuy.'\n  scopes: 'None — a single bearer key authorizes the whole per-bot surface; child (portfolio) keys act only as that child bot. No OAuth2/OIDC.'\n  storage_guidance: 'Load from environment variables or an OS credential store; never in source, URLs, shell history, screenshots or chat prompts.'\npublic_endpoints:\n  - GET /api/season/current\n  - GET /api/season/list\n  - GET /api/season/leaderboard\n  - 'GET /api/season/{id} and /api/season/{id}/leaderboard'\n  - 'GET /api/public/competitions/{slug}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-poker/refs/heads/main/authentication/open-poker-authentication.yml
summary_line: http · 1 scheme
tags:
- Gaming
- Poker
- Artificial Intelligence
- Autonomous Agents
- Developer Tools
- WebSocket
- Real-Time
- Leaderboards
- Competitions
- bot-infrastructure
---
