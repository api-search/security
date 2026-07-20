---
api_key_in:
- header
api_specs:
- filename: gallop-data-openapi.json
  format: json
  label: Gallop Data API
  slug: gallop-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-data-openapi.json
- filename: gallop-analytics-openapi.json
  format: json
  label: Gallop Analytics API
  slug: gallop-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-analytics-openapi.json
- filename: gallop-insights-openapi.json
  format: json
  label: Gallop Insights API
  slug: gallop-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-insights-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gallop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gallop secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gallop
provider_slug: gallop
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/gallop-analytics-openapi.json
  - openapi/gallop-data-openapi.json
  - openapi/gallop-insights-openapi.json
  type: apiKey
slug: gallop-authentication
source_filename: gallop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gallop-analytics-openapi.json, openapi/gallop-data-openapi.json, openapi/gallop-insights-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/gallop-analytics-openapi.json\n  - openapi/gallop-data-openapi.json\n  - openapi/gallop-insights-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/authentication/gallop-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Developer Tools
- NFT
- Blockchain
- Web3
- Data
- Analytics
- Crypto
- Ethereum
- Solana
---
