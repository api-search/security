---
api_key_in: []
auth_types:
- http
description: 'Authentication profile for the Qwil API. Derived from live probing rather than a published OpenAPI (Qwil publishes no public specification). The production API host at https://api.qwil.co is a Django REST Framework service that answers unauthenticated requests with HTTP 401 and `WWW-Authenticate: Bearer realm="api"`, indicating bearer-token authorization. The Qwil web application (app.qwil.com) authenticates end users through Firebase Authentication (Google Identity Platform) on the multi-tenant project `qwil-1149` / tenant `qwil-prod-*`; the resulting identity token is presented to the API as a bearer token. No public OAuth authorization-server or OpenID Connect discovery document is exposed (see well-known/qwil-well-known.yml). Access to the API is private/partner-gated.'
kind: authentication
layout: security
method: searched
name: Qwil Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qwil secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qwil
provider_slug: qwil
scheme_count: 1
schemes:
- description: 'Bearer token presented in the Authorization header. Observed live via the `WWW-Authenticate: Bearer realm="api"` challenge returned by https://api.qwil.co for unauthenticated requests.'
  name: bearerAuth
  scheme: bearer
  sources:
  - live-probe:https://api.qwil.co
  type: http
slug: qwil-authentication
source_filename: qwil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: live probe of https://api.qwil.co (WWW-Authenticate header) + app.qwil.com\n  client configuration\ndescription: >-\n  Authentication profile for the Qwil API. Derived from live probing rather than\n  a published OpenAPI (Qwil publishes no public specification). The production API\n  host at https://api.qwil.co is a Django REST Framework service that answers\n  unauthenticated requests with HTTP 401 and `WWW-Authenticate: Bearer realm=\"api\"`,\n  indicating bearer-token authorization. The Qwil web application (app.qwil.com)\n  authenticates end users through Firebase Authentication (Google Identity\n  Platform) on the multi-tenant project `qwil-1149` / tenant `qwil-prod-*`; the\n  resulting identity token is presented to the API as a bearer token. No public\n  OAuth authorization-server or OpenID Connect discovery document is exposed\n  (see well-known/qwil-well-known.yml). Access to the API is private/partner-gated.\nsummary:\n\
  \  types:\n  - http\n  http_schemes:\n  - bearer\n  identity_provider: Firebase Authentication (Google Identity Platform), multi-tenant\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token presented in the Authorization header. Observed live via the\n    `WWW-Authenticate: Bearer realm=\"api\"` challenge returned by\n    https://api.qwil.co for unauthenticated requests.\n  sources:\n  - live-probe:https://api.qwil.co\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwil/refs/heads/main/authentication/qwil-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Financial Services
- Payments
- Banking
- Plaid
---
