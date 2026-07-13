---
api_key_in: []
api_specs:
- filename: nomba-authentication-openapi.yml
  format: yaml
  label: Nomba Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-authentication-openapi.yml
- filename: nomba-accounts-openapi.yml
  format: yaml
  label: Nomba Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-accounts-openapi.yml
- filename: nomba-virtual-accounts-openapi.yml
  format: yaml
  label: Nomba Virtual Accounts API
  slug: virtual-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-virtual-accounts-openapi.yml
- filename: nomba-transfers-openapi.yml
  format: yaml
  label: Nomba Transfers API
  slug: transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transfers-openapi.yml
- filename: nomba-online-checkout-openapi.yml
  format: yaml
  label: Nomba Online Checkout API
  slug: online-checkout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-online-checkout-openapi.yml
- filename: nomba-charge-openapi.yml
  format: yaml
  label: Nomba Charge API
  slug: charge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-charge-openapi.yml
- filename: nomba-transactions-openapi.yml
  format: yaml
  label: Nomba Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transactions-openapi.yml
- filename: nomba-global-payout-openapi.yml
  format: yaml
  label: Nomba Global Payout API
  slug: global-payout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-global-payout-openapi.yml
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
