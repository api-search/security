---
api_key_in: []
api_specs:
- filename: blueocean-spark-platform-openapi.json
  format: json
  label: BlueOcean Spark Platform API
  slug: blueocean-spark-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueocean/refs/heads/main/openapi/blueocean-spark-platform-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Blueocean Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlueOcean declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: BlueOcean
provider_slug: blueocean
scheme_count: 0
schemes: []
slug: blueocean-authentication
source_filename: blueocean-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/blueocean-spark-platform-openapi.json (+ anonymous HTTP probes of https://poseidon.blueocean.ai/api)\ndocs: null\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  declared_scheme_count: 0\nschemes: []\nnotes: >-\n  BlueOcean publishes no developer authentication documentation and the one machine-readable\n  contract we could find — the FastAPI-generated OpenAPI 3.1.0 served at\n  https://poseidon.blueocean.ai/api/openapi.json, the API base hardcoded by the\n  app.blueocean.ai product login bundle — declares NO components.securitySchemes and NO\n  `security` requirement on any of its 72 operations.\n  Caller identity is instead carried as ordinary request parameters: `user_id` and\n  `account_id` appear as required query parameters or request-body fields on the prompts,\n  siren-schedule, session-document, memory and MCP-registration operations\n  (see AuthorizeRequest, Prompt, SirenScheduleCreate, RegisterMCPRequest,\
  \ ConnectRequest).\n  This is a derived reading of the published contract, not a security assessment.\n  The OAuth 2.0 flows the contract does describe (`/auth/providers/{provider}/authorize`,\n  `/mcp/oauth/google/start`) are OUTBOUND — BlueOcean acting as an OAuth client to connect a\n  user's Google, Microsoft, LinkedIn, Slack or GitHub account — not an authorization server\n  BlueOcean operates for third-party API consumers. No\n  /.well-known/oauth-authorization-server or /.well-known/openid-configuration is served on\n  any BlueOcean host (all 404; see well-known/blueocean-well-known.yml).\nx-evidence:\n  - url: https://poseidon.blueocean.ai/api/openapi.json\n    http_status: 200\n    content_type: application/json\n    finding: no components.securitySchemes; no operation-level security\n  - url: https://poseidon.blueocean.ai/api/mcp/health\n    http_status: 200\n    finding: answered anonymously with no credential\n  - url: https://poseidon.blueocean.ai/api/auth/providers\n    http_status:\
  \ 200\n    finding: answered anonymously with no credential\n  - url: https://poseidon.blueocean.ai/api/prompts\n    http_status: 422\n    finding: rejected for missing user_id/account_id query params, not for missing credential\n  - url: https://www.blueocean.ai/.well-known/openid-configuration\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueocean/refs/heads/main/authentication/blueocean-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Marketing
- Artificial Intelligence
- Agentic AI
- Brand Intelligence
- Marketing Automation
- Analytics
- Go-To-Market
- Model Context Protocol
- Undocumented API
---
