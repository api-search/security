---
api_key_in: []
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: probed
name: Uplight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uplight secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uplight
provider_slug: uplight
scheme_count: 1
schemes:
- bearerFormat: unknown
  evidence: 'HTTP 401 with body {"errors":[{"message":"Invalid or no token provided"}]} and response header server: kong/3.10.0.6-enterprise-edition. Returned for /, /v1, /openapi.json, /swagger.json, /mcp, and every /.well-known/ path — the gateway rejects before routing, so the 401 describes the edge policy, not any one operation.'
  name: bearerToken
  scheme: bearer
  sources:
  - probe:https://api.uplight.com/
  type: http
slug: uplight-authentication
source_filename: uplight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://api.uplight.com (2026-07-27). Not derived from an\n  OpenAPI — this repo has none — and not searched from docs, because Uplight publishes no\n  public authentication page.\ndocumented_publicly: false\nsummary:\n  types:\n  - http-bearer\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The only observable fact is that the production gateway demands a bearer token. The\n    grant type (client credentials, authorization code, or an issued static token) could\n    not be determined anonymously.\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: unknown\n  sources:\n  - probe:https://api.uplight.com/\n  evidence: >-\n    HTTP 401 with body {\"errors\":[{\"message\":\"Invalid or no token provided\"}]} and\n    response header server: kong/3.10.0.6-enterprise-edition. Returned for /, /v1,\n    /openapi.json, /swagger.json, /mcp, and every /.well-known/ path —\
  \ the gateway\n    rejects before routing, so the 401 describes the edge policy, not any one operation.\ndiscovery:\n  openid_configuration: false\n  oauth_authorization_server: false\n  probes:\n  - url: https://api.uplight.com/.well-known/openid-configuration\n    status: 401\n  - url: https://api.uplight.com/.well-known/oauth-authorization-server\n    status: 401\n  - url: https://api.uplight.com/.well-known/oauth-protected-resource\n    status: 401\n  - url: https://uplight.com/.well-known/openid-configuration\n    status: 404\n  - url: https://docs.uplight.com/.well-known/openid-configuration\n    status: 404\n  - url: https://auth.uplight.com/.well-known/openid-configuration\n    status: '000'\n    note: DNS does not resolve.\n  - url: https://login.uplight.com/\n    status: '000'\n    note: DNS does not resolve.\ncredential_issuance:\n  self_serve: false\n  gate: partner-only\n  note: >-\n    Credentials are issued through a commercial relationship — a utility customer or\n    contracted\
  \ ecosystem partner is granted access to the ReadMe portal at\n    docs.uplight.com. No public sign-up, no key-issuance form, no sandbox, no trial.\npointer_note: >-\n  Deliberately NOT wired as type Authentication in apis.yml. That pointer feeds the\n  \"authentication documented\" check, and Uplight documents nothing publicly — this file\n  records what a probe could observe from outside, not a provider-published auth guide.\n  Wire the pointer only if Uplight opens an authentication page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplight/refs/heads/main/authentication/uplight-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Demand Response
- DER
- Grid
- Virtual Power Plant
- DERMS
- Energy Efficiency
- Customer Engagement
---
