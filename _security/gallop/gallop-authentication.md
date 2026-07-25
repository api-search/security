---
api_key_in:
- header
api_specs:
- filename: gallop-ethereum-api-openapi.yml
  format: yaml
  label: Gallop Ethereum API
  slug: gallop-ethereum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-ethereum-api-openapi.yml
- filename: gallop-polygon-api-openapi.yml
  format: yaml
  label: Gallop Polygon API
  slug: gallop-polygon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-polygon-api-openapi.yml
- filename: gallop-solana-api-openapi.yml
  format: yaml
  label: Gallop Solana API
  slug: gallop-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-solana-api-openapi.yml
- filename: gallop-starknet-api-openapi.yml
  format: yaml
  label: Gallop Starknet API
  slug: gallop-starknet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-starknet-api-openapi.yml
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
