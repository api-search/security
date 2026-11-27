---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coldstate-ai-auth-api-openapi.yml
  format: yaml
  label: ColdState Auth API
  slug: coldstate-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-auth-api-openapi.yml
- filename: coldstate-ai-billing-api-openapi.yml
  format: yaml
  label: ColdState Billing API
  slug: coldstate-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-billing-api-openapi.yml
- filename: coldstate-ai-indexes-api-openapi.yml
  format: yaml
  label: ColdState Indexes API
  slug: coldstate-ai-indexes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-indexes-api-openapi.yml
- filename: coldstate-ai-knowledge-api-openapi.yml
  format: yaml
  label: ColdState Knowledge API
  slug: coldstate-ai-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-knowledge-api-openapi.yml
- filename: coldstate-ai-mcp-api-openapi.yml
  format: yaml
  label: ColdState MCP API
  slug: coldstate-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-mcp-api-openapi.yml
- filename: coldstate-ai-meta-api-openapi.yml
  format: yaml
  label: ColdState Meta API
  slug: coldstate-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-meta-api-openapi.yml
- filename: coldstate-ai-search-api-openapi.yml
  format: yaml
  label: ColdState Search API
  slug: coldstate-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-search-api-openapi.yml
- filename: coldstate-ai-usage-api-openapi.yml
  format: yaml
  label: ColdState Usage API
  slug: coldstate-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldstate-ai/openapi/coldstate-ai-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ColdState Authentication
name_suffix: Authentication
oauth_flows: []
overview: ColdState secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ColdState
provider_slug: coldstate-ai
scheme_count: 1
schemes:
- description: API key `cs_live_…` (or dashboard session `cs_sess_…`)
  docs_quote: 'All authenticated endpoints require a Bearer token in the Authorization header: Authorization: Bearer cs_live_...'
  header: 'Authorization: Bearer cs_live_...'
  key_prefixes:
  - cs_live_
  - cs_sess_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/coldstate-ai-openapi.yml
  - https://services.coldstate.ai/docs
  type: http
slug: coldstate-ai-authentication
source_filename: coldstate-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://services.coldstate.ai/docs\ndocs: https://services.coldstate.ai/docs\nsee_also:\n- https://services.coldstate.ai/docs/quickstart\n- https://services.coldstate.ai/docs/mcp\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key `cs_live_…` (or dashboard session `cs_sess_…`)\n  header: 'Authorization: Bearer cs_live_...'\n  key_prefixes:\n  - cs_live_\n  - cs_sess_\n  docs_quote: 'All authenticated endpoints require a Bearer token in the Authorization header: Authorization: Bearer cs_live_...'\n  sources:\n  - openapi/coldstate-ai-openapi.yml\n  - https://services.coldstate.ai/docs\nkey_management:\n  description: API keys are issued at signup (the register response includes the first key) and managed via /v1/auth/keys (list, create, rotate, deactivate, delete). Dashboard sessions use cs_sess_ tokens from /v1/auth/login.\n  operations:\n  - GET /v1/auth/keys\n\
  \  - POST /v1/auth/keys/create\n  - POST /v1/auth/keys/rotate\n  - POST /v1/auth/keys/{keyId}/deactivate\n  - DELETE /v1/auth/keys/{keyId}\n  - POST /v1/auth/logout\nmcp:\n  description: The MCP server at https://cold-api.coldstate.ai/mcp uses the same Bearer API key; per the docs, initialize and tools/list work without a key and tools/call requires one.\noauth: false\nnote: No OAuth, OIDC or scopes are documented; there is no test/sandbox key prefix (only cs_live_).\n"
source_yaml_url: https://artifacts.apis.io/coldstate-ai/authentication/coldstate-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Knowledge Base
- Search
- Deterministic Retrieval
- MCP
- AI Agents
- Citations
---
