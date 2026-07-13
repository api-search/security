---
api_key_in:
- header
api_specs:
- filename: blockchain-data-api-openapi.yml
  format: yaml
  label: Blockchain.com Blockchain Data API
  slug: blockchaincom-blockchain-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-data-api-openapi.yml
- filename: blockchain-charts-stats-openapi.yml
  format: yaml
  label: Blockchain.com Charts, Stats & Market Data API
  slug: blockchaincom-charts-stats-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-charts-stats-openapi.yml
- filename: blockchain-exchange-openapi.yml
  format: yaml
  label: Blockchain.com Exchange REST API
  slug: blockchaincom-exchange-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-exchange-openapi.yml
- filename: blockchain-com-asyncapi.yml
  format: yaml
  label: Blockchain.com WebSocket APIs
  slug: blockchaincom-websocket-apis
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/asyncapi/blockchain-com-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blockchain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockchain.com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blockchain.com
provider_slug: blockchain
scheme_count: 1
schemes:
- description: API key minted in the Exchange API settings panel; required on authenticated endpoints.
  in: header
  name: ApiToken
  parameter: X-API-Token
  sources:
  - openapi/blockchain-exchange-openapi.yml
  type: apiKey
slug: blockchain-authentication
source_filename: blockchain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blockchain-exchange-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-API-Token\n  description: API key minted in the Exchange API settings panel; required on authenticated\n    endpoints.\n  sources:\n  - openapi/blockchain-exchange-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/authentication/blockchain-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Bitcoin
- Blockchain Data
- Exchange
- Market Data
- Trading
- Payments
- Public APIs
---
