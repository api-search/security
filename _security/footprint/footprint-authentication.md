---
api_key_in:
- header
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: Footprint Analytics Data API
  slug: footprint-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Footprint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Footprint Analytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Footprint Analytics
provider_slug: footprint
scheme_count: 2
schemes:
- description: Footprint Analytics API key passed as a request header
  in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: Footprint Analytics API key passed as a query parameter
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: footprint-authentication
source_filename: footprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Footprint Analytics API key passed as a request header\n  sources:\n  - openapi/openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Footprint Analytics API key passed as a query parameter\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/authentication/footprint-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Blockchain
- DeFi
- NFT
- GameFi
- Token Analytics
- On-Chain Data
- Web3
- Crypto
---
