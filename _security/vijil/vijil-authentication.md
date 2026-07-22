---
api_key_in: []
api_specs:
- filename: vijil-openapi-original.json
  format: json
  label: Vijil Console API
  slug: vijil-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/openapi/vijil-openapi-original.json
auth_types:
- http
- cookie
description: ''
kind: authentication
layout: security
method: searched
name: Vijil Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vijil secures its APIs with http and cookie across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vijil
provider_slug: vijil
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Primary authentication for the REST API. Exchange email + password at POST /v1/auth/jwt/login for a JWT access token, then send it as `Authorization: Bearer <token>` on every request. Tokens expire; a 401 means the token must be refreshed (POST /v1/auth/jwt/refresh) or re-issued. Team scope is derived from the token; most operations act on the active team.'
  login_operation: openapi/vijil-openapi-original.json#jwt_login_v1_auth_jwt_login_post
  name: bearerAuth
  refresh_operation: openapi/vijil-openapi-original.json#jwt_refresh_v1_auth_jwt_refresh_post
  scheme: bearer
  sources:
  - https://docs.vijil.ai/developer-guide/agentic/quickstart
  type: http
- cookie_auth: true
  description: Browser/console flow — POST /v1/auth/jwt/login can set the JWT in an httpOnly cookie; POST /v1/auth/jwt/logout clears it. Used by the Vijil Console web UI.
  name: jwtCookie
  sources:
  - https://docs.vijil.ai/api-reference/teams/jwt-login
  type: cookie
slug: vijil-authentication
source_filename: vijil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vijil.ai/developer-guide/agentic/quickstart\ndocs: https://docs.vijil.ai/developer-guide/cli/setup\nnote: >-\n  The published OpenAPI (openapi/vijil-openapi-original.json) declares no\n  components.securitySchemes, so this profile is captured from the Vijil docs\n  (Quickstart, CLI Setup, Manage API Keys) rather than derived from the spec.\nsummary:\n  types: [http, cookie]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Primary authentication for the REST API. Exchange email + password at\n      POST /v1/auth/jwt/login for a JWT access token, then send it as\n      `Authorization: Bearer <token>` on every request. Tokens expire; a 401\n      means the token must be refreshed (POST /v1/auth/jwt/refresh) or re-issued.\n      Team scope is derived from the token;\
  \ most operations act on the active team.\n    login_operation: openapi/vijil-openapi-original.json#jwt_login_v1_auth_jwt_login_post\n    refresh_operation: openapi/vijil-openapi-original.json#jwt_refresh_v1_auth_jwt_refresh_post\n    sources: [https://docs.vijil.ai/developer-guide/agentic/quickstart]\n  - name: jwtCookie\n    type: cookie\n    cookie_auth: true\n    description: >-\n      Browser/console flow — POST /v1/auth/jwt/login can set the JWT in an\n      httpOnly cookie; POST /v1/auth/jwt/logout clears it. Used by the Vijil\n      Console web UI.\n    sources: [https://docs.vijil.ai/api-reference/teams/jwt-login]\nmodel_hub_keys:\n  description: >-\n    Separate from platform auth: Vijil stores per-team \"model hub\" API keys\n    (OpenAI, Together, custom hubs, Vertex AI, DigitalOcean) used to query the\n    model under evaluation. Managed via the Console UI (Keys), the Python client\n    (client.api_keys.list/create/delete/modify/rename), and supplied inline when\n    registering\
  \ an Agent (agent_url + api_key).\n  docs: https://docs.vijil.ai/legacy/tutorials/manage-api-keys\ncli_auth:\n  init: vijil auth init --url https://<console-gateway>\n  login: vijil auth login\n  storage: ~/.vijil/config.yaml\n  docs: https://docs.vijil.ai/developer-guide/cli/setup\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/authentication/vijil-authentication.yml
summary_line: http/cookie · 2 schemes
tags:
- Company
- AI
- AI Agents
- Agent Security
- AI Safety
- Trust
- Red Teaming
- Guardrails
- LLM Security
- Evaluation
- Observability
- MCP
---
