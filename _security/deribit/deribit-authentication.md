---
api_key_in: []
api_specs:
- filename: asyncapi.yaml
  format: yaml
  label: Deribit WebSocket API
  slug: deribit-websocket-api
  spec_type: AsyncAPI
  url: https://docs.deribit.com/
- filename: deribit-account-management-api-openapi.yml
  format: yaml
  label: Deribit Account Management API
  slug: deribit-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-account-management-api-openapi.yml
- filename: deribit-authentication-api-openapi.yml
  format: yaml
  label: Deribit Authentication API
  slug: deribit-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-authentication-api-openapi.yml
- filename: deribit-block-rfq-api-openapi.yml
  format: yaml
  label: Deribit Block RFQ API
  slug: deribit-block-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-block-rfq-api-openapi.yml
- filename: deribit-block-trade-api-openapi.yml
  format: yaml
  label: Deribit Block Trade API
  slug: deribit-block-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-block-trade-api-openapi.yml
- filename: deribit-combo-books-api-openapi.yml
  format: yaml
  label: Deribit Combo Books API
  slug: deribit-combo-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-combo-books-api-openapi.yml
- filename: deribit-mark-price-api-openapi.yml
  format: yaml
  label: Deribit Mark Price API
  slug: deribit-mark-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-mark-price-api-openapi.yml
- filename: deribit-market-data-api-openapi.yml
  format: yaml
  label: Deribit Market Data API
  slug: deribit-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-market-data-api-openapi.yml
- filename: deribit-matching-engine-api-openapi.yml
  format: yaml
  label: Deribit Matching Engine API
  slug: deribit-matching-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-matching-engine-api-openapi.yml
- filename: deribit-portfolio-management-api-openapi.yml
  format: yaml
  label: Deribit Portfolio Management API
  slug: deribit-portfolio-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-portfolio-management-api-openapi.yml
- filename: deribit-private-api-openapi.yml
  format: yaml
  label: Deribit Private API
  slug: deribit-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-private-api-openapi.yml
- filename: deribit-public-api-openapi.yml
  format: yaml
  label: Deribit Public API
  slug: deribit-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-public-api-openapi.yml
- filename: deribit-session-management-api-openapi.yml
  format: yaml
  label: Deribit Session Management API
  slug: deribit-session-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-session-management-api-openapi.yml
- filename: deribit-subscription-management-api-openapi.yml
  format: yaml
  label: Deribit Subscription Management API
  slug: deribit-subscription-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-subscription-management-api-openapi.yml
- filename: deribit-supporting-api-openapi.yml
  format: yaml
  label: Deribit Supporting API
  slug: deribit-supporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-supporting-api-openapi.yml
- filename: deribit-trading-api-openapi.yml
  format: yaml
  label: Deribit Trading API
  slug: deribit-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-trading-api-openapi.yml
- filename: deribit-wallet-api-openapi.yml
  format: yaml
  label: Deribit Wallet API
  slug: deribit-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-wallet-api-openapi.yml
- filename: deribit-websocket-only-api-openapi.yml
  format: yaml
  label: Deribit WebSocket Only API
  slug: deribit-websocket-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-websocket-only-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deribit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deribit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deribit
provider_slug: deribit
scheme_count: 1
schemes:
- description: API key passed as a Bearer token. The authenticated session determines the portfolio that operations are applied to.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/deribit-starbase-openapi.json
  type: http
slug: deribit-authentication
source_filename: deribit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deribit-starbase-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token. The authenticated session determines the portfolio\n    that operations are applied to.\n  sources:\n  - openapi/deribit-starbase-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/authentication/deribit-authentication.yml
summary_line: http · 1 scheme
tags:
- Derivatives
- Cryptocurrency
- Bitcoin
- Ethereum
- Options
- Futures
- Perpetuals
- Trading
- Market Data
- Block Trading
- WebSocket
- Financial
---
