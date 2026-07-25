---
api_key_in: []
api_specs:
- filename: moov-io-accounts-api-openapi.yml
  format: yaml
  label: Moov Accounts API
  slug: moov-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-accounts-api-openapi.yml
- filename: moov-io-bank-accounts-api-openapi.yml
  format: yaml
  label: Moov Bank Accounts API
  slug: moov-io-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-bank-accounts-api-openapi.yml
- filename: moov-io-capabilities-api-openapi.yml
  format: yaml
  label: Moov Capabilities API
  slug: moov-io-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-capabilities-api-openapi.yml
- filename: moov-io-card-issuing-api-openapi.yml
  format: yaml
  label: Moov Card Issuing API
  slug: moov-io-card-issuing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-card-issuing-api-openapi.yml
- filename: moov-io-cards-api-openapi.yml
  format: yaml
  label: Moov Cards API
  slug: moov-io-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-cards-api-openapi.yml
- filename: moov-io-disputes-api-openapi.yml
  format: yaml
  label: Moov Disputes API
  slug: moov-io-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-disputes-api-openapi.yml
- filename: moov-io-institutions-api-openapi.yml
  format: yaml
  label: Moov Institutions API
  slug: moov-io-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-institutions-api-openapi.yml
- filename: moov-io-payment-methods-api-openapi.yml
  format: yaml
  label: Moov Payment Methods API
  slug: moov-io-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-payment-methods-api-openapi.yml
- filename: moov-io-refunds-api-openapi.yml
  format: yaml
  label: Moov Refunds API
  slug: moov-io-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-refunds-api-openapi.yml
- filename: moov-io-representatives-api-openapi.yml
  format: yaml
  label: Moov Representatives API
  slug: moov-io-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-representatives-api-openapi.yml
- filename: moov-io-sweeps-api-openapi.yml
  format: yaml
  label: Moov Sweeps API
  slug: moov-io-sweeps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-sweeps-api-openapi.yml
- filename: moov-io-transfers-api-openapi.yml
  format: yaml
  label: Moov Transfers API
  slug: moov-io-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-transfers-api-openapi.yml
- filename: moov-io-underwriting-api-openapi.yml
  format: yaml
  label: Moov Underwriting API
  slug: moov-io-underwriting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-underwriting-api-openapi.yml
- filename: moov-io-wallets-api-openapi.yml
  format: yaml
  label: Moov Wallets API
  slug: moov-io-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-wallets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moov Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moov secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moov
provider_slug: moov-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moov-io-openapi.yml
  type: http
slug: moov-io-authentication
source_filename: moov-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moov-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token passed as a Bearer token.\n  sources:\n  - openapi/moov-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/authentication/moov-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Money Movement
- Fintech
- ACH
- RTP
- Cards
- Wallets
- Embedded Finance
---
