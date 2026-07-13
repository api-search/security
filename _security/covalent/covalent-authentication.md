---
api_key_in: []
api_specs:
- filename: covalent-foundational-api-openapi.yml
  format: yaml
  label: GoldRush Foundational API
  slug: goldrush-foundational-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-foundational-api-openapi.yml
- filename: covalent-streaming-api-openapi.yml
  format: yaml
  label: GoldRush Streaming API
  slug: goldrush-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-streaming-api-openapi.yml
- filename: covalent-pipeline-api-openapi.yml
  format: yaml
  label: GoldRush Pipeline API
  slug: goldrush-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-pipeline-api-openapi.yml
- filename: covalent-hyperliquid-info-api-openapi.yml
  format: yaml
  label: GoldRush Hyperliquid Info API
  slug: goldrush-hyperliquid-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-hyperliquid-info-api-openapi.yml
- filename: covalent-x402-api-openapi.yml
  format: yaml
  label: GoldRush x402 API
  slug: goldrush-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-x402-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Covalent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Covalent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Covalent
provider_slug: covalent
scheme_count: 1
schemes:
- description: 'GoldRush API key, sent as `Authorization: Bearer <key>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/covalent-foundational-api-openapi.yml
  - openapi/covalent-hyperliquid-info-api-openapi.yml
  - openapi/covalent-pipeline-api-openapi.yml
  - openapi/covalent-streaming-api-openapi.yml
  - openapi/covalent-x402-api-openapi.yml
  type: http
slug: covalent-authentication
source_filename: covalent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/covalent-foundational-api-openapi.yml, openapi/covalent-hyperliquid-info-api-openapi.yml,\n  openapi/covalent-pipeline-api-openapi.yml, openapi/covalent-streaming-api-openapi.yml, openapi/covalent-x402-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'GoldRush API key, sent as `Authorization: Bearer <key>`.'\n  sources:\n  - openapi/covalent-foundational-api-openapi.yml\n  - openapi/covalent-hyperliquid-info-api-openapi.yml\n  - openapi/covalent-pipeline-api-openapi.yml\n  - openapi/covalent-streaming-api-openapi.yml\n  - openapi/covalent-x402-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/authentication/covalent-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Web3
- Multi-Chain
- Data Infrastructure
- Crypto
- DeFi
- NFT
- Hyperliquid
- GoldRush
- AI Agents
---
