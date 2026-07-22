---
api_key_in:
- body
api_specs:
- filename: tenyks-openapi.json
  format: json
  label: Tenyks API
  slug: tenyks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenyks/refs/heads/main/openapi/tenyks-openapi.json
auth_types:
- http
- apiKey-exchange
description: ''
kind: authentication
layout: security
method: searched
name: Tenyks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tenyks secures its APIs with http and apiKey-exchange across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tenyks
provider_slug: tenyks
scheme_count: 1
schemes:
- description: Bearer access token obtained from POST /api/auth/apikey. Applied to every dataset/model/prediction endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tenyks-openapi.json
  type: http
slug: tenyks-authentication
source_filename: tenyks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://docs.tenyks.ai/reference/access-token.md and\n  https://docs.tenyks.ai/reference/retrieving-api-keys.md, corroborated by the\n  bearerAuth securityScheme in openapi/tenyks-openapi.json.\ndocs: https://docs.tenyks.ai/reference/access-token.md\nsummary:\n  types: [http, apiKey-exchange]\n  api_key_in: [body]\n  http_schemes: [bearer]\n  model: >-\n    Two-step: exchange a long-lived API key + secret for a short-lived Bearer\n    access token, then send the Bearer token on every other endpoint.\nflow:\n  step_1_token_exchange:\n    endpoint: POST https://dashboard.tenyks.ai/api/auth/apikey\n    request:\n      api_key: Your Tenyks API key (from the dashboard).\n      api_secret: Your Tenyks API secret.\n    response:\n      access_token: Time-limited Bearer token.\n      id_token: JWT with user and authentication-event information.\n      expires_in: 3600\n      token_type: Bearer\n    docs: https://docs.tenyks.ai/reference/access-token.md\n\
  \  step_2_authenticated_calls:\n    header: \"Authorization: Bearer <access_token>\"\n    note: Token expires after 3600 seconds (60 minutes); refresh by repeating step 1.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Bearer access token obtained from POST /api/auth/apikey. Applied to every\n      dataset/model/prediction endpoint.\n    sources:\n      - openapi/tenyks-openapi.json\napi_keys:\n  retrieval: https://docs.tenyks.ai/reference/retrieving-api-keys.md\n  where: Tenyks dashboard (https://dashboard.tenyks.ai) — Premium; Sandbox key issuance coming for freemium.\nnotes:\n  - The API is currently in alpha and available to Premium (Dashboard) users.\n  - SDK equivalent: Tenyks.authenticate_with_api_key(api_base_url, api_key, api_secret, workspace_name).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenyks/refs/heads/main/authentication/tenyks-authentication.yml
summary_line: http/apiKey-exchange · 1 scheme
tags:
- Company
- Computer Vision
- Machine Learning
- MLOps
- Data Quality
- Model Validation
- Visual Intelligence
- Video Analytics
- Artificial Intelligence
- Developer Tools
---
