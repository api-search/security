---
api_key_in: []
api_specs:
- filename: spaitial-ai-developer-api-openapi.json
  format: json
  label: SpAItial Developer API
  slug: spaitial-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaitial-ai/refs/heads/main/openapi/spaitial-ai-developer-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Spaitial Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpAItial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpAItial
provider_slug: spaitial-ai
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'API key issued from the developer portal (developers.spaitial.ai), sent as Authorization: Bearer spt_live_<key>. Test keys use the spt_test_ prefix with the same scopes and lower rate limits. Keys are shown once, are the unit of rate limiting and observability, and must be kept server-side. Missing, unparseable, or revoked keys return 401 UNAUTHORIZED.'
  name: api-key
  scheme: bearer
  sources:
  - openapi/spaitial-ai-developer-api-openapi.json
  type: http
slug: spaitial-ai-authentication
source_filename: spaitial-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spaitial-ai-developer-api-openapi.json\ndocs: https://docs.spaitial.ai/api/authentication\nsummary:\n  types:\n  - http\n  api_key_prefixes: [spt_live_, spt_test_]\nschemes:\n- name: api-key\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: >-\n    API key issued from the developer portal (developers.spaitial.ai), sent as\n    Authorization: Bearer spt_live_<key>. Test keys use the spt_test_ prefix with\n    the same scopes and lower rate limits. Keys are shown once, are the unit of\n    rate limiting and observability, and must be kept server-side. Missing,\n    unparseable, or revoked keys return 401 UNAUTHORIZED.\n  sources:\n  - openapi/spaitial-ai-developer-api-openapi.json\nscopes:\n- scope: worlds:create\n  description: Create worlds (POST /v1/worlds) and edit panoramas (POST /v1/panoramas/edit)\n- scope: worlds:read\n  description: List, read, download worlds/panoramas/models and list\
  \ exports\n- scope: worlds:write\n  description: Update, cancel, and start exports for worlds\n- scope: files:create\n  description: Upload input files (POST /v1/files)\n- scope: files:read\n  description: List uploaded files (GET /v1/files)\nnotes:\n- Scopes are enforced server-side; calls outside granted scopes return 403 FORBIDDEN.\n- The hosted MCP server (mcp.spaitial.ai) is bring-your-own-key using the same keys, sent as X-Spaitial-Api-Key or Authorization: Bearer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaitial-ai/refs/heads/main/authentication/spaitial-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- World Models
- Spatial AI
- 3D World Generation
- Gaussian Splatting
- Generative AI
- Developer API
- MCP
- Artificial Intelligence
- 3D
---
