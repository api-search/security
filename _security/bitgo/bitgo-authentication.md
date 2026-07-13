---
api_key_in: []
api_specs:
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Wallets API
  slug: bitgo-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Addresses API
  slug: bitgo-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Transactions & Transfers API
  slug: bitgo-transactions-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Keychains & Keys API
  slug: bitgo-keychains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Webhooks API
  slug: bitgo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Wallet Policies API
  slug: bitgo-wallet-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Staking API
  slug: bitgo-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Trading & Settlement (Go Network) API
  slug: bitgo-trading-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Express API
  slug: bitgo-express-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Enterprise & Users API
  slug: bitgo-enterprise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bitgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: BitGo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BitGo
provider_slug: bitgo
scheme_count: 1
schemes:
- bearerFormat: accessToken
  description: 'BitGo access token passed as `Authorization: Bearer <token>`.'
  name: accessToken
  scheme: bearer
  sources:
  - openapi/bitgo-openapi.yml
  type: http
slug: bitgo-authentication
source_filename: bitgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitgo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessToken\n  type: http\n  scheme: bearer\n  bearerFormat: accessToken\n  description: 'BitGo access token passed as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/bitgo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/authentication/bitgo-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Assets
- Custody
- Wallets
- Blockchain
- Crypto
- Staking
- Settlement
---
