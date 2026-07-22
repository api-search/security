---
api_key_in:
- sdk-constructor
auth_types:
- apiKey
- bearer-jwt
description: ''
kind: authentication
layout: security
method: searched
name: Odyssey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Odyssey secures its APIs with apiKey and bearer-jwt across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Odyssey
provider_slug: odyssey
scheme_count: 3
schemes:
- description: 'Server-side API key, prefixed `ody_`, obtained from the developer dashboard. Passed to the SDK constructor (`new Odyssey({ apiKey: ''ody_...'' })` / `Odyssey(api_key=''ody_...'')`). Must stay server-side; never shipped to a browser.'
  issued_at: https://developer.odyssey.ml/dashboard
  key_prefix: ody_
  name: apiKey
  type: apiKey
- bearerFormat: JWT
  description: Browser/edge connection pattern. The server mints a short-lived session token with `createClientCredentials()`; the browser connects with `connectWithCredentials()` and never sees the API key. The returned `session_token` is a JWT locked to a single `session_id`.
  fields:
  - session_id
  - signaling_url
  - session_token
  - expires_in
  - capabilities
  name: clientCredentials
  scheme: bearer
  token_lifetime_seconds: 600
  token_refresh: false
  type: bearer-jwt
- bearerFormat: JWT
  description: View-only Broadcast credential (`spectator_token`) that lets many viewers watch one shared stream via `connectToStream()` without interaction rights.
  name: spectatorToken
  scheme: bearer
  source: https://documentation.api.odyssey.ml/broadcast
  type: bearer-jwt
slug: odyssey-authentication
source_filename: odyssey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://documentation.api.odyssey.ml/client-credentials\ndocs: https://documentation.api.odyssey.ml/api-quick-start\nsummary:\n  types: [apiKey, bearer-jwt]\n  api_key_in: [sdk-constructor]\n  oauth2_flows: []\n  note: >-\n    No OpenAPI is published (the surface is a WebRTC/WebSocket streaming SDK), so\n    this profile is captured from the documentation rather than derived from a\n    spec.\nschemes:\n- name: apiKey\n  type: apiKey\n  description: >-\n    Server-side API key, prefixed `ody_`, obtained from the developer dashboard.\n    Passed to the SDK constructor (`new Odyssey({ apiKey: 'ody_...' })` /\n    `Odyssey(api_key='ody_...')`). Must stay server-side; never shipped to a browser.\n  key_prefix: \"ody_\"\n  issued_at: https://developer.odyssey.ml/dashboard\n- name: clientCredentials\n  type: bearer-jwt\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Browser/edge connection pattern. The server mints\
  \ a short-lived session token\n    with `createClientCredentials()`; the browser connects with\n    `connectWithCredentials()` and never sees the API key. The returned\n    `session_token` is a JWT locked to a single `session_id`.\n  token_lifetime_seconds: 600\n  token_refresh: false\n  fields: [session_id, signaling_url, session_token, expires_in, capabilities]\n- name: spectatorToken\n  type: bearer-jwt\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    View-only Broadcast credential (`spectator_token`) that lets many viewers\n    watch one shared stream via `connectToStream()` without interaction rights.\n  source: https://documentation.api.odyssey.ml/broadcast\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odyssey/refs/heads/main/authentication/odyssey-authentication.yml
summary_line: apiKey/bearer-jwt · 3 schemes
tags:
- Company
- Artificial Intelligence
- World Models
- Generative AI
- Video Generation
- Machine Learning
- Real-Time Streaming
- SDK
- WebRTC
---
