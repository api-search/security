---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Get Covered Authentication
name_suffix: Authentication
oauth_flows: []
overview: Get Covered declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Get Covered
provider_slug: get-covered
scheme_count: 0
schemes: []
slug: get-covered-authentication
source_filename: get-covered-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://api.getcoveredinsurance.com/api-docs\ndocumented: false\nsummary: >-\n  Get Covered publishes no public authentication documentation and no machine-readable\n  contract from which security schemes could be derived. The one observable auth signal\n  is the gate on the API reference itself: api.getcoveredinsurance.com/api-docs returns\n  HTTP 401 with `WWW-Authenticate: Basic realm=\"\"`, i.e. the API documentation is behind\n  HTTP Basic authentication and is available only to partners Get Covered provisions\n  directly. That is the gate on the DOCS, not a statement about how the API authenticates\n  callers — the API's own auth model is not public.\n  No `Authentication` pointer is wired into apis.yml, because the\n  `authentication_documented` check should not be credited to a provider whose auth\n  surface is entirely private.\nschemes: []\nobservations:\n- surface: API reference\n  url: https://api.getcoveredinsurance.com/api-docs\n\
  \  http_status: 401\n  www_authenticate: 'Basic realm=\"\"'\n  content_type: text/plain\n  content_length: 0\n  server_signature: 'Rails-style headers observed (x-request-id, x-runtime, vary: Origin)'\n- surface: OAuth / OIDC discovery\n  probed:\n  - {url: 'https://api.getcoveredinsurance.com/.well-known/openid-configuration', http_status: 404}\n  - {url: 'https://api.getcoveredinsurance.com/.well-known/oauth-authorization-server', http_status: 404}\n  - {url: 'https://www.getcovered.io/.well-known/openid-configuration', http_status: 404}\n  result: no OAuth 2.0 or OpenID Connect discovery metadata published\n- surface: resident portal\n  url: https://renters.getcoveredinsurance.com/auth/login\n  http_status: 200\n  note: End-user (resident) login for the renters-insurance portal; email/password sign-in, not a developer auth surface.\ngaps:\n- No public authentication guide, key-issuance flow, or token model.\n- No OAuth 2.0 / OIDC metadata; scopes/ artifact is not applicable.\n- API\
  \ reference is Basic-auth gated, so security schemes cannot be harvested anonymously.\nx-evidence:\n  fetched: '2026-08-04'\n  tool: curl -D (header inspection)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/get-covered/refs/heads/main/authentication/get-covered-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Insurance
- Insurtech
- Renters Insurance
- Property Management
- Real-Estate
- Compliance
- Risk Management
- Embedded Insurance
- Artificial Intelligence
---
