---
api_key_in: []
api_specs:
- filename: timeular-early-openapi.yml
  format: yaml
  label: EARLY (Timeular) Public API
  slug: early-timeular-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-early-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Timeular Authentication
name_suffix: Authentication
oauth_flows: []
overview: Timeular secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Timeular
provider_slug: timeular
scheme_count: 1
schemes:
- description: Access Token obtained from POST /developer/sign-in using your API Key and API Secret.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/timeular-early-openapi.yml
  type: http
slug: timeular-authentication
source_filename: timeular-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/timeular-early-openapi.yml + https://developers.early.app/ (Authentication folder)\nsummary:\n  types:\n  - http\n  model: api-key-and-secret-exchanged-for-bearer-token\n  detail: >-\n    EARLY (Timeular) authenticates in two steps. First POST your API Key and API\n    Secret to /api/v4/developer/sign-in to obtain a short-lived Access Token. Then\n    send that token as `Authorization: Bearer <token>` on all secured endpoints.\n    API Key & Secret are generated in the EARLY web app (product.early.app), or via\n    POST /api/v4/developer/api-access when you already hold a token.\nsign_in:\n  operationId: signInWithApiKeyApiSecret\n  method: POST\n  path: '/api/v4/developer/sign-in'\n  request:\n    apiKey: string\n    apiSecret: string\n  returns: Access Token (Bearer)\nkey_management:\n  fetch_api_key:\n    operationId: fetchApiKey\n    method: GET\n    path: '/api/v4/developer/api-access'\n  generate_api_key:\n  \
  \  operationId: generateNewApiKeyApiSecret\n    method: POST\n    path: '/api/v4/developer/api-access'\n  logout:\n    operationId: logout\n    method: POST\n    path: '/api/v4/developer/logout'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access Token obtained from POST /developer/sign-in using your API Key and API Secret.\n  sources:\n  - openapi/timeular-early-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/authentication/timeular-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Time Tracking
- Productivity
- Time Management
- Reporting
- Team Management
- Webhooks
- SaaS
---
