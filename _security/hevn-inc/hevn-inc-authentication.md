---
api_key_in:
- header
api_specs:
- filename: hevn-inc-openapi-original.json
  format: json
  label: HEVN API
  slug: hevn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevn-inc/refs/heads/main/openapi/hevn-inc-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hevn Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hevn Inc secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hevn Inc
provider_slug: hevn-inc
scheme_count: 2
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/hevn-inc-openapi-original.json
  type: http
- description: Alternative HEVN API key header. The CLI defaults to Authorization Bearer unless configured with HEVN_API_KEY_HEADER=X-Api-Key.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/hevn-inc-openapi-original.json
  type: apiKey
slug: hevn-inc-authentication
source_filename: hevn-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hevn-inc-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hevn-inc-openapi-original.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Alternative HEVN API key header. The CLI defaults to Authorization Bearer unless\n    configured with HEVN_API_KEY_HEADER=X-Api-Key.\n  sources:\n  - openapi/hevn-inc-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hevn-inc/refs/heads/main/authentication/hevn-inc-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Financial Services
- Fintech
- Banking
- Payments
- Stablecoin
- USDC
- Cross-Border Payments
- Business Accounts
- MCP
- Agents
- API
---
