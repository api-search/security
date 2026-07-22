---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pave Bank Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pave Bank secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pave Bank
provider_slug: pave-bank
scheme_count: 1
schemes:
- client_auth: http_basic
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://docs.pavebank.com/docs/auth
  token_request: grant_type=client_credentials&audience=developer
  token_url: https://api.pavebank.com/oauth2/token
  token_use: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: pave-bank-authentication
source_filename: pave-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.pavebank.com/docs/auth\ndocs: https://docs.pavebank.com/docs/auth\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  access_model: role-based\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.pavebank.com/oauth2/token\n  token_request: grant_type=client_credentials&audience=developer\n  client_auth: http_basic\n  token_use: 'Authorization: Bearer <access_token>'\n  sources: [https://docs.pavebank.com/docs/auth]\nroles:\n- name: admin\n  description: Full read and write access. Can perform all API operations including transfers, account creation, and webhook configuration.\n- name: viewer\n  description: Read-only access. Can view accounts, balances, transactions, and other resources but cannot create or modify them. Unauthorized write attempts return PERMISSION_DENIED.\nrequest_signing:\n  supported: true\n  type: JWT\n  applies_to:\
  \ mutating operations\n  note: Optional JWT-based request payload signing for mutating operations, for compliance and request integrity verification.\nnotes:\n- Pave Bank uses OAuth 2.0 client credentials (server-to-server); no traditional OAuth scopes — access is governed by admin/viewer roles assigned when credentials are created.\n- Base API URL is https://api.pavebank.com/v1/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pave-bank/refs/heads/main/authentication/pave-bank-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Banking
- Payments
- Digital Assets
- Stablecoins
- Cross-Border Payments
- Programmable Money
- API
---
