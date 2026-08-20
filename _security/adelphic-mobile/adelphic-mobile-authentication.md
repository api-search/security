---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Adelphic Mobile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adelphic Mobile * secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adelphic Mobile *
provider_slug: adelphic-mobile
scheme_count: 1
schemes:
- also_observed:
    fetched: '2026-08-12'
    host: https://api.viantinc.com
    status: 401
    www_authenticate: Basic realm="Adelphic"
  description: 'HTTP Basic authentication (RFC 7617). Probing https://api.adelphic.com/ returns 401 Unauthorized with header `WWW-Authenticate: Basic realm="Adelphic"`. Credentials are provisioned to enterprise Adelphic DSP accounts.'
  name: basicAuth
  observed:
    content_type: text/html;charset=utf-8
    fetched: '2026-08-12'
    host: https://api.adelphic.com
    set_cookie: JSESSIONID
    status: 401
    www_authenticate: Basic realm="Adelphic"
  scheme: basic
  sources:
  - live probe of https://api.adelphic.com/ on 2026-07-17
  - live probe of https://api.adelphic.com/ and https://api.viantinc.com/ on 2026-08-12
  type: http
slug: adelphic-mobile-authentication
source_filename: adelphic-mobile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live HTTP probe of https://api.adelphic.com/ and https://api.viantinc.com/\n  (WWW-Authenticate response header), re-verified 2026-08-12\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Adelphic publishes no public OpenAPI and no self-service developer auth\n    reference. This profile records what was directly observed by probing the\n    live API host api.adelphic.com — a gated enterprise endpoint (Java servlet\n    container; JSESSIONID cookie) protected by HTTP Basic authentication.\n    api.viantinc.com returns the byte-identical 401 with the same\n    `Basic realm=\"Adelphic\"` challenge, confirming the two names front the same\n    Adelphic API service. Access requires Viant/Adelphic account credentials;\n    there is no public key issuance and no OAuth or OIDC discovery document\n    (/.well-known/oauth-authorization-server and\n    /.well-known/openid-configuration return 401\
  \ on the API host and 404 on the\n    web hosts).\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication (RFC 7617). Probing https://api.adelphic.com/\n    returns 401 Unauthorized with header\n    `WWW-Authenticate: Basic realm=\"Adelphic\"`. Credentials are provisioned to\n    enterprise Adelphic DSP accounts.\n  observed:\n    host: https://api.adelphic.com\n    status: 401\n    www_authenticate: Basic realm=\"Adelphic\"\n    set_cookie: JSESSIONID\n    content_type: text/html;charset=utf-8\n    fetched: '2026-08-12'\n  also_observed:\n    host: https://api.viantinc.com\n    status: 401\n    www_authenticate: Basic realm=\"Adelphic\"\n    fetched: '2026-08-12'\n  sources:\n  - live probe of https://api.adelphic.com/ on 2026-07-17\n  - live probe of https://api.adelphic.com/ and https://api.viantinc.com/ on 2026-08-12\ncoverage:\n  gated: true\n  note: >-\n    Every path probed on api.adelphic.com — /, /openapi.json, /swagger.json,\n\
  \    /v1/openapi.json, /api-docs, /docs, /redoc and all /.well-known/* — returns\n    401. The contract is behind the credential wall, not absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adelphic-mobile/refs/heads/main/authentication/adelphic-mobile-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Advertising
- AdTech
- Programmatic Advertising
- Demand-Side Platform
- DSP
- Marketing
- Connected TV
---
