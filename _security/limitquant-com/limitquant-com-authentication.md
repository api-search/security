---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: limitquant-com-quant-api-openapi.yml
  format: yaml
  label: LimitQuant Quant API
  slug: limitquant-com-quant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limitquant-com/openapi/limitquant-com-quant-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LimitQuant Authentication
name_suffix: Authentication
oauth_flows: []
overview: LimitQuant secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LimitQuant
provider_slug: limitquant-com
scheme_count: 1
schemes:
- description: LiMiT Quant API key
  in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/limitquant-com-openapi.json
  type: apiKey
slug: limitquant-com-authentication
source_filename: limitquant-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/limitquant-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: LiMiT Quant API key\n  sources:\n  - openapi/limitquant-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/limitquant-com/authentication/limitquant-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Signals
- Bitcoin
- Ethereum
- Solana
---
