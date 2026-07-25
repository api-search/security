---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Big Xyt Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: big xyt secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: big xyt
provider_slug: big-xyt
scheme_count: 1
schemes:
- client_authentication: HTTP basic (client_id "xyt" + service secret)
  flow: password
  name: xytHubOAuth2
  sources:
  - https://github.com/vekonyz/xythub.github.io/blob/master/pages/xyt/api_overview.md
  status: legacy-2018-docs, unverified against current gated documentation
  token_url: '{AUTH_SERVICE_URL}/oauth/token'
  token_usage: 'Authorization: Bearer {access_token}'
  type: oauth2
slug: big-xyt-authentication
source_filename: big-xyt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://github.com/vekonyz/xythub.github.io/blob/master/pages/xyt/api_overview.md\ndocs: https://docs.big-xyt.com/en/api/api\nstatus: legacy-documented\nnote: |\n  The current API reference at docs.big-xyt.com is login-gated (HTTP 403\n  unauthenticated), so the live authentication model cannot be verified. This\n  profile is captured from the last PUBLIC documentation of the xyt hub API\n  (2018, preserved in the vekonyz fork of xythub.github.io after the official\n  repo's history was squashed in 2023). It documented OAuth 2.0 Resource Owner\n  Password Credentials grant issuing bearer tokens: POST to\n  AUTH_SERVICE_URL/oauth/token with HTTP basic client credentials\n  (client_id \"xyt\" + a service secret) and grant_type=password plus\n  username/password form fields; the JSON response returned access_token,\n  token_type bearer, expires_in ~43199 seconds (12h), scope \"read\". Every API\n  request then carries \"Authorization:\
  \ Bearer TOKEN\". Requests/responses used a\n  length-prefixed Protocol Buffers v3 binary wire format. Treat as legacy\n  provenance until the gated current docs can be verified.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [password]\n  token_type: bearer\n  token_lifetime_seconds: 43199\n  scopes_observed: [read]\nschemes:\n- name: xytHubOAuth2\n  type: oauth2\n  flow: password\n  token_url: '{AUTH_SERVICE_URL}/oauth/token'\n  client_authentication: HTTP basic (client_id \"xyt\" + service secret)\n  token_usage: 'Authorization: Bearer {access_token}'\n  status: legacy-2018-docs, unverified against current gated documentation\n  sources:\n  - https://github.com/vekonyz/xythub.github.io/blob/master/pages/xyt/api_overview.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-xyt/refs/heads/main/authentication/big-xyt-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Financial
- Market Data
- Tick Data
- Trading
- Analytics
- Equities
- ETFs
- Transaction Cost Analysis
- Liquidity
- Order Book
---
