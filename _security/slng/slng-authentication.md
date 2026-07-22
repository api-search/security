---
api_key_in: []
api_specs:
- filename: slng-stt-slng-openapi.yml
  format: yaml
  label: SLNG Gateway API
  slug: slng-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-stt-slng-openapi.yml
- filename: slng-agents-openapi.yml
  format: yaml
  label: SLNG Voice Agents API
  slug: slng-voice-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-agents-openapi.yml
- filename: slng-batch-openapi.json
  format: json
  label: SLNG Batch API
  slug: slng-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-batch-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Slng Authentication
name_suffix: Authentication
oauth_flows: []
overview: SLNG secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SLNG
provider_slug: slng
scheme_count: 1
schemes:
- bearerFormat: API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/slng-agents-openapi.yml
  - openapi/slng-batch-openapi.json
  - openapi/slng-management-slng-openapi.yml
  - openapi/slng-me-openapi.json
  - openapi/slng-stt-slng-openapi.yml
  - openapi/slng-tts-pronunciation-dictionaries-openapi.yml
  - openapi/slng-tts-slng-openapi.yml
  type: http
slug: slng-authentication
source_filename: slng-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.slng.ai/authentication.md\ndocs: https://docs.slng.ai/authentication.md\nsummary:\n  types:\n  - http\n  style: bearer-token\n  header: 'Authorization: Bearer <SLNG_API_KEY>'\n  key_management: Keys created/deleted at https://app.slng.ai/api-keys; secret shown once at creation, not retrievable later.\n  rotation: Keys cannot be rotated in place; create a new key and cut over, then delete the old one.\n  websocket_auth: Authorization header, or a `token` query parameter for browser clients that cannot set headers.\n  byok: Add an `X-Slng-Provider-Key` header alongside the SLNG key to run against your own upstream provider account (Bring Your Own Key).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/slng-agents-openapi.yml\n  - openapi/slng-batch-openapi.json\n  - openapi/slng-management-slng-openapi.yml\n  - openapi/slng-me-openapi.json\n  - openapi/slng-stt-slng-openapi.yml\n\
  \  - openapi/slng-tts-pronunciation-dictionaries-openapi.yml\n  - openapi/slng-tts-slng-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/authentication/slng-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Speech
- Voice
- Speech to Text
- Text to Speech
- Voice AI
- Voice Agents
- Transcription
- Speech Recognition
- Artificial Intelligence
- API Gateway
---
