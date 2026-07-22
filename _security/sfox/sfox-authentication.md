---
api_key_in:
- header
api_specs:
- filename: rest-endpoints
  format: yaml
  label: sFOX REST API
  slug: sfox-rest-api
  spec_type: OpenAPI
  url: https://docs.sfox.com/rest-api/rest-endpoints
- filename: sfox-websocket-asyncapi.yml
  format: yaml
  label: sFOX WebSocket API
  slug: sfox-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfox/refs/heads/main/asyncapi/sfox-websocket-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sfox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sfox secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sfox
provider_slug: sfox
scheme_count: 1
schemes:
- applies_to:
  - sFOX REST API (https://api.sfox.com)
  - sFOX WebSocket API (authenticate action before subscribing to private feeds)
  - sFOX Connect API
  description: All REST API requests must include the sFOX API key in the Authorization header as a Bearer token. The key is a static, long-lived secret (not an OAuth access token). API-key permissions are inherited from the owning user account; permission changes apply to existing and new keys automatically.
  environments:
    production: Requires a production API key
    sandbox: Requires a separate sandbox/staging API key
  format: 'Authorization: Bearer <API_KEY>'
  header: Authorization
  in: header
  key_management: https://trade.sfox.com/account/api
  name: BearerApiKey
  scheme: bearer
  type: http
slug: sfox-authentication
source_filename: sfox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sfox.com/rest-api/authentication\ndocs: https://docs.sfox.com/rest-api/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  scheme: bearer-static-key\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <API_KEY>'\n  description: >-\n    All REST API requests must include the sFOX API key in the Authorization\n    header as a Bearer token. The key is a static, long-lived secret (not an\n    OAuth access token). API-key permissions are inherited from the owning user\n    account; permission changes apply to existing and new keys automatically.\n  key_management: https://trade.sfox.com/account/api\n  environments:\n    production: Requires a production API key\n    sandbox: Requires a separate sandbox/staging API key\n  applies_to:\n  - sFOX REST API (https://api.sfox.com)\n  - sFOX WebSocket\
  \ API (authenticate action before subscribing to private feeds)\n  - sFOX Connect API\nnotes: >-\n  WebSocket private feeds require an `authenticate` message carrying the same\n  API key before subscription. Market-data endpoints such as\n  GET /v1/markets/orderbook/{pair} are public and need no auth. sFOX does not use\n  HMAC request signing for the REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sfox/refs/heads/main/authentication/sfox-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cryptocurrency
- Prime Brokerage
- Trading
- Digital Asset Custody
- Liquidity
- Staking
- Institutional
- Financial Services
- Market Data
- WebSocket
- FIX
---
