---
api_key_in: []
api_specs:
- filename: timeular-activities-api-openapi.yml
  format: yaml
  label: Timeular Activities API
  slug: timeular-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-activities-api-openapi.yml
- filename: timeular-authentication-api-openapi.yml
  format: yaml
  label: Timeular Authentication API
  slug: timeular-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-authentication-api-openapi.yml
- filename: timeular-current-tracking-api-openapi.yml
  format: yaml
  label: Timeular Current Tracking API
  slug: timeular-current-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-current-tracking-api-openapi.yml
- filename: timeular-folders-api-openapi.yml
  format: yaml
  label: Timeular Folders API
  slug: timeular-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-folders-api-openapi.yml
- filename: timeular-leaves-api-openapi.yml
  format: yaml
  label: Timeular Leaves API
  slug: timeular-leaves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-leaves-api-openapi.yml
- filename: timeular-members-api-openapi.yml
  format: yaml
  label: Timeular Members API
  slug: timeular-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-members-api-openapi.yml
- filename: timeular-reports-api-openapi.yml
  format: yaml
  label: Timeular Reports API
  slug: timeular-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-reports-api-openapi.yml
- filename: timeular-tags-mentions-api-openapi.yml
  format: yaml
  label: Timeular Tags & Mentions API
  slug: timeular-tags-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-tags-mentions-api-openapi.yml
- filename: timeular-time-entries-api-openapi.yml
  format: yaml
  label: Timeular Time Entries API
  slug: timeular-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-time-entries-api-openapi.yml
- filename: timeular-users-api-openapi.yml
  format: yaml
  label: Timeular Users API
  slug: timeular-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-users-api-openapi.yml
- filename: timeular-webhooks-api-openapi.yml
  format: yaml
  label: Timeular Webhooks API
  slug: timeular-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeular/refs/heads/main/openapi/timeular-webhooks-api-openapi.yml
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
