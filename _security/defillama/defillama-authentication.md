---
api_key_in:
- query
api_specs:
- filename: defillama-coins-api-openapi.yml
  format: yaml
  label: DefiLlama Coins API
  slug: defillama-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/openapi/defillama-coins-api-openapi.yml
- filename: defillama-fees-api-openapi.yml
  format: yaml
  label: DefiLlama Fees API
  slug: defillama-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/openapi/defillama-fees-api-openapi.yml
- filename: defillama-stablecoins-api-openapi.yml
  format: yaml
  label: DefiLlama Stablecoins API
  slug: defillama-stablecoins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/openapi/defillama-stablecoins-api-openapi.yml
- filename: defillama-tvl-api-openapi.yml
  format: yaml
  label: DefiLlama TVL API
  slug: defillama-tvl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/openapi/defillama-tvl-api-openapi.yml
- filename: defillama-volumes-api-openapi.yml
  format: yaml
  label: DefiLlama Volumes API
  slug: defillama-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/openapi/defillama-volumes-api-openapi.yml
- filename: defillama-yields-api-openapi.yml
  format: yaml
  label: DefiLlama Yields API
  slug: defillama-yields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/openapi/defillama-yields-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Defillama Authentication
name_suffix: Authentication
oauth_flows: []
overview: DefiLlama secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DefiLlama
provider_slug: defillama
scheme_count: 1
schemes:
- description: Pro API key is supplied as a path segment in the base URL (pro-api.llama.fi/{apiKey}); this scheme is a placeholder.
  in: query
  name: apiKeyPath
  parameter: apiKey
  sources:
  - openapi/defillama-openapi.yml
  type: apiKey
slug: defillama-authentication
source_filename: defillama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/defillama-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyPath\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Pro API key is supplied as a path segment in the base URL (pro-api.llama.fi/{apiKey});\n    this scheme is a placeholder.\n  sources:\n  - openapi/defillama-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defillama/refs/heads/main/authentication/defillama-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- DeFi
- TVL
- Crypto
- Stablecoins
- Yields
- Bridges
- Aggregator
- Open-Source
---
