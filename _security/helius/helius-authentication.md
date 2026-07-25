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
- filename: helius-addresses-api-openapi.yml
  format: yaml
  label: Helius Addresses API
  slug: helius-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-addresses-api-openapi.yml
- filename: helius-admin-api-openapi.yml
  format: yaml
  label: Helius Admin API
  slug: helius-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-admin-api-openapi.yml
- filename: helius-balances-api-openapi.yml
  format: yaml
  label: Helius Balances API
  slug: helius-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-balances-api-openapi.yml
- filename: helius-funding-api-openapi.yml
  format: yaml
  label: Helius Funding API
  slug: helius-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-funding-api-openapi.yml
- filename: helius-helius-api-catalog-api-openapi.yml
  format: yaml
  label: Helius Helius API Catalog API
  slug: helius-helius-api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-helius-api-catalog-api-openapi.yml
- filename: helius-history-api-openapi.yml
  format: yaml
  label: Helius History API
  slug: helius-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-history-api-openapi.yml
- filename: helius-identity-api-openapi.yml
  format: yaml
  label: Helius Identity API
  slug: helius-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-identity-api-openapi.yml
- filename: helius-nfts-api-openapi.yml
  format: yaml
  label: Helius NFTs API
  slug: helius-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-nfts-api-openapi.yml
- filename: helius-sender-api-openapi.yml
  format: yaml
  label: Helius Sender API
  slug: helius-sender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-sender-api-openapi.yml
- filename: helius-tokens-api-openapi.yml
  format: yaml
  label: Helius Tokens API
  slug: helius-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-tokens-api-openapi.yml
- filename: helius-transactions-api-openapi.yml
  format: yaml
  label: Helius Transactions API
  slug: helius-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-transactions-api-openapi.yml
- filename: helius-transfers-api-openapi.yml
  format: yaml
  label: Helius Transfers API
  slug: helius-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-transfers-api-openapi.yml
- filename: helius-webhooks-api-openapi.yml
  format: yaml
  label: Helius Webhooks API
  slug: helius-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-webhooks-api-openapi.yml
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
