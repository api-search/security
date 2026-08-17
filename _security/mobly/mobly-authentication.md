---
api_key_in:
- header
api_specs:
- filename: mobly-rest-api-v0-openapi.yml
  format: yaml
  label: Mobly REST API v0
  slug: mobly-rest-api-v0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobly/refs/heads/main/openapi/mobly-rest-api-v0-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mobly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mob.ly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mob.ly
provider_slug: mobly
scheme_count: 1
schemes:
- description: Every request must carry a valid organization API key in the `x-api-key` header. The key scopes the request to the authenticated organization — all list endpoints return only that organization's records.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  scope: organization
  sources:
  - openapi/mobly-rest-api-v0-openapi.yml
  - https://help.getmobly.com/documentation/rest-api/rest-api-v0
  type: apiKey
slug: mobly-authentication
source_filename: mobly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/mobly-rest-api-v0-openapi.yml\ndocs: https://help.getmobly.com/documentation/rest-api/rest-api-v0\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  self_serve_key: false\n  key_issuance: >-\n    API keys are not self-serve. The API reference states \"Getting an API key:\n    contact your Mobly CSM\"; the REST API v0 doc says \"You can request an API\n    key by contacting customer support.\"\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  scope: organization\n  description: >-\n    Every request must carry a valid organization API key in the `x-api-key`\n    header. The key scopes the request to the authenticated organization — all\n    list endpoints return only that organization's records.\n  sources:\n  - openapi/mobly-rest-api-v0-openapi.yml\n  - https://help.getmobly.com/documentation/rest-api/rest-api-v0\nerrors:\n- condition: Missing API key\n\
  \  status: 401\n  body: '{\"status\": 401, \"error\": \"Unauthorized\"}'\n  observed: true\n- condition: Invalid API key\n  status: 403\n  body: '{\"status\": 403, \"error\": \"Forbidden\"}'\n  observed: true\nx-evidence:\n- url: https://help.getmobly.com/documentation/rest-api/rest-api-v0\n  http_status: 200\n  note: documented authentication section, header name and error table\n- url: https://core-api.getmobly.com/api/v0/events\n  http_status: 401\n  note: anonymous GET returned {\"error\":\"Unauthorized\"} on 2026-08-13\n- url: https://core-api.getmobly.com/api/v0/events\n  http_status: 403\n  note: GET with an invalid x-api-key returned {\"error\":\"Forbidden\"} on 2026-08-13\nnotes:\n- No OAuth 2.0, OIDC, mTLS or JWT surface is published; the REST API v0 is API-key only.\n- No scope or permission model is documented, so no scopes/ artifact is emitted.\n- The customer web app (hub.getmobly.com) authenticates end users with Firebase Auth, which is\n  a separate, non-public surface\
  \ from the documented REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobly/refs/heads/main/authentication/mobly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Events
- Event Marketing
- Lead Capture
- Lead Enrichment
- B2B
- Marketing
- Go-To-Market
- Artificial Intelligence
- CRM
- Marketing Automation
- Trade Shows
---
