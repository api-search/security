---
api_key_in: []
api_specs:
- filename: gameye-session-openapi.yml
  format: yaml
  label: Gameye Session API
  slug: gameye-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameye/refs/heads/main/openapi/gameye-session-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gameye Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gameye secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gameye
provider_slug: gameye
scheme_count: 1
schemes:
- bearerFormat: token
  name: api-token
  scheme: bearer
  sources:
  - openapi/gameye-session-openapi.yml
  type: http
slug: gameye-authentication
source_filename: gameye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gameye-session-openapi.yml\ndocs: https://gameye.com/docs/api-v2/authentication/\nsummary:\n  types:\n  - http\n  scheme: bearer\n  token_delivery: Authorization header\n  token_format: 'Authorization: Bearer <token>'\n  token_management: >-\n    API tokens are created per-user in the Gameye Admin Panel (Users > Edit >\n    API Tokens > Add Token). The full token value is shown only once at creation\n    time. All Session API endpoints require a bearer token.\nschemes:\n- name: api-token\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  sources:\n  - openapi/gameye-session-openapi.yml\n# Token permission scopes attached to operation security[] requirements in the\n# OpenAPI. Gameye uses bearer tokens (not OAuth2), so these are token-level\n# permissions rather than OAuth scopes.\ntoken_scopes:\n- scope: session:start\n  description: Allocate a new game session (POST /session).\n- scope: session:read\n  description:\
  \ List and describe sessions (GET /session, GET /session/{id}).\n- scope: session:stop\n  description: Terminate a running session (DELETE /session/{id}).\n- scope: artifact:read\n  description: Download artifacts from a terminated session's container (GET /artifacts).\n- scope: regions:read\n  description: List available locations and check image tags (GET /available-location/{image}, GET /tag/...).\n- scope: logs:read\n  description: Stream a session's stdout/stderr logs (GET /logs).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameye/refs/heads/main/authentication/gameye-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Game Server Hosting
- Game Server Orchestration
- Multiplayer
- Containers
- Infrastructure
- Gaming
- Edge Computing
- DevOps
---
