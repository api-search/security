---
api_key_in: []
api_specs:
- filename: sommelier-api-openapi.yml
  format: yaml
  label: Sommelier Finance API
  slug: sommelier-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sommelier/refs/heads/main/openapi/sommelier-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: derived
name: Sommelier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sommelier secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sommelier
provider_slug: sommelier
scheme_count: 0
schemes: []
slug: sommelier-authentication
source_filename: sommelier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sommelier-api-openapi.yml + https://api.sommelier.finance/\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public: true\nnotes: >-\n  The Sommelier Finance API is a public, read-only HTTP API. No securitySchemes\n  are declared in the spec and the official API Information page documents no\n  API keys, tokens, or OAuth. All endpoints are open GET requests with\n  path-based parameters. Consumers should treat this as an unauthenticated,\n  best-effort public data API and apply their own rate-limit / retry handling.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sommelier/refs/heads/main/authentication/sommelier-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Crypto Web3
- DeFi
- Blockchain
- Ethereum
- Vaults
- Yield
- Analytics
---
