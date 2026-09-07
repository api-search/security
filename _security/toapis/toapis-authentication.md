---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Toapis Authentication
name_suffix: Authentication
oauth_flows: []
overview: ToAPIs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ToAPIs
provider_slug: toapis
scheme_count: 1
schemes:
- applies_to: all endpoints on https://toapis.com/v1 (and https://toapis.cn for mainland China)
  header: 'Authorization: Bearer <key>'
  key_prefix: sk-
  name: API key (Bearer token)
  scheme: bearer
  type: http
slug: toapis-authentication
source_filename: toapis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://docs.toapis.com/docs/cn/quickstart.md\ndocs: https://docs.toapis.com/docs/cn/quickstart\nnotes: >-\n  No OpenAPI is published, so this profile is read from the documentation. Every\n  endpoint uses the same scheme; there is no OAuth, no scopes, and no mTLS. Keys are\n  created in the console (https://toapis.com/console/token) or via the\n  POST /v1/account/tokens API; a key's secret is returned exactly once at creation.\nschemes:\n  - type: http\n    scheme: bearer\n    name: API key (Bearer token)\n    header: 'Authorization: Bearer <key>'\n    key_prefix: sk-\n    applies_to: all endpoints on https://toapis.com/v1 (and https://toapis.cn for mainland China)\nkey_management:\n  console: https://toapis.com/console/token\n  api: POST /v1/account/tokens (create tokens with name, expiry, quota, model restrictions)\n  controls:\n    - per-token expiry (Unix timestamp or -1 for never)\n    - per-token total quota / credits\
  \ (200 credits = 1 USD)\n    - per-token daily and monthly credit limits\n    - per-token model restrictions\n  rate_limit_scope: per user ID — all tokens of one user share rate-limit buckets\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toapis/refs/heads/main/authentication/toapis-authentication.yml
summary_line: 1 scheme
tags:
- AI API
- LLM/AI gateway
- model aggregation
- OpenAI-compatible
- model routing
- provider failover
- text generation
- image generation
- video generation
- developer tools
---
