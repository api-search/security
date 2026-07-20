---
api_key_in: []
api_specs:
- filename: coactive-openapi-original.json
  format: json
  label: Coactive API
  slug: coactive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coactive/refs/heads/main/openapi/coactive-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Coactive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coactive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coactive
provider_slug: coactive
scheme_count: 1
schemes:
- bearer_format: access_token
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/coactive-openapi-original.json
  type: http
slug: coactive-authentication
source_filename: coactive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/coactive-openapi-original.json\ndocs: https://docs.coactive.ai/api-reference/authentication/api-authentication\nsummary:\n  types:\n  - http\n  token_model: bearer-access-token\n  token_exchange: POST https://api.coactive.ai/api/v0/login\n  access_token_ttl_seconds: 3600\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearer_format: access_token\n  sources:\n  - openapi/coactive-openapi-original.json\ncredential_types:\n- name: PERSONAL_TOKEN\n  description: User-scoped personal token created in the Coactive UI (app.coactive.ai/settings/credentials).\n    Expires after 30 days unused or 3 months from creation; cannot be retrieved after\n    creation (regenerate to obtain a new one).\n  exchange:\n    endpoint: POST https://api.coactive.ai/api/v0/login\n    auth: bearer PERSONAL_TOKEN\n    grant_type: refresh_token\n- name: SYSTEM_CREDENTIALS\n  description: Administrator CLIENT_ID + CLIENT_SECRET (system\
  \ credentials) that do not\n    expire. Managed via the systemCredentials API and the Coactive UI.\n  exchange:\n    endpoint: POST https://api.coactive.ai/api/v0/login\n    auth: HTTP Basic CLIENT_ID:CLIENT_SECRET\n    grant_type: client_credentials\naccess_token:\n  token_type: Bearer\n  expires_in: 3600\n  usage: 'Authorization: Bearer <access_token> on every subsequent API request.'\nscopes:\n  documented: false\n  notes: No granular OAuth scopes are documented; a valid access token grants API access\n    per the caller's credential type and role. No scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coactive/refs/heads/main/authentication/coactive-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Multimodal AI
- Computer Vision
- Video Intelligence
- Image Search
- Content Intelligence
- Semantic Search
- Contextual Advertising
- Metadata
- Machine Learning
- Media
---
