---
api_key_in:
- header
api_specs:
- filename: amberdata-asyncapi.yml
  format: yaml
  label: Amberdata WebSocket Streaming API
  slug: websocket-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/asyncapi/amberdata-asyncapi.yml
- filename: amberdata-defi-openapi.yaml
  format: yaml
  label: Amberdata DeFi API
  slug: amberdata-defi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-defi-openapi.yaml
- filename: amberdata-derivatives-openapi.yaml
  format: yaml
  label: Amberdata Futures API
  slug: amberdata-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-derivatives-openapi.yaml
- filename: amberdata-blockchain-openapi.yaml
  format: yaml
  label: Amberdata On-Chain API
  slug: amberdata-on-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-blockchain-openapi.yaml
- filename: amberdata-derivatives-openapi.yaml
  format: yaml
  label: Amberdata Options API
  slug: amberdata-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-derivatives-openapi.yaml
- filename: amberdata-spot-openapi.yaml
  format: yaml
  label: Amberdata Spot API
  slug: amberdata-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-spot-openapi.yaml
- filename: amberdata-arc-openapi.yaml
  format: yaml
  label: Amberdata Asset Reference & Classification API
  slug: amberdata-arc-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-arc-openapi.yaml
- filename: amberdata-market-openapi.yaml
  format: yaml
  label: Amberdata Market-api
  slug: amberdata-market-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-market-openapi.yaml
- filename: amberdata-metrics-openapi.yaml
  format: yaml
  label: Amberdata Market Metrics
  slug: amberdata-metrics-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-metrics-openapi.yaml
- filename: amberdata-price-openapi.yaml
  format: yaml
  label: Amberdata Pricing
  slug: amberdata-price-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-price-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Amberdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amberdata secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amberdata
provider_slug: amberdata
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/amberdata-arc-openapi.yaml
  - openapi/amberdata-blockchain-openapi.yaml
  - openapi/amberdata-defi-api-openapi.yml
  - openapi/amberdata-defi-market-openapi.yaml
  - openapi/amberdata-defi-openapi.yaml
  - openapi/amberdata-derivatives-openapi.yaml
  - openapi/amberdata-futures-api-openapi.yml
  - openapi/amberdata-market-openapi.yaml
  - openapi/amberdata-metrics-openapi.yaml
  - openapi/amberdata-on-chain-api-openapi.yml
  - openapi/amberdata-options-api-openapi.yml
  - openapi/amberdata-price-openapi.yaml
  - openapi/amberdata-spot-api-openapi.yml
  - openapi/amberdata-spot-openapi.yaml
  type: apiKey
slug: amberdata-authentication
source_filename: amberdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\ndocs: https://docs.amberdata.io/http/http-api-fundamentals\nnotes: >-\n  Every REST request requires the user-specific x-api-key header (requests\n  without a valid key are refused); key types encode the subscription tier\n  (UAT trial, UAO on-demand, UAK enterprise). WebSocket connections to\n  wss://ws.web3api.io authenticate with the same x-api-key header on the\n  upgrade request. An optional dated api-version header selects the API\n  version. No OAuth surface is published.\nsource: openapi/amberdata-arc-openapi.yaml, openapi/amberdata-blockchain-openapi.yaml, openapi/amberdata-defi-api-openapi.yml,\n  openapi/amberdata-defi-market-openapi.yaml, openapi/amberdata-defi-openapi.yaml, openapi/amberdata-derivatives-openapi.yaml,\n  openapi/amberdata-futures-api-openapi.yml, openapi/amberdata-market-openapi.yaml, openapi/amberdata-metrics-openapi.yaml,\n  openapi/amberdata-on-chain-api-openapi.yml, openapi/amberdata-options-api-openapi.yml,\
  \ openapi/amberdata-price-openapi.yaml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/amberdata-arc-openapi.yaml\n  - openapi/amberdata-blockchain-openapi.yaml\n  - openapi/amberdata-defi-api-openapi.yml\n  - openapi/amberdata-defi-market-openapi.yaml\n  - openapi/amberdata-defi-openapi.yaml\n  - openapi/amberdata-derivatives-openapi.yaml\n  - openapi/amberdata-futures-api-openapi.yml\n  - openapi/amberdata-market-openapi.yaml\n  - openapi/amberdata-metrics-openapi.yaml\n  - openapi/amberdata-on-chain-api-openapi.yml\n  - openapi/amberdata-options-api-openapi.yml\n  - openapi/amberdata-price-openapi.yaml\n  - openapi/amberdata-spot-api-openapi.yml\n  - openapi/amberdata-spot-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/authentication/amberdata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Crypto
- Blockchain
- Market Data
- Digital Assets
- Derivatives
- DeFi
- Onchain
---
