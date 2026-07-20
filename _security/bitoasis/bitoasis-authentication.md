---
api_key_in: []
api_specs:
- filename: bitoasis-exchange-openapi.yml
  format: yaml
  label: BitOasis Exchange API
  slug: bitoasis-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitoasis/refs/heads/main/openapi/bitoasis-exchange-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bitoasis Authentication
name_suffix: Authentication
oauth_flows: []
overview: BitOasis secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BitOasis
provider_slug: bitoasis
scheme_count: 1
schemes:
- description: 'A BitOasis API token (Key + Secret pair) generated from the account UI at Settings > Security > Token Management (https://bitoasis.net/en/settings/security/tokens). Sent as an Authorization: Bearer header. Public market-data endpoints require no token.'
  format: Bearer <api-token>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bitoasis-exchange-openapi.yml
  type: http
slug: bitoasis-authentication
source_filename: bitoasis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://api.bitoasis.net/doc/ ; https://raw.githubusercontent.com/bit-oasis/bitoasis-mcp/main/src/bitoasis_mcp/client.py ;\n  https://instructions.tryargus.com/bitoasis.html\ndocs: https://support.bitoasis.net/en/support/solutions/articles/29000035643-api-documentation\nsummary:\n  types: [http]\n  http_scheme: bearer\n  token_style: api-token\n  token_location: header\n  header: Authorization\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <api-token>'\n    sources: [openapi/bitoasis-exchange-openapi.yml]\n    description: >-\n      A BitOasis API token (Key + Secret pair) generated from the account UI at\n      Settings > Security > Token Management\n      (https://bitoasis.net/en/settings/security/tokens). Sent as an\n      Authorization: Bearer header. Public market-data endpoints require no token.\ntoken_management:\n\
  \  create_at: https://bitoasis.net/en/settings/security/tokens\n  ip_whitelisting: optional\n  permissions:\n    - id: account_balance\n      label: Account Balance\n      access: read\n    - id: coin_deposit_read\n      label: Digital Assets Deposit Read Access\n      access: read\n    - id: coin_withdrawal_read\n      label: Digital Asset Withdrawal Read Access\n      access: read\n    - id: fiat_deposit_read\n      label: Fiat Deposit Read Access\n      access: read\n    - id: fiat_withdrawal_read\n      label: Fiat Withdrawal Read Access\n      access: read\n    - id: pro_order_read\n      label: Pro Order Read Access\n      access: read\n  note: >-\n    Token permissions are granular read/write capability toggles, not OAuth\n    scopes (there is no OAuth authorization/token endpoint). The read\n    permissions above are documented; write-capable permissions exist to enable\n    place-order and withdrawal operations. Read-only tokens are recommended\n    unless trading/withdrawal automation\
  \ is required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitoasis/refs/heads/main/authentication/bitoasis-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Crypto
- Cryptocurrency
- Exchange
- Trading
- Digital Assets
- Bitcoin
- MENA
- Fintech
- MCP
---
