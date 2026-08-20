---
api_key_in: []
api_specs:
- filename: beehero-audio-api-openapi.yml
  format: yaml
  label: BeeHero Audio API
  slug: beehero-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-audio-api-openapi.yml
- filename: beehero-auth-api-openapi.yml
  format: yaml
  label: BeeHero Auth API
  slug: beehero-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-auth-api-openapi.yml
- filename: beehero-gateways-api-openapi.yml
  format: yaml
  label: BeeHero Gateways API
  slug: beehero-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-gateways-api-openapi.yml
- filename: beehero-sensors-api-openapi.yml
  format: yaml
  label: BeeHero Sensors API
  slug: beehero-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-sensors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Beehero Authentication
name_suffix: Authentication
oauth_flows: []
overview: BeeHero secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BeeHero
provider_slug: beehero
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Please enter access_token (taken from login response body)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/beehero-openapi-original.yml
  type: http
slug: beehero-authentication
source_filename: beehero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/beehero-openapi-original.yml\ndocs: https://docs.beehero.io/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  style: password login exchanged for a bearer token\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Please enter access_token (taken from login response body)\n  sources:\n  - openapi/beehero-openapi-original.yml\nflow:\n  step_1:\n    operation: login\n    request: POST https://backend.beehero.io/external/login\n    body: '{\"email\": \"<account email>\", \"password\": \"<account password>\"}'\n    response: '200 with {\"access_token\": \"...\"} in the body and a Set-Cookie: access_token_cookie=<token> header'\n    failure: 404 \"Login credentials do not match\"\n  step_2:\n    header: 'Authorization: Bearer <access_token>'\n    applies_to: every operation other than login\n    failures:\n    - '401 Login required, user is not logged in\
  \ — no token presented'\n    - '403 Invalid Token — token expired, malformed, or not valid for the account'\n  docs_note: >-\n    The Swagger UI at docs.beehero.io instructs: \"To use BeeHero API, it is necessary to first log in\n    and then copy and enter the given access_token into Authorize button.\"\ntoken:\n  lifetime: undocumented\n  refresh: undocumented\n  revocation: undocumented\n  rotation: undocumented\nmcp_server:\n  package: https://www.npmjs.com/package/beehero-mcp\n  style: same password-login pattern, performed by the server on the operator's behalf\n  login_path: /admin/login\n  credentials: API_USER_EMAIL + API_PASSWORD environment variables (API_PASSWORD marked sensitive)\n  token_header: 'Authorization: Bearer <access_token>'\n  see_also: mcp/beehero-mcp.yml\nnot_supported:\n- oauth2 (no oauth2 securityScheme; /.well-known/oauth-authorization-server 404 on every host)\n- openIdConnect (no /.well-known/openid-configuration on any host)\n- apiKey\n- mutualTLS\n- scoped\
  \ authorization (no scopes are declared or documented — scopes/ is intentionally absent)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/authentication/beehero-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Agriculture
- AgTech
- Pollination
- beekeeping
- Precision Agriculture
- IoT
- Sensors
- Environmental Data
- MCP
- agent-native
---
