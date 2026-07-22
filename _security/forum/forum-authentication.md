---
api_key_in:
- header
api_specs:
- filename: forum-openapi-original.yml
  format: yaml
  label: Forum API
  slug: forum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forum/refs/heads/main/openapi/forum-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Forum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forum secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Forum
provider_slug: forum
scheme_count: 3
schemes:
- description: Your API key ID (e.g. `fk_a1b2c3d4e5f6...`)
  in: header
  name: ForumAccessKey
  parameter: FORUM-ACCESS-KEY
  sources:
  - openapi/forum-openapi-original.yml
  type: apiKey
- description: Unix epoch in seconds (UTC), as a string
  in: header
  name: ForumAccessTimestamp
  parameter: FORUM-ACCESS-TIMESTAMP
  sources:
  - openapi/forum-openapi-original.yml
  type: apiKey
- description: 'Base64-encoded HMAC-SHA256 signature.


    **Signature generation:**

    ```

    prehash = timestamp + method + requestPath + body

    signature = Base64(HMAC-SHA256(secret, prehash))

    ```'
  in: header
  name: ForumAccessSign
  parameter: FORUM-ACCESS-SIGN
  sources:
  - openapi/forum-openapi-original.yml
  type: apiKey
slug: forum-authentication
source_filename: forum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/forum-openapi-original.yml\ndocs: https://docs.forum.market/api-reference/authentication\nmodel: hmac-signature\nmodel_notes: >-\n  Three apiKey headers combine into an HMAC-SHA256 request signature. FORUM-ACCESS-SIGN =\n  Base64(HMAC-SHA256(secret, timestamp + method + requestPath + body)). Timestamp\n  (FORUM-ACCESS-TIMESTAMP) must be within a 30-second window (else 401 TIMESTAMP_EXPIRED).\n  Keys are minted in app.forum.market with `read` or `trade` permission (key id `fk_...`,\n  secret `sk_...`, secret shown once). Public market-data endpoints need no auth.\npermissions:\n- read\n- trade\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ForumAccessKey\n  type: apiKey\n  in: header\n  parameter: FORUM-ACCESS-KEY\n  description: Your API key ID (e.g. `fk_a1b2c3d4e5f6...`)\n  sources:\n  - openapi/forum-openapi-original.yml\n- name: ForumAccessTimestamp\n  type: apiKey\n  in: header\n \
  \ parameter: FORUM-ACCESS-TIMESTAMP\n  description: Unix epoch in seconds (UTC), as a string\n  sources:\n  - openapi/forum-openapi-original.yml\n- name: ForumAccessSign\n  type: apiKey\n  in: header\n  parameter: FORUM-ACCESS-SIGN\n  description: |-\n    Base64-encoded HMAC-SHA256 signature.\n\n    **Signature generation:**\n    ```\n    prehash = timestamp + method + requestPath + body\n    signature = Base64(HMAC-SHA256(secret, prehash))\n    ```\n  sources:\n  - openapi/forum-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forum/refs/heads/main/authentication/forum-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Trading
- Exchange
- Perpetual Futures
- Market Data
- Attention Economy
- Fintech
- WebSocket
- Real Time
---
