---
api_key_in: []
api_specs:
- filename: nomba-accounts-api-openapi.yml
  format: yaml
  label: Nomba Accounts API
  slug: nomba-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-accounts-api-openapi.yml
- filename: nomba-authentication-api-openapi.yml
  format: yaml
  label: Nomba Authentication API
  slug: nomba-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-authentication-api-openapi.yml
- filename: nomba-card-charge-api-openapi.yml
  format: yaml
  label: Nomba Card Charge API
  slug: nomba-card-charge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-card-charge-api-openapi.yml
- filename: nomba-checkout-orders-api-openapi.yml
  format: yaml
  label: Nomba Checkout Orders API
  slug: nomba-checkout-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-checkout-orders-api-openapi.yml
- filename: nomba-corridors-api-openapi.yml
  format: yaml
  label: Nomba Corridors API
  slug: nomba-corridors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-corridors-api-openapi.yml
- filename: nomba-exchange-rates-api-openapi.yml
  format: yaml
  label: Nomba Exchange Rates API
  slug: nomba-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-exchange-rates-api-openapi.yml
- filename: nomba-order-management-api-openapi.yml
  format: yaml
  label: Nomba Order Management API
  slug: nomba-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-order-management-api-openapi.yml
- filename: nomba-payouts-api-openapi.yml
  format: yaml
  label: Nomba Payouts API
  slug: nomba-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-payouts-api-openapi.yml
- filename: nomba-saved-cards-api-openapi.yml
  format: yaml
  label: Nomba Saved Cards API
  slug: nomba-saved-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-saved-cards-api-openapi.yml
- filename: nomba-tokenized-cards-api-openapi.yml
  format: yaml
  label: Nomba Tokenized Cards API
  slug: nomba-tokenized-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-tokenized-cards-api-openapi.yml
- filename: nomba-transactions-api-openapi.yml
  format: yaml
  label: Nomba Transactions API
  slug: nomba-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transactions-api-openapi.yml
- filename: nomba-transfers-api-openapi.yml
  format: yaml
  label: Nomba Transfers API
  slug: nomba-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transfers-api-openapi.yml
- filename: nomba-virtual-accounts-api-openapi.yml
  format: yaml
  label: Nomba Virtual Accounts API
  slug: nomba-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-virtual-accounts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nomba Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nomba secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nomba
provider_slug: nomba
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 bearer token obtained from the Nomba Authentication API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nomba-accounts-openapi.yml
  - openapi/nomba-authentication-openapi.yml
  - openapi/nomba-charge-openapi.yml
  - openapi/nomba-global-payout-openapi.yml
  - openapi/nomba-online-checkout-openapi.yml
  - openapi/nomba-transactions-openapi.yml
  - openapi/nomba-transfers-openapi.yml
  - openapi/nomba-virtual-accounts-openapi.yml
  type: http
slug: nomba-authentication
source_filename: nomba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nomba-accounts-openapi.yml, openapi/nomba-authentication-openapi.yml, openapi/nomba-charge-openapi.yml,\n  openapi/nomba-global-payout-openapi.yml, openapi/nomba-online-checkout-openapi.yml, openapi/nomba-transactions-openapi.yml,\n  openapi/nomba-transfers-openapi.yml, openapi/nomba-virtual-accounts-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 bearer token obtained from the Nomba Authentication API.\n  sources:\n  - openapi/nomba-accounts-openapi.yml\n  - openapi/nomba-authentication-openapi.yml\n  - openapi/nomba-charge-openapi.yml\n  - openapi/nomba-global-payout-openapi.yml\n  - openapi/nomba-online-checkout-openapi.yml\n  - openapi/nomba-transactions-openapi.yml\n  - openapi/nomba-transfers-openapi.yml\n  - openapi/nomba-virtual-accounts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/authentication/nomba-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Fintech
- Banking
- Transfers
- Virtual Accounts
- Checkout
- Cross-Border Payments
- Cards
---
