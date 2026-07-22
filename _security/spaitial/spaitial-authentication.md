---
api_key_in: []
api_specs:
- filename: spaitial-developer-api-openapi.json
  format: json
  label: SpAItial Developer API
  slug: spaitial-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaitial/refs/heads/main/openapi/spaitial-developer-api-openapi.json
auth_types:
- http
description: The SpAItial Developer API authenticates with a bearer API key issued from the developer portal (developers.spaitial.ai). Keys are scoped and enforced server-side; the hosted MCP server accepts the same keys (BYOK) as either a Bearer token or an X-Spaitial-Api-Key header, and additionally advertises OAuth 2.0 in its MCP server card.
kind: authentication
layout: security
method: searched
name: Spaitial Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpAItial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpAItial
provider_slug: spaitial
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Bearer API key issued by the developers site. Production keys look like spt_live_<32-char-base32>; test keys use the spt_test_ prefix (same scopes, lower rate limits). Keys are shown once at creation. A missing, unparseable, or revoked key returns 401 UNAUTHORIZED.
  header: Authorization
  in: header
  name: api-key
  scheme: bearer
  sources:
  - openapi/spaitial-developer-api-openapi.json
  type: http
slug: spaitial-authentication
source_filename: spaitial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://docs.spaitial.ai/api/authentication, https://docs.spaitial.ai/api/llm-skills,\n  and the securitySchemes in openapi/spaitial-developer-api-openapi.json.\ndescription: >-\n  The SpAItial Developer API authenticates with a bearer API key issued from the\n  developer portal (developers.spaitial.ai). Keys are scoped and enforced\n  server-side; the hosted MCP server accepts the same keys (BYOK) as either a\n  Bearer token or an X-Spaitial-Api-Key header, and additionally advertises\n  OAuth 2.0 in its MCP server card.\nsummary:\n  types:\n    - http\nschemes:\n  - name: api-key\n    type: http\n    scheme: bearer\n    bearerFormat: API Key\n    in: header\n    header: Authorization\n    description: >-\n      Bearer API key issued by the developers site. Production keys look like\n      spt_live_<32-char-base32>; test keys use the spt_test_ prefix (same scopes,\n      lower rate limits). Keys are shown once at creation.\
  \ A missing, unparseable,\n      or revoked key returns 401 UNAUTHORIZED.\n    sources:\n      - openapi/spaitial-developer-api-openapi.json\nkey_format:\n  production_prefix: spt_live_\n  test_prefix: spt_test_\n  example: spt_live_abc123def456...\nscopes:\n  enforcement: Server-side; a call outside the granted scopes returns 403 FORBIDDEN.\n  values:\n    - {scope: 'worlds:create', grants: 'POST /v1/worlds, POST /v1/panoramas/edit'}\n    - {scope: 'worlds:read', grants: 'GET world requests/status/result/exports/splat/panorama, GET panoramas, GET models'}\n    - {scope: 'worlds:write', grants: 'PATCH world, cancel job, start export'}\n    - {scope: 'files:create', grants: 'POST /v1/files'}\n    - {scope: 'files:read', grants: 'GET /v1/files'}\n  detail: scopes/spaitial-scopes.yml\nmcp_auth:\n  server: https://mcp.spaitial.ai/mcp\n  byok: true\n  schemes: [bearer, oauth2]\n  headers: ['X-Spaitial-Api-Key: spt_live_...', 'Authorization: Bearer spt_live_...']\nrevocation:\n  mechanism: Revoke\
  \ a key from the developer portal; takes effect on the next request.\n  note: Creating a new key does not invalidate existing ones — revoke the old key explicitly.\ndocs: https://docs.spaitial.ai/api/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaitial/refs/heads/main/authentication/spaitial-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Spatial AI
- World Models
- 3D
- Gaussian Splatting
- Generative AI
- Developer API
- MCP
---
