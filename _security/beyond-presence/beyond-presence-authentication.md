---
api_key_in:
- header
api_specs:
- filename: beyond-presence-openapi-original.json
  format: json
  label: Beyond Presence API
  slug: beyond-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-presence/refs/heads/main/openapi/beyond-presence-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Beyond Presence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beyond Presence secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Beyond Presence
provider_slug: beyond-presence
scheme_count: 1
schemes:
- description: Your Beyond Presence API Key.
  in: header
  name: APIKeyHeader
  parameter: x-api-key
  sources:
  - openapi/beyond-presence-openapi-original.json
  type: apiKey
slug: beyond-presence-authentication
source_filename: beyond-presence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/beyond-presence-openapi-original.json\ndocs: https://docs.bey.dev/api-reference/authentication/verify-api-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Beyond Presence authenticates every request with a single API key passed in\n  the x-api-key header. Keys are created and managed in the dashboard at\n  app.bey.chat. A dedicated GET /v1/auth/verify operation lets clients validate\n  a key before use. No OAuth 2.0 / OIDC surface is published.\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your Beyond Presence API Key.\n  sources:\n  - openapi/beyond-presence-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-presence/refs/heads/main/authentication/beyond-presence-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai Enterprise Software
- Artificial Intelligence
- Avatars
- Video
- Conversational AI
- Agents
- Speech To Video
- Real Time Communication
---
