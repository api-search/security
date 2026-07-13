---
api_key_in: []
api_specs:
- filename: flutterwave-payments-api-openapi.yml
  format: yaml
  label: Flutterwave Payments API
  slug: flutterwave-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-payments-api-openapi.yml
- filename: flutterwave-transfers-api-openapi.yml
  format: yaml
  label: Flutterwave Transfers API
  slug: flutterwave-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-transfers-api-openapi.yml
- filename: flutterwave-settlements-api-openapi.yml
  format: yaml
  label: Flutterwave Settlements API
  slug: flutterwave-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-settlements-api-openapi.yml
- filename: flutterwave-wallets-api-openapi.yml
  format: yaml
  label: Flutterwave Wallets API
  slug: flutterwave-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-wallets-api-openapi.yml
- filename: flutterwave-banks-api-openapi.yml
  format: yaml
  label: Flutterwave Banks API
  slug: flutterwave-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-banks-api-openapi.yml
- filename: flutterwave-webhooks-api-openapi.yml
  format: yaml
  label: Flutterwave Webhooks API
  slug: flutterwave-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Flutterwave Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Flutterwave secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Flutterwave
provider_slug: flutterwave
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/flutterwave-banks-api-openapi.yml
  - openapi/flutterwave-payments-api-openapi.yml
  - openapi/flutterwave-settlements-api-openapi.yml
  - openapi/flutterwave-transfers-api-openapi.yml
  - openapi/flutterwave-wallets-api-openapi.yml
  type: oauth2
slug: flutterwave-authentication
source_filename: flutterwave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flutterwave-banks-api-openapi.yml, openapi/flutterwave-payments-api-openapi.yml,\n  openapi/flutterwave-settlements-api-openapi.yml, openapi/flutterwave-transfers-api-openapi.yml,\n  openapi/flutterwave-wallets-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token\n    scopes: 0\n  sources:\n  - openapi/flutterwave-banks-api-openapi.yml\n  - openapi/flutterwave-payments-api-openapi.yml\n  - openapi/flutterwave-settlements-api-openapi.yml\n  - openapi/flutterwave-transfers-api-openapi.yml\n  - openapi/flutterwave-wallets-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/authentication/flutterwave-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Payments
- Payouts
- Mobile Money
- Cards
- Africa
- Fintech
- Remittance
- Virtual Accounts
- Chargebacks
- Multi-Currency
---
