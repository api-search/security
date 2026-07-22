---
api_key_in:
- header
api_specs:
- filename: ripple-labs-rlusd-openapi-original.yml
  format: yaml
  label: Ripple Mint API (RLUSD Stablecoin)
  slug: ripple-mint-api-rlusd-stablecoin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-rlusd-openapi-original.yml
- filename: ripple-labs-ripplenet-openapi-original.yml
  format: yaml
  label: RippleNet Server API
  slug: ripplenet-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-ripplenet-openapi-original.yml
- filename: ripple-labs-report-service-openapi-original.yml
  format: yaml
  label: Report Service API
  slug: report-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-report-service-openapi-original.yml
- filename: ripple-labs-smart-liquidation-openapi-original.yml
  format: yaml
  label: Smart Liquidation API
  slug: smart-liquidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-smart-liquidation-openapi-original.yml
- filename: ripple-labs-palisade-wallet-openapi-original.yml
  format: yaml
  label: Palisade Wallet-as-a-Service API
  slug: palisade-wallet-as-a-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-palisade-wallet-openapi-original.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ripple Labs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ripple Labs secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ripple Labs
provider_slug: ripple-labs
scheme_count: 3
schemes:
- in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/ripple-labs-palisade-wallet-openapi-original.yml
  - openapi/ripple-labs-ripplenet-openapi-original.yml
  - openapi/ripple-labs-smart-liquidation-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  name: Bearer
  scheme: bearer
  sources:
  - openapi/ripple-labs-report-service-openapi-original.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.ripple.com/v2/oauth/token
  name: oauth2
  sources:
  - openapi/ripple-labs-rlusd-openapi-original.yml
  type: oauth2
slug: ripple-labs-authentication
source_filename: ripple-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/ripple-labs-palisade-wallet-openapi-original.yml, openapi/ripple-labs-report-service-openapi-original.yml,\n  openapi/ripple-labs-ripplenet-openapi-original.yml, openapi/ripple-labs-rlusd-openapi-original.yml,\n  openapi/ripple-labs-smart-liquidation-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/ripple-labs-palisade-wallet-openapi-original.yml\n  - openapi/ripple-labs-ripplenet-openapi-original.yml\n  - openapi/ripple-labs-smart-liquidation-openapi-original.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ripple-labs-report-service-openapi-original.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ripple.com/v2/oauth/token\n\
  \    scopes: 2\n  sources:\n  - openapi/ripple-labs-rlusd-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/authentication/ripple-labs-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Financial Services
- Payments
- Cross-Border Payments
- Blockchain
- Cryptocurrency
- Stablecoin
- Digital Assets
- Custody
- Wallet
- Fintech
---
