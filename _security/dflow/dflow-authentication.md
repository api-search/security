---
api_key_in:
- header
api_specs:
- filename: dflow-admin-api-openapi.yml
  format: yaml
  label: DFlow admin API
  slug: dflow-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-admin-api-openapi.yml
- filename: dflow-intent-api-openapi.yml
  format: yaml
  label: DFlow intent API
  slug: dflow-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-intent-api-openapi.yml
- filename: dflow-order-api-openapi.yml
  format: yaml
  label: DFlow order API
  slug: dflow-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-order-api-openapi.yml
- filename: dflow-prediction-market-api-openapi.yml
  format: yaml
  label: DFlow prediction_market API
  slug: dflow-prediction-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-prediction-market-api-openapi.yml
- filename: dflow-swap-api-openapi.yml
  format: yaml
  label: DFlow swap API
  slug: dflow-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-swap-api-openapi.yml
- filename: dflow-tokens-api-openapi.yml
  format: yaml
  label: DFlow tokens API
  slug: dflow-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-tokens-api-openapi.yml
- filename: dflow-venues-api-openapi.yml
  format: yaml
  label: DFlow venues API
  slug: dflow-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-venues-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: DFlow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DFlow
provider_slug: dflow
scheme_count: 1
schemes:
- description: API key for authentication. Contact hello@dflow.net to obtain an API key.
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/dflow-openapi-original.json
  type: apiKey
slug: dflow-authentication
source_filename: dflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dflow-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication. Contact hello@dflow.net to obtain an API key.\n  sources:\n  - openapi/dflow-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/authentication/dflow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto Web3
- Solana
- Trading API
- DeFi
- DEX Aggregator
- Token Swap
- Blockchain
- MEV Protection
- Prediction Markets
- Agent Ready
---
