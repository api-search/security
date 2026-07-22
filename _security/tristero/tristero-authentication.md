---
api_key_in:
- header
api_specs:
- filename: tristero-api-openapi.json
  format: json
  label: Tristero API
  slug: tristero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-api-openapi.json
- filename: tristero-feather-api-openapi.json
  format: json
  label: Feather API
  slug: feather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-feather-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tristero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tristero secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tristero
provider_slug: tristero
scheme_count: 1
schemes:
- description: API key for authentication (if required by deployment)
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/tristero-api-openapi.json
  type: apiKey
slug: tristero-authentication
source_filename: tristero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tristero-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication (if required by deployment)\n  sources:\n  - openapi/tristero-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/authentication/tristero-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cryptocurrency
- Trading
- DeFi
- Cross-Chain
- Web3
- Margin Trading
- Dark Pools
---
