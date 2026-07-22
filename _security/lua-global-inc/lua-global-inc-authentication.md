---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lua Global Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lua Global Inc secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lua Global Inc
provider_slug: lua-global-inc
scheme_count: 1
schemes:
- applies_to: https://api.heylua.ai HTTP API (chat generate/stream)
  format: Bearer YOUR_API_KEY
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  - changelog examples
  type: http
slug: lua-global-inc-authentication
source_filename: lua-global-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.heylua.ai/cli/authentication\ndocs: https://docs.heylua.ai/cli/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  http_scheme: bearer\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: \"Bearer YOUR_API_KEY\"\n    applies_to: https://api.heylua.ai HTTP API (chat generate/stream)\n    sources: [docs, changelog examples]\nprovisioning:\n  - method: email-otp\n    description: >-\n      Recommended. A 6-digit code is emailed and, on verification, an API key\n      is generated and saved automatically (via `lua auth`).\n  - method: existing-key\n    description: Supply a pre-existing key; it is validated and stored locally.\nkey_resolution_priority:\n  - LUA_API_KEY (environment variable — highest priority, CI/CD)\n  - ~/.lua-cli/credentials (local credentials file, 0600 perms)\n  - .env (local development\
  \ fallback)\nnotes: >-\n  API-key / bearer-token auth only — no OAuth2, OIDC, or mTLS surface, so no\n  scopes/ artifact. Keys are the complete credential. No published real OpenAPI\n  exists (the docs openapi.json is the Mintlify Plant Store placeholder), so\n  this profile is derived from the documented HTTP API + CLI auth pages.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lua-global-inc/refs/heads/main/authentication/lua-global-inc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Platform
- Developer Tools
- Model Context Protocol
- Conversational AI
- Chatbots
- Automation
---
