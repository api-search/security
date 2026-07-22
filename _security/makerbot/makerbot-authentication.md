---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Makerbot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Makerbot secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Makerbot
provider_slug: makerbot
scheme_count: 2
schemes:
- bearerFormat: opaque
  evidence: 'WWW-Authenticate: Bearer V1 header returned by api.thingiverse.com'
  header: Authorization
  location: header
  name: BearerToken
  scheme: bearer
  sources:
  - live probe https://api.thingiverse.com/things/1
  type: http
- evidence: OAuth authorize endpoint redirects to Thingiverse login
  flows:
  - authorizationUrl: https://www.thingiverse.com/login/oauth/authorize
    flow: authorizationCode
    note: authorizationUrl verified live (302 -> /login when unauthenticated); tokenUrl per Thingiverse developer docs.
    tokenUrl: https://www.thingiverse.com/login/oauth/token
  - authorizationUrl: https://www.thingiverse.com/login/oauth/authorize
    flow: implicit
  name: OAuth2
  sources:
  - live probe https://www.thingiverse.com/login/oauth/authorize
  type: oauth2
slug: makerbot-authentication
source_filename: makerbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: live probe of https://api.thingiverse.com + https://www.thingiverse.com/developers\ndocs: https://www.thingiverse.com/developers\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit]\n  notes: >-\n    The MakerBot Thingiverse REST API requires a Bearer access token on every\n    request. Unauthenticated requests return HTTP 401 with\n    {\"error\",\"code\":401,\"type\":\"NO_TOKEN_PROVIDED\"}. The WWW-Authenticate\n    response header is \"Bearer V1\". Tokens are obtained either as per-application\n    App Tokens issued when registering an app, or via the OAuth 2.0\n    authorization flow for acting on behalf of a Thingiverse user.\nschemes:\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: opaque\n    location: header\n    header: Authorization\n    evidence: 'WWW-Authenticate: Bearer V1 header returned by api.thingiverse.com'\n    sources: [live probe\
  \ https://api.thingiverse.com/things/1]\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.thingiverse.com/login/oauth/authorize\n        tokenUrl: https://www.thingiverse.com/login/oauth/token\n        note: >-\n          authorizationUrl verified live (302 -> /login when unauthenticated);\n          tokenUrl per Thingiverse developer docs.\n      - flow: implicit\n        authorizationUrl: https://www.thingiverse.com/login/oauth/authorize\n    evidence: 'OAuth authorize endpoint redirects to Thingiverse login'\n    sources: [live probe https://www.thingiverse.com/login/oauth/authorize]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makerbot/refs/heads/main/authentication/makerbot-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- 3D Printing
- Manufacturing
- Thingiverse
- Maker
- Hardware
- Designs
- Community
---
