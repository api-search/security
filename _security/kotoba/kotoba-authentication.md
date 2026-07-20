---
api_key_in:
- header
api_specs:
- filename: kotoba-transcription-openapi-original.yml
  format: yaml
  label: Kotoba Transcription API (Batch REST)
  slug: kotoba-transcription-api-batch-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-transcription-openapi-original.yml
- filename: kotoba-asr-realtime-openapi-original.yml
  format: yaml
  label: Kotoba ASR Realtime API (WebSocket)
  slug: kotoba-asr-realtime-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-asr-realtime-openapi-original.yml
- filename: kotoba-sts-realtime-openapi-original.yml
  format: yaml
  label: Kotoba Speech-to-Speech Translation API (WebSocket)
  slug: kotoba-speech-to-speech-translation-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-sts-realtime-openapi-original.yml
- filename: kotoba-tts-realtime-openapi-original.yml
  format: yaml
  label: Kotoba TTS Realtime API (WebSocket)
  slug: kotoba-tts-realtime-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-tts-realtime-openapi-original.yml
auth_types:
- http
- client-secret
description: ''
kind: authentication
layout: security
method: searched
name: Kotoba Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kotoba secures its APIs with http and client-secret across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kotoba
provider_slug: kotoba
scheme_count: 3
schemes:
- description: 'HTTP Bearer authentication. Pass the Kotoba API key as a Bearer

    token via the Authorization header. Server-side use only.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kotoba-asr-realtime-openapi-original.yml
  - openapi/kotoba-tts-realtime-openapi-original.yml
  type: http
- description: 'HTTP Basic authentication. Set device_id as the username and api_key

    as the password. Send it via the Authorization header during the

    WebSocket handshake.'
  name: httpBasic
  scheme: basic
  sources:
  - openapi/kotoba-sts-realtime-openapi-original.yml
  type: http
- description: 'Browser / client-side flow. Browsers cannot set arbitrary headers on a

    WebSocket handshake, so the backend mints a short-lived client secret by

    calling POST https://api.kotobatech.ai/v1/realtime/transcription_sessions,

    passes it to the browser, and the browser supplies it through the

    Sec-WebSocket-Protocol header. Documented but not present in any published

    spec. No browser-side SDK is available yet.'
  format: realtime, kotoba-insecure-api-key.<CLIENT_SECRET>
  in: header
  mint_endpoint: https://api.kotobatech.ai/v1/realtime/transcription_sessions
  name: browserClientSecret
  parameter: Sec-WebSocket-Protocol
  short_lived: true
  sources:
  - https://docs.kotoba.tech/overview/authentication
  type: client-secret
slug: kotoba-authentication
source_filename: kotoba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kotoba-asr-realtime-openapi-original.yml, openapi/kotoba-sts-realtime-openapi-original.yml,\n  openapi/kotoba-tts-realtime-openapi-original.yml\ndocs: https://docs.kotoba.tech/overview/authentication\nnotes: >-\n  Derived from the published securitySchemes, then upgraded from the docs auth\n  page. All Kotoba realtime APIs authenticate during the WebSocket handshake.\n  The docs describe a third, browser-oriented flow that is NOT expressed in any\n  published spec: mint a short-lived client secret server-side and pass it via\n  the Sec-WebSocket-Protocol subprotocol header. There is no OAuth 2.0 or OIDC\n  surface — `scopes/` is intentionally absent for this provider.\nsummary:\n  types:\n  - http\n  - client-secret\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    HTTP Bearer authentication. Pass\
  \ the Kotoba API key as a Bearer\n    token via the Authorization header. Server-side use only.\n  sources:\n  - openapi/kotoba-asr-realtime-openapi-original.yml\n  - openapi/kotoba-tts-realtime-openapi-original.yml\n- name: httpBasic\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic authentication. Set device_id as the username and api_key\n    as the password. Send it via the Authorization header during the\n    WebSocket handshake.\n  sources:\n  - openapi/kotoba-sts-realtime-openapi-original.yml\n- name: browserClientSecret\n  type: client-secret\n  in: header\n  parameter: Sec-WebSocket-Protocol\n  format: 'realtime, kotoba-insecure-api-key.<CLIENT_SECRET>'\n  description: |-\n    Browser / client-side flow. Browsers cannot set arbitrary headers on a\n    WebSocket handshake, so the backend mints a short-lived client secret by\n    calling POST https://api.kotobatech.ai/v1/realtime/transcription_sessions,\n    passes it to the browser, and the browser supplies it through\
  \ the\n    Sec-WebSocket-Protocol header. Documented but not present in any published\n    spec. No browser-side SDK is available yet.\n  mint_endpoint: https://api.kotobatech.ai/v1/realtime/transcription_sessions\n  short_lived: true\n  sources:\n  - https://docs.kotoba.tech/overview/authentication\nguidance:\n  server_side_recommended: true\n  warning: Never embed long-lived API keys in browser-side code.\n  env_var: KOTOBA_API_KEY\n  sdk: kotoba-sdk (Python) reads KOTOBA_API_KEY from the environment by default\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/authentication/kotoba-authentication.yml
summary_line: http/client-secret · 3 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Voice
- Speech Recognition
- Speech to Text
- Text to Speech
- Translation
- Real Time
- WebSockets
- Audio
- Transcription
---
