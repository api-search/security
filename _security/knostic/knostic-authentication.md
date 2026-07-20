---
api_key_in:
- header
api_specs:
- filename: knostic-agentmesh-openapi.yml
  format: yaml
  label: Knostic AgentMesh API
  slug: agentmesh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knostic/refs/heads/main/openapi/knostic-agentmesh-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Knostic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knostic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knostic
provider_slug: knostic
scheme_count: 1
schemes:
- description: AgentMesh API key. Created from the console via POST /api/console/keys and sent on every request as an Authorization bearer token.
  format: 'Authorization: Bearer <api_key>'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/knostic-agentmesh-openapi.yml
  type: http
slug: knostic-authentication
source_filename: knostic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://agentmesh.knostic.ai/api\ndocs: https://agentmesh.knostic.ai/api\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    AgentMesh authenticates API callers with a bearer API key minted from the AgentMesh\n    console. There is no OAuth 2.0 / OpenID Connect surface on the public API, so no\n    scopes artifact is emitted. Console (browser) sessions are brokered by Descope as\n    the identity provider, but that is the console's own login, not the API contract.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <api_key>'\n  description: >-\n    AgentMesh API key. Created from the console via POST /api/console/keys and sent on\n    every request as an Authorization bearer token.\n  sources:\n  - openapi/knostic-agentmesh-openapi.yml\ntiers:\n- tier: anonymous\n  description: >-\n    Read endpoints\
  \ (/skills, /mcp, /extensions) answer unauthenticated requests at a\n    reduced tier. Verified live 2026-07-19: responses carry the header `X-Tier: anonymous`.\n  requires_key: false\n  endpoints:\n  - GET /skills\n  - GET /mcp\n  - GET /extensions\n- tier: api-key\n  description: >-\n    Scan endpoints require a valid API key; each key carries its own daily scan quota and\n    can only read back the scans it created.\n  requires_key: true\n  endpoints:\n  - POST /scan/skill/{slug}\n  - POST /scan/extension/{slug}\n  - GET /scans\n  - GET /scans/{scan_id}\nkey_management:\n  console: https://agentmesh.knostic.ai/console\n  create_key_endpoint: POST /api/console/keys\n  identity_provider: Descope\n  notes: >-\n    Console endpoints (/api/console/me, /api/console/keys, /api/console/artefacts) are\n    session-scoped browser APIs behind the Descope login; they additionally send an\n    X-User-Email header. They are not part of the public API contract.\nfailure_modes:\n- status: 401\n  detail:\
  \ Missing or invalid API key\n- status: 403\n  detail: Scan belongs to a different API key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knostic/refs/heads/main/authentication/knostic-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Artificial Intelligence
- AI Agents
- Agent Security
- Supply Chain Security
- Model Context Protocol
- Threat Intelligence
- Developer Tools
- Shadow AI
---
