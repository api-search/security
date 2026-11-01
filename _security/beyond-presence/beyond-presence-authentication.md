---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: beyond-presence-agents-api-openapi.yml
  format: yaml
  label: Beyond Presence Agents API
  slug: beyond-presence-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-agents-api-openapi.yml
- filename: beyond-presence-authentication-api-openapi.yml
  format: yaml
  label: Beyond Presence Authentication API
  slug: beyond-presence-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-authentication-api-openapi.yml
- filename: beyond-presence-avatars-api-openapi.yml
  format: yaml
  label: Beyond Presence Avatars API
  slug: beyond-presence-avatars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-avatars-api-openapi.yml
- filename: beyond-presence-agent-conversations-api-openapi.yml
  format: yaml
  label: Beyond Presence Agent Conversations API
  slug: beyond-presence-agent-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-agent-conversations-api-openapi.yml
- filename: beyond-presence-agent-integration-api-openapi.yml
  format: yaml
  label: Beyond Presence Agent Integration API
  slug: beyond-presence-agent-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-agent-integration-api-openapi.yml
- filename: beyond-presence-agent-knowledge-files-api-openapi.yml
  format: yaml
  label: Beyond Presence Agent Knowledge Files API
  slug: beyond-presence-agent-knowledge-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-agent-knowledge-files-api-openapi.yml
- filename: beyond-presence-agents-external-apis-api-openapi.yml
  format: yaml
  label: Beyond Presence Agents External APIs API
  slug: beyond-presence-agents-external-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-agents-external-apis-api-openapi.yml
- filename: beyond-presence-speech-to-video-sessions-api-openapi.yml
  format: yaml
  label: Beyond Presence Speech-to-Video Sessions API
  slug: beyond-presence-speech-to-video-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyond-presence/openapi/beyond-presence-speech-to-video-sessions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/beyond-presence/authentication/beyond-presence-authentication.yml
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
- Real-Time Communication
- A2A
---
