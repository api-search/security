---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Across Authentication
name_suffix: Authentication
oauth_flows: []
overview: Across declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Across
provider_slug: across
scheme_count: 2
schemes:
- description: API key issued per integrator; sent on every API call.
  format: 'Authorization: Bearer [example key]'
  in: header
  name: Authorization
  required_for: production
  scheme: bearer
  type: http
- description: Unique integrator identifier. Passed as the integratorId query parameter on Swap API calls; for direct contract integration it is appended to calldata prefixed with the delimiter 1dc0de (without the 0x prefix).
  format: 2-byte hex identifier (e.g. 0xdead, 0x0001, 0xffff)
  in: query
  name: integratorId
  required_for: production
  type: apiKey
slug: across-authentication
source_filename: across-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.across.to/introduction/api-keys\nprovider: Across\napi: Across Swap API\ndocs: https://docs.across.to/introduction/api-keys\nsummary: >-\n  Production use of the Across Swap API requires two credentials: an API key\n  passed as a Bearer token in the Authorization header, and a 2-byte hex\n  integratorId. Testnet requires no credentials.\nschemes:\n- type: http\n  scheme: bearer\n  name: Authorization\n  in: header\n  required_for: production\n  format: 'Authorization: Bearer [example key]'\n  description: API key issued per integrator; sent on every API call.\n- type: apiKey\n  name: integratorId\n  in: query\n  required_for: production\n  format: 2-byte hex identifier (e.g. 0xdead, 0x0001, 0xffff)\n  description: >-\n    Unique integrator identifier. Passed as the integratorId query parameter on\n    Swap API calls; for direct contract integration it is appended to calldata\n    prefixed with the delimiter 1dc0de\
  \ (without the 0x prefix).\nnotes:\n- Testnet does not require an API key or integrator ID.\n- Requests without valid credentials are subject to strict rate limits; authenticated requests receive higher allowances.\n- Exceeding limits returns HTTP 429 Too Many Requests.\ncredentials_request: https://docs.across.to/introduction/api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/across/refs/heads/main/authentication/across-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Crypto Infrastructure
- Cross Chain
- Bridge
- Interoperability
- Blockchain
- DeFi
- Web3
- Swap
- Payments
---
