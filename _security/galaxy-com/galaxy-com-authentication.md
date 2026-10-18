---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: galaxy-com-ethereum-api-openapi.yml
  format: yaml
  label: Galaxy Ethereum API
  slug: galaxy-com-ethereum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galaxy-com/refs/heads/main/openapi/galaxy-com-ethereum-api-openapi.yml
- filename: galaxy-com-solana-api-openapi.yml
  format: yaml
  label: Galaxy Solana API
  slug: galaxy-com-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galaxy-com/refs/heads/main/openapi/galaxy-com-solana-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Galaxy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Galaxy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Galaxy
provider_slug: galaxy-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: AuthorizationToken
  scheme: bearer
  sources:
  - openapi/galaxy-com-ethereum-staking-openapi.yml
  - openapi/galaxy-com-solana-staking-openapi.yml
  type: http
- in: header
  name: APIKey
  parameter: X-API-KEY
  sources:
  - openapi/galaxy-com-ethereum-staking-openapi.yml
  - openapi/galaxy-com-solana-staking-openapi.yml
  type: apiKey
slug: galaxy-com-authentication
source_filename: galaxy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/galaxy-com-ethereum-staking-openapi.yml, openapi/galaxy-com-solana-staking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AuthorizationToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/galaxy-com-ethereum-staking-openapi.yml\n  - openapi/galaxy-com-solana-staking-openapi.yml\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/galaxy-com-ethereum-staking-openapi.yml\n  - openapi/galaxy-com-solana-staking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galaxy-com/refs/heads/main/authentication/galaxy-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Cryptocurrency
- Digital Assets
- Staking
- Ethereum
- Solana
- Trading
- Custody
- Financial Services
---
