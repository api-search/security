---
api_key_in:
- header
api_specs:
- filename: allium-openapi-original.json
  format: json
  label: Allium Realtime API
  slug: allium-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allium/refs/heads/main/openapi/allium-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Allium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Allium secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Allium
provider_slug: allium
scheme_count: 1
schemes:
- in: header
  name: APIKeyBearer
  parameter: X-API-KEY
  sources:
  - openapi/allium-openapi-original.json
  type: apiKey
slug: allium-authentication
source_filename: allium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/allium-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyBearer\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/allium-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allium/refs/heads/main/authentication/allium-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Analytics
- Blockchain
- Crypto
- Web3
- Data Infrastructure
- Real-Time Data
- Stablecoins
- DeFi
- Machine Payments
---
