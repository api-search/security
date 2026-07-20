---
api_key_in: []
api_specs:
- filename: codag-openapi-original.json
  format: json
  label: Codag API
  slug: codag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codag/refs/heads/main/openapi/codag-openapi-original.json
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Codag Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Codag secures its APIs with http, oauth2, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Codag
provider_slug: codag
scheme_count: 4
schemes:
- docs: https://codag.ai/docs/rest-api.html
  format: 'Authorization: Bearer <api-token>'
  header: Authorization
  issued_via:
  - POST /api/orgs/{slug}/keys
  - POST /api/org/keys
  location: header
  name: BearerToken
  scheme: bearer
  type: http
  used_by:
  - POST /v1/compact
  - GET  /v1/whoami
- device_authorization_endpoint: https://api.codag.ai/oauth/device/code
  flow: deviceCode
  name: OAuthDeviceFlow
  notes: RFC 8628 device authorization grant used by the codag CLI to obtain tokens.
  token_endpoint: https://api.codag.ai/oauth/token
  type: oauth2
  used_by:
  - codag auth login (CLI)
- name: GoogleSignIn
  provider: google
  type: openIdConnect
  used_by:
  - POST /api/auth/google
  - POST /api/auth/console-session
- issued_via:
  - POST /v1/anonymous/token
  name: AnonymousToken
  notes: Short-lived anonymous token for trial / unauthenticated free usage.
  scheme: bearer
  type: http
slug: codag-authentication
source_filename: codag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://codag.ai/docs/rest-api.html\ndocs: https://codag.ai/docs\nnotes: >-\n  The published openapi.json declares no components.securitySchemes (FastAPI app\n  applies auth via dependencies), so this profile is reconstructed from the REST\n  API docs and the spec's OAuth/key operations. Two request-time credential\n  models: an org-scoped Bearer API token for the compaction API, and an OAuth 2.0\n  device-authorization flow used by the CLI. Console/web sessions use Google\n  sign-in. The free compaction path is unauthenticated.\nsummary:\n  types: [http, oauth2, apiKey]\n  http_schemes: [bearer]\n  oauth2_flows: [deviceCode]\nschemes:\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: \"Authorization: Bearer <api-token>\"\n    issued_via:\n      - POST /api/orgs/{slug}/keys       # create_key (org-scoped API key)\n      - POST /api/org/keys             \
  \  # create_current_org_key\n    used_by:\n      - POST /v1/compact                 # inference compaction (Pro) / drain (Free)\n      - GET  /v1/whoami\n    docs: https://codag.ai/docs/rest-api.html\n  - name: OAuthDeviceFlow\n    type: oauth2\n    flow: deviceCode\n    device_authorization_endpoint: https://api.codag.ai/oauth/device/code\n    token_endpoint: https://api.codag.ai/oauth/token\n    used_by:\n      - codag auth login (CLI)\n    notes: RFC 8628 device authorization grant used by the codag CLI to obtain tokens.\n  - name: GoogleSignIn\n    type: openIdConnect\n    provider: google\n    used_by:\n      - POST /api/auth/google            # google_login (console/web session)\n      - POST /api/auth/console-session   # mint_console_session\n  - name: AnonymousToken\n    type: http\n    scheme: bearer\n    issued_via:\n      - POST /v1/anonymous/token         # anonymous_token_endpoint\n    notes: Short-lived anonymous token for trial / unauthenticated free usage.\nunauthenticated:\n\
  \  - POST /v1/free/compact                # deterministic drain compaction, no auth\n  - GET  /health\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codag/refs/heads/main/authentication/codag-authentication.yml
summary_line: http/oauth2/apiKey · 4 schemes
tags:
- Company
- Developer Tools
- Logging
- Observability
- Log Compression
- AI Agents
- MCP
- LLM Tooling
- Debugging
- Y Combinator
---
