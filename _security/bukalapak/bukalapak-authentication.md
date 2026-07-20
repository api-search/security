---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bukalapak Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Bukalapak secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Bukalapak
provider_slug: bukalapak
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.bukalapak.com/token
    usage: Application credentials (clientId + clientSecret). Grants access to read-only / public endpoints without a user context.
  - flow: password
    tokenUrl: https://accounts.bukalapak.com/token
    usage: Resource-owner password grant (username/email + password). Grants access to authenticated, user-scoped endpoints; token auto-refreshes.
  name: oauth2
  sources:
  - https://github.com/bukalapak/bukalapak.js
  token_presentation: Authorization Bearer header
  type: oauth2
slug: bukalapak-authentication
source_filename: bukalapak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://github.com/bukalapak/bukalapak.js (official SDK README) +\n  https://github.com/bukalapak/omniauth-bukalapak +\n  https://github.com/bukalapak/doorkeeper (org OAuth2 provider fork)\ndocs: https://github.com/bukalapak/bukalapak.js\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, password]\n  authorization_server: https://accounts.bukalapak.com\n  api_host: https://api.bukalapak.com\nnotes: >-\n  Bukalapak's public REST API uses OAuth2. Tokens are issued by the dedicated\n  authorization server accounts.bukalapak.com and presented as a Bearer token in\n  the Authorization header against api.bukalapak.com. The official JavaScript SDK\n  exposes two grants: client_credentials (application-level, read-only public\n  resources such as GET /products) and resource_owner_password (email + password\n  login, granting access to authenticated resources such as GET /me). Expired\n  access\
  \ tokens are auto-refreshed. The org runs a Doorkeeper-based (Rails) OAuth2\n  provider and ships an OmniAuth strategy, confirming a standard OAuth2 posture.\n  No OpenAPI/Swagger spec is published, so scheme details are captured from\n  first-party SDK/provider source rather than derived from a spec.\nschemes:\n  - name: oauth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://accounts.bukalapak.com/token\n        usage: >-\n          Application credentials (clientId + clientSecret). Grants access to\n          read-only / public endpoints without a user context.\n      - flow: password\n        tokenUrl: https://accounts.bukalapak.com/token\n        usage: >-\n          Resource-owner password grant (username/email + password). Grants\n          access to authenticated, user-scoped endpoints; token auto-refreshes.\n    token_presentation: Authorization Bearer header\n    sources:\n      - https://github.com/bukalapak/bukalapak.js\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bukalapak/refs/heads/main/authentication/bukalapak-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Indonesia
- Southeast Asia
- Payments
- OAuth2
---
