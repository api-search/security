---
api_key_in: []
api_specs:
- filename: unitary-ai-content-classification-openapi-original.yaml
  format: yaml
  label: Unitary Content Classification API
  slug: unitary-content-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/openapi/unitary-ai-content-classification-openapi-original.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Unitary Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unitary AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unitary AI
provider_slug: unitary-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: JWTBearer
  scheme: bearer
  sources:
  - openapi/unitary-ai-content-classification-openapi-original.yaml
  token_endpoint: https://api.unitary.ai/v1/authenticate
  token_ttl: 24h
  type: http
slug: unitary-ai-authentication
source_filename: unitary-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unitary-ai-content-classification-openapi-original.yaml\ndocs: https://docs.unitary.ai/api-references/authentication\nsummary:\n  types:\n  - http\n  flow: api-key-for-token exchange\n  notes: >-\n    API keys are issued by Unitary (email support@unitary.ai — no self-serve\n    signup). POST https://api.unitary.ai/v1/authenticate with form field\n    key={API_KEY} (application/x-www-form-urlencoded) returns {api_token,\n    expiry}; the api_token is a JWT valid for ~24 hours and is sent as\n    Authorization: Bearer {api_token} on all other endpoints. /authenticate is\n    rate-limited — clients must re-use tokens until expiry. A separate preshared\n    secret (issued with the API key) signs webhook payloads via the\n    X-Hub-Signature-256 header (base64 HMAC-SHA256).\nschemes:\n- name: JWTBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  token_ttl: 24h\n  token_endpoint: https://api.unitary.ai/v1/authenticate\n\
  \  sources:\n  - openapi/unitary-ai-content-classification-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/authentication/unitary-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Saas
- Content Moderation
- Trust And Safety
- Artificial Intelligence
- Machine Learning
- Computer Vision
- Video
- Virtual Agents
---
