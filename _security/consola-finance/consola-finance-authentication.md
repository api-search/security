---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Consola Finance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Consola Finance secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Consola Finance
provider_slug: consola-finance
scheme_count: 2
schemes:
- description: Bearer API key from the Developer tab in Settings (https://app.request.finance/account/api-keys). Separate Test and Live keys. Docs note API keys are being deprecated in favor of OAuth for live apps.
  in: header
  name: ApiKey
  parameter: Authorization
  type: apiKey
- access_token_ttl: 24h
  audience: accounts
  authorizationUrl: https://auth.request.finance/authorize
  default_scopes:
  - openid
  - profile
  - email
  - offline_access
  flows:
  - flow: authorizationCode
    use: act on a user's behalf (read their invoices); returns access + refresh tokens
  - flow: clientCredentials
    use: act on your own account (send invoices); access token only, activation required
  issuer: https://auth.request.finance/
  name: OAuth2
  tokenUrl: https://auth.request.finance/oauth/token
  type: oauth2
slug: consola-finance-authentication
source_filename: consola-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.request.finance/getting-started\ndocs: https://docs.request.finance/going-live\nnotes: >-\n  Request Finance API auth, captured from the docs (no OpenAPI is published).\n  Two modes: API key (Bearer-style Authorization header) for quick start, and\n  OAuth 2.0 (Auth0-backed at auth.request.finance) for production. Endpoints and\n  scopes cross-checked against the live OIDC discovery document saved under\n  well-known/.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_header: Authorization\n  oauth2_flows: [authorizationCode, clientCredentials]\n  extra_headers:\n  - name: X-Network\n    values: [test, live]\n    required: true\n    description: Selects the test (Sepolia testnet) or live environment.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Bearer API key from the Developer tab in Settings\n    (https://app.request.finance/account/api-keys).\
  \ Separate Test and Live keys.\n    Docs note API keys are being deprecated in favor of OAuth for live apps.\n- name: OAuth2\n  type: oauth2\n  issuer: https://auth.request.finance/\n  audience: accounts\n  authorizationUrl: https://auth.request.finance/authorize\n  tokenUrl: https://auth.request.finance/oauth/token\n  flows:\n  - flow: authorizationCode\n    use: act on a user's behalf (read their invoices); returns access + refresh tokens\n  - flow: clientCredentials\n    use: act on your own account (send invoices); access token only, activation required\n  access_token_ttl: 24h\n  default_scopes: [openid, profile, email, offline_access]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consola-finance/refs/heads/main/authentication/consola-finance-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Crypto Accounting
- Digital Assets
- Web3 Finance
- Accounts Payable
- Accounts Receivable
- Invoicing
- Payroll
- Bookkeeping
- Blockchain
---
