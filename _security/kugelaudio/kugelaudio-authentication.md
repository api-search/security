---
api_key_in:
- header
- query
api_specs:
- filename: kugelaudio-tts-openapi-original.json
  format: json
  label: KugelAudio TTS API
  slug: tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-tts-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kugelaudio Authentication
name_suffix: Authentication
oauth_flows: []
overview: KugelAudio secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: KugelAudio
provider_slug: kugelaudio
scheme_count: 3
schemes:
- docs: https://docs.kugelaudio.com/api-reference/authentication
  format: 'Authorization: Bearer [example key]'
  in: header
  name: BearerApiKey
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.kugelaudio.com/api-reference/authentication
  transport:
  - https
  type: http
- docs: https://docs.kugelaudio.com/api-reference/raw-api
  in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - https://docs.kugelaudio.com/api-reference/raw-api
  transport:
  - https
  type: apiKey
- in: query
  name: ApiKeyQuery
  note: WebSocket endpoints (/ws/tts, /ws/tts/stream, /ws/tts/multi) accept the key as a query parameter; an Authorization header is also accepted where the client supports it.
  parameter: api_key
  sources:
  - https://docs.kugelaudio.com/api-reference/authentication
  transport:
  - wss
  type: apiKey
slug: kugelaudio-authentication
source_filename: kugelaudio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.kugelaudio.com/openapi.json\ndocs: https://docs.kugelaudio.com/api-reference/authentication\nnotes: >-\n  Searched from the docs rather than derived: the published OpenAPI 3.1 document\n  at https://api.kugelaudio.com/openapi.json declares NO components.securitySchemes\n  and no root-level security requirement, even though every documented endpoint\n  requires an API key. The auth model below is captured from the authentication\n  and raw-API docs pages. This gap is recorded in review notes as a concrete fix\n  for the provider.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  oauth2: false\n  scopes_supported: false\nschemes:\n  - name: BearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Bearer [example key]'\n    transport: [https]\n    docs: https://docs.kugelaudio.com/api-reference/authentication\n\
  \    sources: [https://docs.kugelaudio.com/api-reference/authentication]\n  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    transport: [https]\n    docs: https://docs.kugelaudio.com/api-reference/raw-api\n    sources: [https://docs.kugelaudio.com/api-reference/raw-api]\n  - name: ApiKeyQuery\n    type: apiKey\n    in: query\n    parameter: api_key\n    transport: [wss]\n    note: >-\n      WebSocket endpoints (/ws/tts, /ws/tts/stream, /ws/tts/multi) accept the key\n      as a query parameter; an Authorization header is also accepted where the\n      client supports it.\n    sources: [https://docs.kugelaudio.com/api-reference/authentication]\nkey_management:\n  issued_at: https://kugelaudio.com/dashboard\n  path: Dashboard -> Settings -> API Keys\n  shown_once: true\n  revocable: true\n  revocation_effect: immediate\n  rotation_guidance: >-\n    Docs recommend periodic rotation and separate keys per environment\n    (development, staging, production).\n\
  \  environment_variable: KUGELAUDIO_API_KEY\n  scoped_permissions: false\n  scoped_permissions_note: >-\n    \"All API keys have full access to your account's resources. We're working on\n    scoped permissions for future releases.\" — docs, 2026-07-19.\n  region_routing: >-\n    Prefixing a key with `eu-` routes to the direct EU endpoint\n    (https://api.eu.kugelaudio.com) instead of the geo-routed canonical host.\nclient_side_guidance: >-\n  Docs explicitly warn against using keys in frontend JavaScript, mobile app\n  source, public repositories, or client-side environment variables.\nauth_errors:\n  - {status: 401, error_code: UNAUTHORIZED, meaning: API key missing, invalid, or revoked}\n  - {status: 403, error_code: UNAUTHORIZED, meaning: Key valid but cannot access the requested resource}\n  - {ws_close_code: 4001, error_code: UNAUTHORIZED, meaning: WebSocket authentication failed}\nrelated:\n  - errors/kugelaudio-error-codes.yml\n  - conventions/kugelaudio-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/authentication/kugelaudio-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Voice
- Text to Speech
- Speech Synthesis
- Voice AI
- Voice Cloning
- Audio
- Artificial Intelligence
- Machine Learning
- Streaming
- Real Time
- Conversational AI
- Europe
- Data Sovereignty
- GDPR
- Company
---
