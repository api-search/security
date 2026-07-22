---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Monzo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Monzo secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Monzo
provider_slug: monzo
scheme_count: 2
schemes:
- authorizationUrl: https://auth.monzo.com/
  flow: authorizationCode
  logout: https://api.monzo.com/oauth2/logout
  name: OAuth2
  refresh: true
  refresh_note: Refresh tokens are only issued to confidential clients. Public (non-confidential) clients must re-authenticate when the access token expires.
  sources:
  - https://docs.monzo.com
  tokenUrl: https://api.monzo.com/oauth2/token
  type: oauth2
- in: header
  name: BearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.monzo.com
  type: http
slug: monzo-authentication
source_filename: monzo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.monzo.com\ndocs: https://docs.monzo.com\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - authorizationCode\n  http_schemes:\n  - bearer\n  notes: >-\n    Monzo uses OAuth 2.0 authorization code grant. Users authenticate and\n    authorise in the browser at auth.monzo.com; the resulting access token is\n    presented as an HTTP Bearer token on every API request. Strong Customer\n    Authentication (SCA) requires the user to approve access from a push\n    notification inside the Monzo mobile app. Access to transaction history\n    older than 90 days is revoked five minutes after authentication unless the\n    user approves ongoing access via SCA.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://auth.monzo.com/\n  tokenUrl: https://api.monzo.com/oauth2/token\n  refresh: true\n  refresh_note: >-\n    Refresh tokens are only issued to confidential clients.\
  \ Public\n    (non-confidential) clients must re-authenticate when the access token\n    expires.\n  logout: https://api.monzo.com/oauth2/logout\n  sources:\n  - https://docs.monzo.com\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  sources:\n  - https://docs.monzo.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monzo/refs/heads/main/authentication/monzo-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Banking
- Fintech
- Financial Services
- Payments
- Open Banking
- Accounts
- Transactions
- OAuth
---
