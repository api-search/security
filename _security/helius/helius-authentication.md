---
api_key_in:
- header
- query
api_specs:
- filename: helius-asyncapi.yml
  format: yaml
  label: Helius Solana RPC
  slug: rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/asyncapi/helius-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Helius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helius secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Helius
provider_slug: helius
scheme_count: 2
schemes:
- description: Your Helius API key. You can get one for free in the [dashboard](https://dashboard.helius.dev/api-keys).
  in: query
  name: ApiKeyQuery
  parameter: api-key
  sources:
  - openapi/helius-openapi.json
  type: apiKey
- description: API key passed in request header
  in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/helius-openapi.json
  type: apiKey
slug: helius-authentication
source_filename: helius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/helius-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api-key\n  description: Your Helius API key. You can get one for free in the [dashboard](https://dashboard.helius.dev/api-keys).\n  sources:\n  - openapi/helius-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key passed in request header\n  sources:\n  - openapi/helius-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/authentication/helius-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Web3
- Blockchain
- Solana
- RPC
- DAS
- Streams
---
