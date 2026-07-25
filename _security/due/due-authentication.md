---
api_key_in: []
api_specs:
- filename: due-account-api-openapi.yml
  format: yaml
  label: Due Account API
  slug: due-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-account-api-openapi.yml
- filename: due-account-wallets-api-openapi.yml
  format: yaml
  label: Due Account Wallets API
  slug: due-account-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-account-wallets-api-openapi.yml
- filename: due-blockchain-transfers-api-openapi.yml
  format: yaml
  label: Due Blockchain Transfers API
  slug: due-blockchain-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-blockchain-transfers-api-openapi.yml
- filename: due-channels-api-openapi.yml
  format: yaml
  label: Due Channels API
  slug: due-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-channels-api-openapi.yml
- filename: due-financial-institutions-api-openapi.yml
  format: yaml
  label: Due Financial Institutions API
  slug: due-financial-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-financial-institutions-api-openapi.yml
- filename: due-kyc-api-openapi.yml
  format: yaml
  label: Due KYC API
  slug: due-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-kyc-api-openapi.yml
- filename: due-markets-api-openapi.yml
  format: yaml
  label: Due Markets API
  slug: due-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-markets-api-openapi.yml
- filename: due-quote-api-openapi.yml
  format: yaml
  label: Due Quote API
  slug: due-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-quote-api-openapi.yml
- filename: due-recipients-api-openapi.yml
  format: yaml
  label: Due Recipients API
  slug: due-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-recipients-api-openapi.yml
- filename: due-simulate-pay-in-api-openapi.yml
  format: yaml
  label: Due Simulate pay-in API
  slug: due-simulate-pay-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-simulate-pay-in-api-openapi.yml
- filename: due-tos-api-openapi.yml
  format: yaml
  label: Due TOS API
  slug: due-tos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-tos-api-openapi.yml
- filename: due-transfers-api-openapi.yml
  format: yaml
  label: Due Transfers API
  slug: due-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-transfers-api-openapi.yml
- filename: due-usage-api-openapi.yml
  format: yaml
  label: Due Usage API
  slug: due-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-usage-api-openapi.yml
- filename: due-vaults-api-openapi.yml
  format: yaml
  label: Due Vaults API
  slug: due-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-vaults-api-openapi.yml
- filename: due-virtual-accounts-api-openapi.yml
  format: yaml
  label: Due Virtual Accounts API
  slug: due-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-virtual-accounts-api-openapi.yml
- filename: due-wallets-api-openapi.yml
  format: yaml
  label: Due Wallets API
  slug: due-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-wallets-api-openapi.yml
- filename: due-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Due Webhook Endpoints API
  slug: due-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-webhook-endpoints-api-openapi.yml
- filename: due-webhooks-api-openapi.yml
  format: yaml
  label: Due Webhooks API
  slug: due-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Due Authentication
name_suffix: Authentication
oauth_flows: []
overview: Due secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Due
provider_slug: due
scheme_count: 1
schemes:
- description: API key presented as a bearer token.
  header: Authorization
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/due-openapi-original.yml
  type: http
slug: due-authentication
source_filename: due-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/due-openapi-original.yml\ndocs: https://due.readme.io/docs/creating-customers\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  note: >-\n    Due authenticates with an API key presented as an HTTP bearer token (Authorization: Bearer <api_key>).\n    Per-account operations are additionally scoped by the Due-Account-Id header. Read-only FX/market\n    endpoints require no authentication. Sandbox and production use environment-specific keys/hosts.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key presented as a bearer token.\n  header: Authorization\n  sources:\n  - openapi/due-openapi-original.yml\naccount_scoping:\n  header: Due-Account-Id\n  note: Scopes per-account requests (see webhook fetch/retry examples).\npublic_endpoints:\n  note: FX markets (getmarkets, getmarket, getmarkethistory) are public and require no authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/authentication/due-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Cross-Border Payments
- Stablecoins
- Fintech
- Virtual Accounts
- Foreign Exchange
- KYC
- Wallets
- API
---
