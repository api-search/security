---
api_key_in:
- header
api_specs:
- filename: reactor-helios-asyncapi.yml
  format: yaml
  label: Reactor Realtime Video API
  slug: reactor-realtime-video-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/reactor/refs/heads/main/asyncapi/reactor-helios-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Reactor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reactor secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Reactor
provider_slug: reactor
scheme_count: 2
schemes:
- in: header
  name: ReactorAPIKey
  note: Long-lived account key (rk_...); used only server-side against the /tokens endpoint.
  parameter: Reactor-API-Key
  type: apiKey
- bearerFormat: JWT
  name: SessionJWT
  note: Short-lived session-scoped token returned by POST /tokens; passed to the SDK to open a model connection.
  scheme: bearer
  type: http
slug: reactor-authentication
source_filename: reactor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.reactor.inc/authentication\ndocs: https://docs.reactor.inc/authentication\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  api_key_prefix: \"rk_\"\n  token_type: JWT\nmodel: >-\n  Reactor uses a two-stage credential model. A long-lived account API key\n  (prefix rk_, created in the dashboard under API Keys) is exchanged server-side\n  for a short-lived, session-scoped JWT via POST https://api.reactor.inc/tokens.\n  Browser/client code never sees the API key — only the minted JWT is passed to\n  the SDK. The Python SDK performs the exchange automatically on connect().\nschemes:\n  - name: ReactorAPIKey\n    type: apiKey\n    in: header\n    parameter: Reactor-API-Key\n    note: Long-lived account key (rk_...); used only server-side against the /tokens endpoint.\n  - name: SessionJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    note: Short-lived session-scoped token returned by POST\
  \ /tokens; passed to the SDK to open a model connection.\ntoken_exchange:\n  endpoint: POST https://api.reactor.inc/tokens\n  request_header: \"Reactor-API-Key: rk_...\"\n  request_body_example:\n    authorization_details:\n      - type: session\n        resources:\n          models:\n            match: [\"helios\"]\n        constraints:\n          max_sessions: 5\n    expires_after: 3600\n  response_example:\n    jwt: \"<jwt>\"\n    expires_at: 1234567890\n  scoping: >-\n    authorization_details of type \"session\" restrict a token to named models\n    (no wildcards) and to managing its own sessions only — no account API or key\n    management. Omitting authorization_details mints an unscoped full-account\n    token (never expose to browsers).\n  expiry: default 3600s (1h), configurable via expires_after up to a 6h server ceiling\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reactor/refs/heads/main/authentication/reactor-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai Ml
- Video
- Generative AI
- Real-Time
- WebRTC
- Streaming
- SDK
- Media
---
