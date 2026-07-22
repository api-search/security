---
api_key_in:
- header
api_specs:
- filename: mine-openapi-original.json
  format: json
  label: MineOS API
  slug: mineos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-openapi-original.json
- filename: mine-partners-openapi-original.json
  format: json
  label: MineOS Partners API
  slug: mineos-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-partners-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mine Authentication
name_suffix: Authentication
oauth_flows: []
overview: MINE secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MINE
provider_slug: mine
scheme_count: 1
schemes:
- description: "Authorization header using the Bearer scheme. \r\n\r\nEnter 'Bearer' [space] and then your API Key in the text input below.\r\n\r\nExample: 'Bearer 12345abcdef'"
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/mine-openapi-original.json
  - openapi/mine-partners-openapi-original.json
  type: apiKey
slug: mine-authentication
source_filename: mine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mine-openapi-original.json, openapi/mine-partners-openapi-original.json\ndocs: https://developers.mineos.ai/docs/authentication\nnotes: >-\n  API-key Bearer token. Create keys in the workspace under For Developers > API Keys;\n  the key is shown once. Max 10 active keys per workspace. HTTPS is required.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"Authorization header using the Bearer scheme. \\r\\n\\r\\nEnter 'Bearer' [space]\\\n    \\ and then your API Key in the text input below.\\r\\n\\r\\nExample: 'Bearer 12345abcdef'\"\n  sources:\n  - openapi/mine-openapi-original.json\n  - openapi/mine-partners-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/authentication/mine-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Privacy
- Data Governance
- Privacy Operations
- Consent Management
- AI Governance
- Third-Party Risk
- Compliance
- Security
---
