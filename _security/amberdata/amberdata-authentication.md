---
api_key_in:
- header
api_specs:
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata Spot Market Data API
  slug: spot-market-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata Derivatives API
  slug: derivatives
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata DeFi API
  slug: defi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata On-Chain API
  slug: on-chain
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-asyncapi.yml
  format: yaml
  label: Amberdata WebSocket Streaming API
  slug: websocket-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/asyncapi/amberdata-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amberdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amberdata secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amberdata
provider_slug: amberdata
scheme_count: 1
schemes:
- description: Unique, user-specific API key. Required on every REST request via the x-api-key header.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/amberdata-openapi.yml
  type: apiKey
slug: amberdata-authentication
source_filename: amberdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amberdata-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Unique, user-specific API key. Required on every REST request via the x-api-key\n    header.\n  sources:\n  - openapi/amberdata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/authentication/amberdata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Crypto
- Blockchain
- Market Data
- Digital Assets
- Derivatives
- DeFi
- On-Chain
---
