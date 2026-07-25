---
api_key_in:
- header
api_specs:
- filename: mobula-market-api-openapi.yml
  format: yaml
  label: Mobula Market API
  slug: mobula-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-market-api-openapi.yml
- filename: mobula-metadata-api-openapi.yml
  format: yaml
  label: Mobula Metadata API
  slug: mobula-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-metadata-api-openapi.yml
- filename: mobula-search-api-openapi.yml
  format: yaml
  label: Mobula Search API
  slug: mobula-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-search-api-openapi.yml
- filename: mobula-wallet-api-openapi.yml
  format: yaml
  label: Mobula Wallet API
  slug: mobula-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-wallet-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mobula Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mobula secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mobula
provider_slug: mobula
scheme_count: 1
schemes:
- description: 'Free Mobula API key sent in the `Authorization` header (e.g. `Authorization: <MOBULA_API_KEY>`).'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/mobula-openapi.yml
  type: apiKey
slug: mobula-authentication
source_filename: mobula-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mobula-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Free Mobula API key sent in the `Authorization` header (e.g. `Authorization:\n    <MOBULA_API_KEY>`).'\n  sources:\n  - openapi/mobula-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/authentication/mobula-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Crypto
- Web3
- Market Data
- Blockchain
- Wallet
- Real Time
---
