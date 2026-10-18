---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zebpay-futures-api-openapi.yml
  format: yaml
  label: ZebPay Futures API
  slug: zebpay-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-api-openapi.yml
- filename: zebpay-futures-exchange-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Exchange API
  slug: zebpay-futures-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-exchange-api-openapi.yml
- filename: zebpay-futures-market-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Market API
  slug: zebpay-futures-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-market-api-openapi.yml
- filename: zebpay-futures-trade-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Trade API
  slug: zebpay-futures-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-trade-api-openapi.yml
- filename: zebpay-futures-user-leverage-api-openapi.yml
  format: yaml
  label: ZebPay Futures > User Leverage API
  slug: zebpay-futures-user-leverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-user-leverage-api-openapi.yml
- filename: zebpay-futures-wallet-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Wallet API
  slug: zebpay-futures-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-wallet-api-openapi.yml
- filename: zebpay-market-api-openapi.yml
  format: yaml
  label: ZebPay Market API
  slug: zebpay-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-market-api-openapi.yml
- filename: zebpay-trade-api-api-openapi.yml
  format: yaml
  label: ZebPay Trade API
  slug: zebpay-trade-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-trade-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Zebpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZebPay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZebPay
provider_slug: zebpay
scheme_count: 1
schemes:
- name: noauthAuth
  scheme: noauth
  sources:
  - openapi/zebpay-openapi.yml
  type: http
slug: zebpay-authentication
source_filename: zebpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/zebpay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: noauthAuth\n  type: http\n  scheme: noauth\n  sources:\n  - openapi/zebpay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/authentication/zebpay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Futures
- India
- Market Data
- MCP
---
