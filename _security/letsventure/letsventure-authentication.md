---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Letsventure Authentication
name_suffix: Authentication
oauth_flows: []
overview: LVX (formerly LetsVenture) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LVX (formerly LetsVenture)
provider_slug: letsventure
scheme_count: 1
schemes:
- documented: false
  evidence: 'GET https://api.lvxventures.com/ -> 401 with response header `WWW-Authenticate: Token` and body {"detail":"Authorization header is missing"}'
  in: header
  name: Token
  parameter_name: Authorization
  scheme: token
  type: http
slug: letsventure-authentication
source_filename: letsventure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live HTTP probes of https://api.lvxventures.com\nstatus: private-undocumented\nnotes: >-\n  LVX publishes no public API program, no developer portal and no OpenAPI\n  definition, so no securityScheme could be derived. The host\n  api.lvxventures.com is nonetheless live and serves a token-authenticated\n  private API that backs the LVX platform. The scheme below is what the server\n  itself advertises in its 401 response; it is NOT provider-documented, so no\n  `Authentication` pointer is wired into apis.yml (the ergonomics check reads\n  documented authentication, which LVX does not publish).\nhost: https://api.lvxventures.com\nsummary:\n  types:\n  - http\n  documented: false\n  public_api_program: false\nschemes:\n- name: Token\n  type: http\n  scheme: token\n  in: header\n  parameter_name: Authorization\n  documented: false\n  evidence: >-\n    GET https://api.lvxventures.com/ -> 401 with response header\n    `WWW-Authenticate:\
  \ Token` and body {\"detail\":\"Authorization header is missing\"}\nevidence:\n- probe: GET https://api.lvxventures.com/\n  status: 401\n  www_authenticate: Token\n  content_type: application/json\n  allow: GET, HEAD, OPTIONS\n- probe: GET https://api.lvxventures.com/v1/\n  status: 401\n  note: versioned path exists behind auth\n- probe: GET https://api.lvxventures.com/health\n  status: 200\n  body: '{\"message\":true}'\n- probe: GET https://api.lvxventures.com/openapi.json\n  status: 404\n- probe: GET https://api.lvxventures.com/docs\n  status: 404\n- probe: GET https://api.lvxventures.com/redoc\n  status: 404\n- probe: GET https://api.lvxventures.com/api/schema/\n  status: 404\nserver_fingerprint:\n  server_header: uvicorn\n  note: >-\n    Python ASGI stack; the token-auth envelope and Allow header shape are\n    consistent with Django REST Framework style TokenAuthentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letsventure/refs/heads/main/authentication/letsventure-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Venture Capital
- Angel Investing
- Private Markets
- Investment Platform
- Startup Funding
- India
---
