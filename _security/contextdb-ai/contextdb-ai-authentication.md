---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contextdb-ai-decisions-api-openapi.yml
  format: yaml
  label: ContextDB Decisions API
  slug: contextdb-ai-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-decisions-api-openapi.yml
- filename: contextdb-ai-mcp-api-openapi.yml
  format: yaml
  label: ContextDB MCP API
  slug: contextdb-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-mcp-api-openapi.yml
- filename: contextdb-ai-memory-api-openapi.yml
  format: yaml
  label: ContextDB Memory API
  slug: contextdb-ai-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-memory-api-openapi.yml
- filename: contextdb-ai-meta-api-openapi.yml
  format: yaml
  label: ContextDB Meta API
  slug: contextdb-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-meta-api-openapi.yml
- filename: contextdb-ai-oauth-api-openapi.yml
  format: yaml
  label: ContextDB OAuth API
  slug: contextdb-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-oauth-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Contextdb Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ContextDB secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ContextDB
provider_slug: contextdb-ai
scheme_count: 2
schemes:
- description: Project-wide server credential (`cdb_…`). Never in browsers.
  name: ProjectKey
  scheme: bearer
  sources:
  - openapi/contextdb-ai-openapi.yaml
  type: http
- description: User-bound marketplace connector grant (`cmo_…`).
  flows:
  - authorizationUrl: https://app.contextdb.ai/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.contextdb.ai/oauth/token
  name: McpOAuth
  sources:
  - openapi/contextdb-ai-openapi.yaml
  type: oauth2
slug: contextdb-ai-authentication
source_filename: contextdb-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/contextdb-ai-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ProjectKey\n  type: http\n  scheme: bearer\n  description: Project-wide server credential (`cdb_…`). Never in browsers.\n  sources:\n  - openapi/contextdb-ai-openapi.yaml\n- name: McpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.contextdb.ai/oauth/authorize\n    tokenUrl: https://api.contextdb.ai/oauth/token\n    scopes: 3\n  description: User-bound marketplace connector grant (`cmo_…`).\n  sources:\n  - openapi/contextdb-ai-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/contextdb-ai/authentication/contextdb-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Memory
- Customer Data
- Agent Platform
- Context
---
