---
api_key_in:
- header
api_specs:
- filename: monaco-accounts-api-openapi.yml
  format: yaml
  label: Monaco Accounts API
  slug: monaco-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-accounts-api-openapi.yml
- filename: monaco-audiences-api-openapi.yml
  format: yaml
  label: Monaco Audiences API
  slug: monaco-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-audiences-api-openapi.yml
- filename: monaco-auth-api-openapi.yml
  format: yaml
  label: Monaco Auth API
  slug: monaco-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-auth-api-openapi.yml
- filename: monaco-campaigns-api-openapi.yml
  format: yaml
  label: Monaco Campaigns API
  slug: monaco-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-campaigns-api-openapi.yml
- filename: monaco-contacts-api-openapi.yml
  format: yaml
  label: Monaco Contacts API
  slug: monaco-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-contacts-api-openapi.yml
- filename: monaco-meetings-api-openapi.yml
  format: yaml
  label: Monaco Meetings API
  slug: monaco-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-meetings-api-openapi.yml
- filename: monaco-opportunities-api-openapi.yml
  format: yaml
  label: Monaco Opportunities API
  slug: monaco-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-opportunities-api-openapi.yml
- filename: monaco-schemas-api-openapi.yml
  format: yaml
  label: Monaco Schemas API
  slug: monaco-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-schemas-api-openapi.yml
- filename: monaco-sequence-templates-api-openapi.yml
  format: yaml
  label: Monaco Sequence Templates API
  slug: monaco-sequence-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-sequence-templates-api-openapi.yml
- filename: monaco-sequences-api-openapi.yml
  format: yaml
  label: Monaco Sequences API
  slug: monaco-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-sequences-api-openapi.yml
- filename: monaco-tags-api-openapi.yml
  format: yaml
  label: Monaco Tags API
  slug: monaco-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-tags-api-openapi.yml
- filename: monaco-tasks-api-openapi.yml
  format: yaml
  label: Monaco Tasks API
  slug: monaco-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-tasks-api-openapi.yml
- filename: monaco-users-api-openapi.yml
  format: yaml
  label: Monaco Users API
  slug: monaco-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Monaco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monaco secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Monaco
provider_slug: monaco
scheme_count: 2
schemes:
- description: Monaco's public REST API uses API-key authentication. Every request must include a valid API key in the Authorization header as a bearer token. Keys are created in the Monaco app (Settings > API Keys); the plaintext value (prefix mks_) is shown only once and stored as a hash server-side.
  format: Bearer mks_<48-char-url-safe-token>
  header: Authorization
  in: header
  key_prefix: mks_
  name: apiKeyBearer
  scheme: bearer
  scoping: Each API key is scoped to an organization and optionally tied to a specific user. If no user is set, the key operates as the user who created it.
  sources:
  - docs
  type: http
- description: The hosted MCP server at https://mcp.monaco.com/mcp authenticates via OAuth 2.0; the MCP client handles the authorization flow on first connection. Every request is authenticated as the user who completed login and respects that user's Monaco permissions. API-key bearer auth is also supported for Codex/ChatGPT MCP connections.
  name: oauth2Mcp
  sources:
  - docs
  type: oauth2
slug: monaco-authentication
source_filename: monaco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.monaco.com/auth\ndocs: https://docs.monaco.com/auth\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_scheme: bearer\n  oauth2_flows: []\n  note: >-\n    The OpenAPI spec (api.monaco.com/openapi.json) declares no securitySchemes;\n    the authentication model below is captured from the published docs. The MCP\n    server (mcp.monaco.com) uses OAuth 2.0 in addition to API-key bearer auth.\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Bearer mks_<48-char-url-safe-token>\"\n  key_prefix: mks_\n  description: >-\n    Monaco's public REST API uses API-key authentication. Every request must\n    include a valid API key in the Authorization header as a bearer token. Keys\n    are created in the Monaco app (Settings > API Keys); the plaintext value\n    (prefix mks_) is shown only once and stored as a hash server-side.\n  scoping: >-\n\
  \    Each API key is scoped to an organization and optionally tied to a specific\n    user. If no user is set, the key operates as the user who created it.\n  sources: [docs]\n- name: oauth2Mcp\n  type: oauth2\n  description: >-\n    The hosted MCP server at https://mcp.monaco.com/mcp authenticates via OAuth\n    2.0; the MCP client handles the authorization flow on first connection.\n    Every request is authenticated as the user who completed login and respects\n    that user's Monaco permissions. API-key bearer auth is also supported for\n    Codex/ChatGPT MCP connections.\n  sources: [docs]\nkey_management:\n  deactivation: Keys can be deactivated from Settings; deactivated keys are immediately rejected.\n  rotation: No in-place rotation. Create a new key, migrate, then deactivate the old key.\nauth_errors:\n- status: 401\n  meaning: Missing or invalid API key.\n- status: 403\n  meaning: API key is valid but lacks required access.\n- status: 429\n  meaning: Rate limit exceeded.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/authentication/monaco-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- CRM
- Sales
- Revenue Operations
- Artificial Intelligence
- Contacts
- Account
- Opportunities
- Pipeline
- Go-To-Market
- MCP
- Campaigns
- Audiences
- Sales Engagement
- Agents
---
