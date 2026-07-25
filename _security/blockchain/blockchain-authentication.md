---
api_key_in:
- header
api_specs:
- filename: blockchain-com-asyncapi.yml
  format: yaml
  label: Blockchain.com WebSocket APIs
  slug: blockchaincom-websocket-apis
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/asyncapi/blockchain-com-asyncapi.yml
- filename: blockchain-addresses-api-openapi.yml
  format: yaml
  label: Blockchain.com Addresses API
  slug: blockchain-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-addresses-api-openapi.yml
- filename: blockchain-blocks-api-openapi.yml
  format: yaml
  label: Blockchain.com Blocks API
  slug: blockchain-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-blocks-api-openapi.yml
- filename: blockchain-charts-api-openapi.yml
  format: yaml
  label: Blockchain.com Charts API
  slug: blockchain-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-charts-api-openapi.yml
- filename: blockchain-market-data-api-openapi.yml
  format: yaml
  label: Blockchain.com Market Data API
  slug: blockchain-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-market-data-api-openapi.yml
- filename: blockchain-network-api-openapi.yml
  format: yaml
  label: Blockchain.com Network API
  slug: blockchain-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-network-api-openapi.yml
- filename: blockchain-payments-api-openapi.yml
  format: yaml
  label: Blockchain.com Payments API
  slug: blockchain-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-payments-api-openapi.yml
- filename: blockchain-pools-api-openapi.yml
  format: yaml
  label: Blockchain.com Pools API
  slug: blockchain-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-pools-api-openapi.yml
- filename: blockchain-stats-api-openapi.yml
  format: yaml
  label: Blockchain.com Stats API
  slug: blockchain-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-stats-api-openapi.yml
- filename: blockchain-trading-api-openapi.yml
  format: yaml
  label: Blockchain.com Trading API
  slug: blockchain-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-trading-api-openapi.yml
- filename: blockchain-transactions-api-openapi.yml
  format: yaml
  label: Blockchain.com Transactions API
  slug: blockchain-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-transactions-api-openapi.yml
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
