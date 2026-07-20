---
api_key_in:
- header
api_specs:
- filename: kalpa-labs-openapi-original.json
  format: json
  label: Kalpa Speech API
  slug: kalpa-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalpa-labs/refs/heads/main/openapi/kalpa-labs-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kalpa Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kalpa Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kalpa Labs
provider_slug: kalpa-labs
scheme_count: 1
schemes:
- description: Every /v1/* endpoint authenticates with a per-team API key, sent as a bearer token in the Authorization header (preferred) or in the X-API-Key header. A missing or invalid key returns 401 authentication_error; if key verification is temporarily unavailable the API returns 503 service_unavailable (retry, do not treat as invalid).
  header_alternate: X-API-Key
  header_primary: Authorization
  header_primary_format: Bearer <key>
  in: header
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/kalpa-labs-openapi-original.json
  type: apiKey
slug: kalpa-labs-authentication
source_filename: kalpa-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kalpa-labs-openapi-original.json\ndocs: https://docs.kalpalabs.ai/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  provisioning: per-team, early access (request via hello@kalpalabs.ai)\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  scheme: bearer\n  header_primary: Authorization\n  header_primary_format: 'Bearer <key>'\n  header_alternate: X-API-Key\n  description: >-\n    Every /v1/* endpoint authenticates with a per-team API key, sent as a bearer\n    token in the Authorization header (preferred) or in the X-API-Key header.\n    A missing or invalid key returns 401 authentication_error; if key verification\n    is temporarily unavailable the API returns 503 service_unavailable (retry, do\n    not treat as invalid).\n  sources:\n  - openapi/kalpa-labs-openapi-original.json\nnotes:\n  - Keys are secret; call the API server-side, never from browsers or shipped apps.\n  - Keys\
  \ are rotated / limits raised by contacting hello@kalpalabs.ai.\n  - Each key carries its own rate limits and its own usage meter (GET /v1/usage).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalpa-labs/refs/heads/main/authentication/kalpa-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Speech
- Text to Speech
- Voice
- Audio
- Conversational AI
- Machine Learning
- Artificial Intelligence
---
