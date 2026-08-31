---
api_key_in: []
api_specs:
- filename: rtcstats-rtcstats-api-api-openapi.yml
  format: yaml
  label: rtcStats rtcStats API API
  slug: rtcstats-rtcstats-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtcstats/refs/heads/main/openapi/rtcstats-rtcstats-api-api-openapi.yml
auth_types:
- http
description: 'One authentication mechanism across the whole surface: a static application JWT presented as an HTTP Bearer token. There is no OAuth 2.0 authorization server, no OIDC discovery, no API-key header variant and no mTLS — probes of /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and /.well-known/openid-configuration return 404 on both hosts. The same token authenticates the REST API and the MCP Streamable HTTP endpoint.'
kind: authentication
layout: security
method: searched
name: Rtcstats Authentication
name_suffix: Authentication
oauth_flows: []
overview: rtcStats secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: rtcStats
provider_slug: rtcstats
scheme_count: 1
schemes:
- applied_to: all 9 operations (declared per-operation in the OpenAPI security block)
  bearerFormat: JWT
  description: 'Use header: Authorization: Bearer <token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rtcstats-api-openapi.yml
  type: http
slug: rtcstats-authentication
source_filename: rtcstats-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/rtcstats-api-openapi.yml\ndocs:\n  - https://rtcstats.com/api-docs\n  - https://rtcstats.com/integrations/mcp\n  - https://rtcstats.com/llms.txt\ndescription: >-\n  One authentication mechanism across the whole surface: a static application\n  JWT presented as an HTTP Bearer token. There is no OAuth 2.0 authorization\n  server, no OIDC discovery, no API-key header variant and no mTLS — probes of\n  /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\n  and /.well-known/openid-configuration return 404 on both hosts. The same token\n  authenticates the REST API and the MCP Streamable HTTP endpoint.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  bearer_formats:\n    - JWT\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: 'Use header: Authorization: Bearer <token>'\n    applied_to:\
  \ all 9 operations (declared per-operation in the OpenAPI security block)\n    sources:\n      - openapi/rtcstats-api-openapi.yml\ntoken_lifecycle:\n  issuance: rtcStats dashboard, Settings > Applications — create an application to mint a token\n  visibility: Shown once at creation and cannot be read back; if lost, create a new application\n  rotation: Create a new application and retire the old one; no documented rotation endpoint or expiry policy\n  scopes: none — the token is account-wide with no scope or permission model\n  revocation: Delete the application in the dashboard\nplan_gating:\n  api_access: Developer plan or above; accounts without API access receive HTTP 403\n  mcp_access: Developer plan or above\n  free_plan: No API or MCP access\nmcp:\n  endpoint: https://api.rtcstats.com/v1.0/mcp\n  header: 'Authorization: Bearer <application JWT>'\n  anonymous_methods:\n    - initialize\n    - tools/list\n  authenticated_methods:\n    - tools/call\n  note: >-\n    Discovery is deliberately\
  \ open — the tool contract with real inputSchema is\n    readable without credentials; only tool invocation requires the token.\nfailure_modes:\n  - {status: 401, meaning: Missing or invalid token}\n  - {status: 403, meaning: API access is not included in the account plan}\ngaps:\n  - No OAuth 2.1 / dynamic client registration for the MCP server, which is where hosted MCP is converging.\n  - No scopes — a token that can read every session can also delete every session.\n  - No documented token expiry, so credential rotation is entirely manual.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtcstats/refs/heads/main/authentication/rtcstats-authentication.yml
summary_line: http · 1 scheme
tags:
- WebRTC
- observability
- Monitoring
- debugging
- real-time-communications
- Video
- Voice
- Artificial Intelligence
- MCP
- Developer Tools
---
