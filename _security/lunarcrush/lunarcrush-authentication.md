---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lunarcrush Authentication
name_suffix: Authentication
oauth_flows: []
overview: LunarCrush secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LunarCrush
provider_slug: lunarcrush
scheme_count: 1
schemes:
- applies_to:
  - api: LunarCrush API v4
    base_url: https://lunarcrush.com/api4
    example: 'curl -H "Authorization: Bearer <API_KEY>" https://lunarcrush.com/api4/public/topics/list/v1'
  - api: LunarCrush.ai
    base_url: https://lunarcrush.ai
    example: 'curl -H "Authorization: Bearer <API_KEY>" https://lunarcrush.ai/topic/bitcoin?format=json'
  description: 'API key issued in the LunarCrush account/settings, sent as `Authorization: Bearer <API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://lunarcrush.com/developers/api/authentication
  type: http
slug: lunarcrush-authentication
source_filename: lunarcrush-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://lunarcrush.com/developers/api/authentication\ndocs: https://lunarcrush.com/developers/api/authentication\nsummary:\n  types: [http]\n  scheme: bearer\n  api_key_in: [header]\n  note: >-\n    Both LunarCrush surfaces (the v4 REST API at lunarcrush.com/api4 and the\n    AI/agent interface at lunarcrush.ai) authenticate with a single Bearer API\n    key passed in the Authorization header. There is no OAuth or per-scope\n    authorization surface; access level is governed by the account subscription\n    tier, not by token scopes.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key issued in the LunarCrush account/settings, sent as\n    `Authorization: Bearer <API_KEY>`.\n  sources:\n  - https://lunarcrush.com/developers/api/authentication\n  applies_to:\n  - api: LunarCrush API v4\n    base_url: https://lunarcrush.com/api4\n    example: 'curl -H \"Authorization: Bearer <API_KEY>\"\
  \ https://lunarcrush.com/api4/public/topics/list/v1'\n  - api: LunarCrush.ai\n    base_url: https://lunarcrush.ai\n    example: 'curl -H \"Authorization: Bearer <API_KEY>\" https://lunarcrush.ai/topic/bitcoin?format=json'\ncli_auth:\n  login_browser: lunarcrush login\n  login_key: lunarcrush login --api-key <key>\n  whoami: lunarcrush whoami\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunarcrush/refs/heads/main/authentication/lunarcrush-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Social Intelligence
- Cryptocurrency
- Stocks
- Sentiment Analysis
- Social Media
- Market Data
- Analytics
- AI Agents
- MCP
---
