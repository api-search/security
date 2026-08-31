---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Freetts Authentication
name_suffix: Authentication
oauth_flows: []
overview: FreeTTS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FreeTTS
provider_slug: freetts
scheme_count: 2
schemes:
- applies_to:
  - POST /api/v1/tts
  - POST /api/tts-pro
  id: apiKeyHeader
  in: header
  issuance: Free account required; the docs state keys are only issued to accounts with a verified email address. Free plan gets 1 key, PRO and Creator up to 10. Revoking a key is documented as taking effect instantly.
  key_prefix: null
  key_prefix_note: FreeTTS publishes no key prefix convention. Every documented example uses an environment variable ($FREETTS_API_KEY) rather than a literal key, so there is no example token in the docs to record or to redact.
  name: x-api-key
  required: true
  rotation: revoke-and-remint from the dashboard; no documented rotation policy or key expiry
  type: apiKey
- applies_to:
  - GET /api/voices
  - GET /api/audio/{file_id}
  - GET /api/srt/{file_id}
  - GET /api/health
  id: none
  in: null
  name: null
  note: CONFIRMED BY PROBE. GET https://freetts.org/api/voices returned HTTP 200 with a 585,024-byte JSON array of 1,410 voice objects and no credential of any kind. GET /api/health returned 200 {"status":"ok","timestamp":...}. The audio and SRT download endpoints are unauthenticated too and are guarded only by the unguessable file_id UUID plus the 1-hour retention window - an access-control model worth naming, since a leaked file_id is the whole credential for that object until it expires.
  required: false
  type: public
slug: freetts-authentication
source_filename: freetts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://freetts.org/developers\nprobed: '2026-08-28'\nnote: >-\n  No OpenAPI exists for this provider, so derive-authentication.py had no\n  securitySchemes to read. This profile is written from the provider's own\n  developer documentation and confirmed against live unauthenticated probes of\n  the production API.\nsummary: >-\n  Single-scheme API-key auth. A key is minted in the FreeTTS dashboard under\n  \"API Keys\" and sent as the x-api-key request header. There is no OAuth, no\n  OpenID Connect, no mutual TLS, no bearer token and no scope surface, so no\n  scopes/ artifact is emitted.\nschemes:\n- id: apiKeyHeader\n  type: apiKey\n  in: header\n  name: x-api-key\n  applies_to:\n  - POST /api/v1/tts\n  - POST /api/tts-pro\n  required: true\n  key_prefix: null\n  key_prefix_note: >-\n    FreeTTS publishes no key prefix convention. Every documented example uses an\n    environment variable ($FREETTS_API_KEY) rather than\
  \ a literal key, so there\n    is no example token in the docs to record or to redact.\n  issuance: >-\n    Free account required; the docs state keys are only issued to accounts with\n    a verified email address. Free plan gets 1 key, PRO and Creator up to 10.\n    Revoking a key is documented as taking effect instantly.\n  rotation: revoke-and-remint from the dashboard; no documented rotation policy\n    or key expiry\n- id: none\n  type: public\n  in: null\n  name: null\n  applies_to:\n  - GET /api/voices\n  - GET /api/audio/{file_id}\n  - GET /api/srt/{file_id}\n  - GET /api/health\n  required: false\n  note: >-\n    CONFIRMED BY PROBE. GET https://freetts.org/api/voices returned HTTP 200\n    with a 585,024-byte JSON array of 1,410 voice objects and no credential of\n    any kind. GET /api/health returned 200 {\"status\":\"ok\",\"timestamp\":...}. The\n    audio and SRT download endpoints are unauthenticated too and are guarded\n    only by the unguessable file_id UUID plus the 1-hour\
  \ retention window - an\n    access-control model worth naming, since a leaked file_id is the whole\n    credential for that object until it expires.\nprobes:\n- url: https://freetts.org/api/v1/tts\n  method: POST\n  headers: none\n  status: 401\n  body: '{\"detail\":\"Missing x-api-key header\"}'\n- url: https://freetts.org/api/v1/tts\n  method: POST\n  headers: 'x-api-key: <deliberately invalid>'\n  status: 401\n  body: '{\"detail\":\"Invalid API key\"}'\n- url: https://freetts.org/api/voices\n  method: GET\n  headers: none\n  status: 200\n- url: https://freetts.org/api/health\n  method: GET\n  headers: none\n  status: 200\ndocumentation_conflict: >-\n  The /developers hero and the About page both advertise the API as \"No Key\n  Required\" / \"No API key required to get started\", while the same page's FAQ,\n  every code sample on it, and the live 401 all require x-api-key. The\n  marketing claim is wrong and the FAQ is right. This is worth raising with the\n  provider - it is the first\
  \ thing a developer reads and it is contradicted\n  sixty lines later.\ntransport:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\ncors:\n  enabled: false\n  source: >-\n    /developers \"Technical Notes\" states the API does not emit CORS headers by\n    default and directs browser callers to proxy through their own backend.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freetts/refs/heads/main/authentication/freetts-authentication.yml
summary_line: 2 schemes
tags:
- Text-to-Speech
- Speech Synthesis
- AI Voice
- Audio
- Media
- Accessibility
- Speech-to-Text
- Content Creation
- Developer Tools
---
