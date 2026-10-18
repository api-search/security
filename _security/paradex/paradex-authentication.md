---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: paradex-websocket-asyncapi.yml
  format: yaml
  label: Paradex WebSocket API
  slug: paradex-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/asyncapi/paradex-websocket-asyncapi.yml
- filename: paradex-account-api-openapi.yml
  format: yaml
  label: Paradex Account API
  slug: paradex-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-account-api-openapi.yml
- filename: paradex-algos-api-openapi.yml
  format: yaml
  label: Paradex Algos API
  slug: paradex-algos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-algos-api-openapi.yml
- filename: paradex-authentication-api-openapi.yml
  format: yaml
  label: Paradex Authentication API
  slug: paradex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-authentication-api-openapi.yml
- filename: paradex-blocktrades-api-openapi.yml
  format: yaml
  label: Paradex Block Trades API
  slug: paradex-blocktrades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-blocktrades-api-openapi.yml
- filename: paradex-insurance-api-openapi.yml
  format: yaml
  label: Paradex Insurance API
  slug: paradex-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-insurance-api-openapi.yml
- filename: paradex-liquidations-api-openapi.yml
  format: yaml
  label: Paradex Liquidations API
  slug: paradex-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-liquidations-api-openapi.yml
- filename: paradex-marketmakerprotection-api-openapi.yml
  format: yaml
  label: Paradex Market Maker Protection API
  slug: paradex-marketmakerprotection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-marketmakerprotection-api-openapi.yml
- filename: paradex-markets-api-openapi.yml
  format: yaml
  label: Paradex Markets API
  slug: paradex-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-markets-api-openapi.yml
- filename: paradex-orders-api-openapi.yml
  format: yaml
  label: Paradex Orders API
  slug: paradex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-orders-api-openapi.yml
- filename: paradex-referrals-api-openapi.yml
  format: yaml
  label: Paradex Referrals API
  slug: paradex-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-referrals-api-openapi.yml
- filename: paradex-rfqs-api-openapi.yml
  format: yaml
  label: Paradex Rfqs API
  slug: paradex-rfqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-rfqs-api-openapi.yml
- filename: paradex-staking-api-openapi.yml
  format: yaml
  label: Paradex Staking API
  slug: paradex-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-staking-api-openapi.yml
- filename: paradex-subkey-api-openapi.yml
  format: yaml
  label: Paradex Subkey API
  slug: paradex-subkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-subkey-api-openapi.yml
- filename: paradex-system-api-openapi.yml
  format: yaml
  label: Paradex System API
  slug: paradex-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-system-api-openapi.yml
- filename: paradex-token-api-openapi.yml
  format: yaml
  label: Paradex Token API
  slug: paradex-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-token-api-openapi.yml
- filename: paradex-trades-api-openapi.yml
  format: yaml
  label: Paradex Trades API
  slug: paradex-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-trades-api-openapi.yml
- filename: paradex-transfers-api-openapi.yml
  format: yaml
  label: Paradex Transfers API
  slug: paradex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-transfers-api-openapi.yml
- filename: paradex-vaults-api-openapi.yml
  format: yaml
  label: Paradex Vaults API
  slug: paradex-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-vaults-api-openapi.yml
- filename: paradex-xptransfersv2-api-openapi.yml
  format: yaml
  label: Paradex XP Transfers V2 API
  slug: paradex-xptransfersv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-xptransfersv2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Paradex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paradex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paradex
provider_slug: paradex
scheme_count: 1
schemes:
- in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/paradex-openapi.yml
  type: apiKey
slug: paradex-authentication
source_filename: paradex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/paradex-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/paradex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/authentication/paradex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cryptocurrency
- Exchange
- Derivatives
- Trading
- Perpetual Futures
- DeFi
- WebSocket
- MCP
---
