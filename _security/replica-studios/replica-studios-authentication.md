---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Replica Studios Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replica Studios secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Replica Studios
provider_slug: replica-studios
scheme_count: 2
schemes:
- description: API Key auth. Documented as the quick/simple integration method, usable to generate text-to-speech, speech-to-speech, and to retrieve the voice list. Personal Access Tokens are created from Account settings in the Replica desktop application (subscription with API access required).
  in: header
  name: apiKey
  type: apiKey
- bearerFormat: JWT
  description: 'Bearer token (JWT) auth, sent as the `Authorization: Bearer <jwt>` header. A Personal Access Token client_id and secret are exchanged at the POST /v2/auth endpoint to mint a short-lived JWT plus a refresh token. Documented as the more secure/powerful option.'
  name: bearerJWT
  scheme: bearer
  token_endpoint: /v2/auth
  type: http
slug: replica-studios-authentication
source_filename: replica-studios-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.replicastudios.com/guide/authentication\ndocs: https://docs.replicastudios.com/guide/authentication\nnotes: >-\n  Replica Studios ceased operations on 2025-06-30; api.replicastudios.com no\n  longer resolves. This profile captures the historical, publicly documented\n  authentication model from the archived Replica API v2 documentation. No\n  OpenAPI could be captured (docs host rejects non-browser TLS), so exact\n  header/parameter names are recorded only where the docs state them.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    description: >-\n      API Key auth. Documented as the quick/simple integration method, usable to\n      generate text-to-speech, speech-to-speech, and to retrieve the voice list.\n      Personal Access Tokens are created from Account settings in the Replica\n      desktop application\
  \ (subscription with API access required).\n  - name: bearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Bearer token (JWT) auth, sent as the `Authorization: Bearer <jwt>` header.\n      A Personal Access Token client_id and secret are exchanged at the\n      POST /v2/auth endpoint to mint a short-lived JWT plus a refresh token.\n      Documented as the more secure/powerful option.\n    token_endpoint: /v2/auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replica-studios/refs/heads/main/authentication/replica-studios-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Voice
- Text to Speech
- Speech to Speech
- AI
- Audio
- Voice AI
- Generative AI
---
