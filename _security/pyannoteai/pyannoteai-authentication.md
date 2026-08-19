---
api_key_in:
- header
api_specs:
- filename: pyannoteai-api-openapi.yml
  format: yaml
  label: pyannoteAI API
  slug: pyannoteai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyannoteai/refs/heads/main/openapi/pyannoteai-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pyannoteai Authentication
name_suffix: Authentication
oauth_flows: []
overview: PyannoteAI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PyannoteAI
provider_slug: pyannoteai
scheme_count: 1
schemes:
- bearerFormat: JWT
  docs: https://docs.pyannote.ai/authentication
  name: api-key
  note: 'Every REST endpoint is authenticated with the team API key presented as a bearer token in the Authorization header (Authorization: Bearer <apikey>). The OpenAPI declares bearerFormat JWT. Keys are generated and rotated in the dashboard at https://dashboard.pyannote.ai. There is no OAuth 2.0 / OpenID Connect surface, so no scopes/ artifact is emitted.'
  scheme: bearer
  sources:
  - openapi/pyannoteai-api-openapi.yml
  type: http
slug: pyannoteai-authentication
source_filename: pyannoteai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://docs.pyannote.ai/authentication\ndocs: https://docs.pyannote.ai/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: api-key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/pyannoteai-api-openapi.yml\n  docs: https://docs.pyannote.ai/authentication\n  note: >-\n    Every REST endpoint is authenticated with the team API key presented as a bearer token in the\n    Authorization header (Authorization: Bearer <apikey>). The OpenAPI declares bearerFormat JWT.\n    Keys are generated and rotated in the dashboard at https://dashboard.pyannote.ai. There is no\n    OAuth 2.0 / OpenID Connect surface, so no scopes/ artifact is emitted.\ncredentials:\n  issuance: https://dashboard.pyannote.ai\n  scope: team\n  rotation: self-service in the dashboard\nadditional_credentials:\n- name: stream session token\n  type: url-embedded single-use token\n\
  \  where: query parameter on the WebSocket URL returned by POST /v1/live\n  source: asyncapi/pyannoteai-streaming-asyncapi.yml\n  note: >-\n    The streaming WebSocket gateway is NOT authenticated with the team API key. POST /v1/live returns a\n    generated WebSocket URL carrying a single-use token that grants access only to that stream session\n    and carries no team credentials. Documented verbatim in the provider's AsyncAPI channel bindings.\n- name: webhook signing secret\n  type: shared secret (HMAC-SHA256)\n  where: X-Signature + X-Request-Timestamp request headers on inbound webhooks\n  docs: https://docs.pyannote.ai/webhooks/verifying-webhooks\n  note: >-\n    Per-team secret used to verify pyannoteAI -> customer webhook callbacks. Signed content is\n    \"v0:{timestamp}:{body}\" hashed with HMAC-SHA256 and compared against X-Signature. Rotatable from the\n    dashboard Webhooks page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pyannoteai/refs/heads/main/authentication/pyannoteai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Data
- Speech Recognition
- Speaker Diarization
- Audio
- Voice AI
- Machine Learning
- Transcription
- Streaming
- Webhooks
---
