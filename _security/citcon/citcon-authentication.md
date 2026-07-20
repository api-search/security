---
api_key_in: []
auth_types:
- http
description: The Citcon UPI API authenticates with a Bearer access token passed in the Authorization header. An access token is generated from your Citcon private key by POSTing to /v1/access-tokens and is then supplied on every subsequent request. Tokens carry a permissions array scoping which operations they may perform.
kind: authentication
layout: security
method: searched
name: Citcon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citcon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Citcon
provider_slug: citcon
scheme_count: 1
schemes:
- format: 'Authorization: Bearer {access-token}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  source: https://www.citcon.com/dev/universal-payment-interface-upi---api
  type: http
slug: citcon-authentication
source_filename: citcon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.citcon.com/dev/universal-payment-interface-upi---api\nsummary:\n  types: [http]\n  http_scheme: bearer\n  token_model: access-token\ndescription: >-\n  The Citcon UPI API authenticates with a Bearer access token passed in the\n  Authorization header. An access token is generated from your Citcon private\n  key by POSTing to /v1/access-tokens and is then supplied on every subsequent\n  request. Tokens carry a permissions array scoping which operations they may\n  perform.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer {access-token}'\n  source: https://www.citcon.com/dev/universal-payment-interface-upi---api\ntoken:\n  issue_endpoint: POST /v1/access-tokens\n  generated_from: private-key\n  default_expiry: 24h\n  expiry_signal: HTTP 401 Unauthorized\n  token_types: [client, server]\n  permissions:\n  - charge\n  - inquiry\n  -\
  \ capture\n  - vault\n  - consult\n  - encryption-config\n  - refund\nnotes: >-\n  Token permissions function as coarse operation scopes but are not OAuth 2.0\n  scopes; there is no OAuth authorization-code/client-credentials flow, so no\n  scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citcon/refs/heads/main/authentication/citcon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Cross-Border Payments
- Digital Wallets
- Payment Gateway
- BNPL
- Global Payouts
- Fintech
---
