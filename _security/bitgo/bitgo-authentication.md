---
api_key_in: []
api_specs:
- filename: bitgo-addresses-api-openapi.yml
  format: yaml
  label: BitGo Addresses API
  slug: bitgo-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-addresses-api-openapi.yml
- filename: bitgo-enterprise-api-openapi.yml
  format: yaml
  label: BitGo Enterprise API
  slug: bitgo-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-enterprise-api-openapi.yml
- filename: bitgo-keychains-api-openapi.yml
  format: yaml
  label: BitGo Keychains API
  slug: bitgo-keychains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-keychains-api-openapi.yml
- filename: bitgo-policies-api-openapi.yml
  format: yaml
  label: BitGo Policies API
  slug: bitgo-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-policies-api-openapi.yml
- filename: bitgo-staking-api-openapi.yml
  format: yaml
  label: BitGo Staking API
  slug: bitgo-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-staking-api-openapi.yml
- filename: bitgo-trading-api-openapi.yml
  format: yaml
  label: BitGo Trading API
  slug: bitgo-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-trading-api-openapi.yml
- filename: bitgo-transactions-api-openapi.yml
  format: yaml
  label: BitGo Transactions API
  slug: bitgo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-transactions-api-openapi.yml
- filename: bitgo-transfers-api-openapi.yml
  format: yaml
  label: BitGo Transfers API
  slug: bitgo-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-transfers-api-openapi.yml
- filename: bitgo-user-api-openapi.yml
  format: yaml
  label: BitGo User API
  slug: bitgo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-user-api-openapi.yml
- filename: bitgo-wallets-api-openapi.yml
  format: yaml
  label: BitGo Wallets API
  slug: bitgo-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-wallets-api-openapi.yml
- filename: bitgo-webhooks-api-openapi.yml
  format: yaml
  label: BitGo Webhooks API
  slug: bitgo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-webhooks-api-openapi.yml
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
