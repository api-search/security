---
api_key_in: []
api_specs:
- filename: sojo-industries-victoria-agent-openapi.json
  format: json
  label: SOJO Planning Assistant (Victoria) API
  slug: sojo-planning-assistant-victoria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sojo-industries/refs/heads/main/openapi/sojo-industries-victoria-agent-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Sojo Industries Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sojo Industries secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sojo Industries
provider_slug: sojo-industries
scheme_count: 1
schemes:
- applies_to:
  - POST /orchestrate
  - POST /api/chat
  - GET /api/chat/conversations
  - GET /api/chat/conversation/{session_id}
  - PATCH /api/chat/conversation/{session_id}
  - DELETE /api/chat/conversation/{session_id}
  - GET /api/chat/conversation/export/{session_id}
  bearerFormat: JWT
  description: 'Stytch session JWT. Pass as ''Authorization: Bearer <token>''.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sojo-industries-victoria-agent-openapi.json
  type: http
slug: sojo-industries-authentication
source_filename: sojo-industries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: >-\n  openapi/sojo-industries-victoria-agent-openapi.json (info.description + components.securitySchemes)\n  plus live unauthenticated probes of https://api.sojoshield.com and the public sojoshield.com JS bundle\nsummary:\n  types:\n  - http\n  model: >-\n    Bearer JWT throughout. Sojo Industries uses Stytch as its identity provider for the Sojo\n    Shield web app; the Stytch session JWT is the credential presented to both the Shield\n    platform API and the Victoria agent API. There is no API-key surface, no OAuth\n    authorization-server metadata document, and no published self-service key issuance —\n    credentials come from a Shield tenant account.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Stytch session JWT. Pass as ''Authorization: Bearer <token>''.'\n  applies_to:\n    - 'POST /orchestrate'\n    - 'POST /api/chat'\n    - 'GET /api/chat/conversations'\n    -\
  \ 'GET /api/chat/conversation/{session_id}'\n    - 'PATCH /api/chat/conversation/{session_id}'\n    - 'DELETE /api/chat/conversation/{session_id}'\n    - 'GET /api/chat/conversation/export/{session_id}'\n  sources:\n  - openapi/sojo-industries-victoria-agent-openapi.json\n\nidentity_provider:\n  name: Stytch\n  evidence: >-\n    The Sojo Shield SPA bundle at https://sojoshield.com/assets/index-C2RJOvGT.js embeds the\n    Stytch browser SDK (stytch.com/docs/sdks, telemetry.stytch.com, powered_by_stytch logo asset).\n    The Victoria OpenAPI info.description names the credential \"Stytch session JWT\".\n  token_resolution: >-\n    The Victoria OpenAPI states the bearer token is resolved to an identity via the Shield\n    internal endpoint /api/internal/v1/auth/resolve and cached in Redis. That endpoint is internal\n    and not part of any public contract.\n\nunauthenticated_surface:\n  note: 'These are the only routes reachable with no credential at all, verified 2026-08-28.'\n  routes:\n\
  \  - {url: 'https://victoria-agent.sojoshield.com/openapi.json', status: 200, note: 'The full public OpenAPI'}\n  - {url: 'https://victoria-agent.sojoshield.com/mcp', status: 200, note: 'MCP initialize + tools/list succeed anonymously'}\n  - {url: 'https://victoria-agent.sojoshield.com/health', status: 200, note: 'Detailed health, including auth_enabled=true and infrastructure internals'}\n  - {url: 'https://victoria-agent.sojoshield.com/ready', status: 200}\n  - {url: 'https://victoria-agent.sojoshield.com/upload-image', status: null, note: 'Declared in the OpenAPI with no security requirement — not exercised by this pass'}\n  - {url: 'https://api.sojoshield.com/docs', status: 200, note: 'Public Swagger UI shell'}\n\nauth_wall:\n  host: api.sojoshield.com\n  status: 401\n  envelope: '{\"data\":{\"message\":\"No bearer token provided.\"},\"error\":{\"code\":\"UNAUTHORIZED\",\"details\":{...}}}'\n  scope: >-\n    Host-wide. Every probed path on api.sojoshield.com returns this 401, including\
  \ /.well-known/*,\n    /graphql, /health and every spec path — the only exceptions are /docs (200, the Swagger UI HTML)\n    and /swagger.json (503, \"Swagger spec not initialised\").\n\ngaps:\n- 'No published authentication documentation page — the auth model is only discoverable from the OpenAPI info.description and the SPA bundle.'\n- 'No OAuth 2.0 authorization-server or protected-resource metadata at either host.'\n- 'No documented scopes or permissions model; the API entry point is tenant-scoped rather than scope-scoped.'\n- 'No self-service sign-up or key issuance — access requires a Sojo Shield customer account.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sojo-industries/refs/heads/main/authentication/sojo-industries-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Supply Chain
- Traceability
- Food and Beverage
- Manufacturing
- Logistics
- Packaging
- Industrial Automation
- Blockchain
- Artificial Intelligence
- Model Context Protocol
---
