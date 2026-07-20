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
name: Erebor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Erebor secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Erebor
provider_slug: erebor
scheme_count: 2
schemes:
- confirmed: partial
  description: API key required on all api.erebor.bank requests. Confirmed by the gateway's 401 "Invalid or missing API key" response. Header name not published.
  in: header
  name: apiKey
  sources:
  - https://api.erebor.bank/
  type: apiKey
- confirmed: true
  description: Auth0-hosted OpenID Connect used to authenticate humans into the customer banking app and the developer dashboard. API keys are minted after login.
  flow: authorizationCode
  name: auth0
  provider: Auth0
  sources:
  - https://erebor.bank/assets/env-Dv_ZYF_D.js
  - https://developer.erebor.bank/assets/env-VmXpXH3m.js
  type: oauth2
slug: erebor-authentication
source_filename: erebor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  Live-observed 401 from https://api.erebor.bank/ and the Auth0 configuration in\n  the erebor.bank / developer.erebor.bank front-end bundles (env.js). Full auth\n  documentation lives at https://docs.erebor.bank but is login-gated.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Two distinct auth surfaces. (1) Programmatic API access to api.erebor.bank is\n    secured with an API key — an unauthenticated request returns HTTP 401\n    {\"error\":\"UNAUTHORIZED\",\"message\":\"Invalid or missing API key.\"}. The exact\n    header/parameter name is not documented publicly (docs are gated); header\n    placement is inferred from the \"API key\" wording and common practice and is\n    NOT confirmed. (2) Human access to the customer app (erebor.bank) and the\n    developer dashboard (developer.erebor.bank) is via Auth0 (OpenID Connect /\n    OAuth 2.0 Authorization\
  \ Code), configured with auth0Domain, auth0ClientId,\n    auth0Audience; the developer dashboard carries separate test and live Auth0\n    configurations (test/live mode).\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    API key required on all api.erebor.bank requests. Confirmed by the gateway's\n    401 \"Invalid or missing API key\" response. Header name not published.\n  confirmed: partial\n  sources: [https://api.erebor.bank/]\n- name: auth0\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Auth0-hosted OpenID Connect used to authenticate humans into the customer\n    banking app and the developer dashboard. API keys are minted after login.\n  provider: Auth0\n  confirmed: true\n  sources:\n  - https://erebor.bank/assets/env-Dv_ZYF_D.js\n  - https://developer.erebor.bank/assets/env-VmXpXH3m.js\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erebor/refs/heads/main/authentication/erebor-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Fintech
- Banking
- Digital Bank
- Stablecoin
- Cryptocurrency
- Payments
- Financial Services
- API
---
