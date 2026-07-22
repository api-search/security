---
api_key_in: []
api_specs:
- filename: voiceitt-rest-api-openapi-original.json
  format: json
  label: Voiceitt HTTP API
  slug: voiceitt-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voiceitt/refs/heads/main/openapi/voiceitt-rest-api-openapi-original.json
- filename: voiceitt-websockets-asyncapi.yml
  format: yaml
  label: Voiceitt WebSockets API
  slug: voiceitt-websockets-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/voiceitt/refs/heads/main/asyncapi/voiceitt-websockets-asyncapi.yml
auth_types:
- http
description: Voiceitt uses JSON Web Tokens (JWT) for authenticated sessions. Apps obtain tokens by POSTing an App ID and API key to /v1/auth/login/user_id (speaker-independent mode, optionally scoped to a user_id) or App ID, API key, email and password to /v1/auth/login/email (personalized mode — the end user must first enroll and train at https://web.voiceitt.com/). The returned JWT is passed as a Bearer token in the HTTP header of each call to the transcribe endpoint, or in the auth option (token + refresh_token) when initializing a WebSockets (Socket.IO) connection. Tokens carry token_expires_at / refresh_token_expires_at timestamps and are renewed by POSTing the refresh_token to /v1/auth/refresh_token (HTTP) or emitting the refresh_token event (WebSockets).
kind: authentication
layout: security
method: searched
name: Voiceitt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voiceitt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voiceitt
provider_slug: voiceitt
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/voiceitt-rest-api-openapi-original.json
  token_endpoints:
  - /v1/auth/login/user_id
  - /v1/auth/login/email
  - /v1/auth/refresh_token
  type: http
slug: voiceitt-authentication
source_filename: voiceitt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/voiceitt-rest-api-openapi-original.json\ndocs: https://voiceitt-si-api.readme.io/reference/getting-started-with-the-voiceitt-rest-api-copy\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  credential_issuance: App ID + API key issued via the Voiceitt developer portal (developer.voiceitt.com)\ndescription: >-\n  Voiceitt uses JSON Web Tokens (JWT) for authenticated sessions. Apps obtain\n  tokens by POSTing an App ID and API key to /v1/auth/login/user_id\n  (speaker-independent mode, optionally scoped to a user_id) or App ID, API\n  key, email and password to /v1/auth/login/email (personalized mode — the\n  end user must first enroll and train at https://web.voiceitt.com/). The\n  returned JWT is passed as a Bearer token in the HTTP header of each call to\n  the transcribe endpoint, or in the auth option (token + refresh_token) when\n  initializing a WebSockets (Socket.IO) connection. Tokens carry\n  token_expires_at\
  \ / refresh_token_expires_at timestamps and are renewed by\n  POSTing the refresh_token to /v1/auth/refresh_token (HTTP) or emitting the\n  refresh_token event (WebSockets).\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  token_endpoints:\n  - /v1/auth/login/user_id\n  - /v1/auth/login/email\n  - /v1/auth/refresh_token\n  sources:\n  - openapi/voiceitt-rest-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voiceitt/refs/heads/main/authentication/voiceitt-authentication.yml
summary_line: http · 1 scheme
tags:
- Speech Recognition
- Speech-to-Text
- Voice
- Accessibility
- Assistive Technology
- Artificial Intelligence
- Transcription
- Captioning
- Company
---
