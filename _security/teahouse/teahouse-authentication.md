---
api_key_in:
- header
api_specs:
- filename: teahouse-vault-openapi.yml
  format: yaml
  label: Teahouse Vault API
  slug: teahouse-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teahouse/refs/heads/main/openapi/teahouse-vault-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Teahouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teahouse Finance secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teahouse Finance
provider_slug: teahouse
scheme_count: 1
schemes:
- documented: partial
  in: header
  name: X-API-KEY
  note: header name inferred/placeholder; provider does not publish it
  sources:
  - openapi/teahouse-vault-openapi.yml
  type: apiKey
slug: teahouse-authentication
source_filename: teahouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.teahouse.finance/docs/vault-api\ndocs: https://docs.teahouse.finance/docs/for-developers/vault-api-introduction\nnote: >-\n  Teahouse documents a 401 \"API Key verification failed\" response for the Vault\n  API, indicating API-key authentication is required for authenticated calls.\n  The exact header/parameter name is NOT published in the docs and must be\n  confirmed with the provider. Several read endpoints (the /vaults catalog)\n  appear to be publicly readable and are also consumed by third parties such as\n  DeFiLlama.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    name: X-API-KEY\n    documented: partial\n    note: header name inferred/placeholder; provider does not publish it\n    sources: [openapi/teahouse-vault-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teahouse/refs/heads/main/authentication/teahouse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- DeFi
- Blockchain
- Vaults
- Liquidity Management
- Asset Management
- Uniswap
- Web3
---
