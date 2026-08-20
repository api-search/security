---
api_key_in:
- header
api_specs:
- filename: parallel-chat-api-beta-api-openapi.yml
  format: yaml
  label: Parallel Chat API (Beta) API
  slug: parallel-chat-api-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-chat-api-beta-api-openapi.yml
- filename: parallel-extract-api-openapi.yml
  format: yaml
  label: Parallel Extract API
  slug: parallel-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-extract-api-openapi.yml
- filename: parallel-findall-api-openapi.yml
  format: yaml
  label: Parallel FindAll API
  slug: parallel-findall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-findall-api-openapi.yml
- filename: parallel-monitor-api-openapi.yml
  format: yaml
  label: Parallel Monitor API
  slug: parallel-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-monitor-api-openapi.yml
- filename: parallel-search-api-openapi.yml
  format: yaml
  label: Parallel Search API
  slug: parallel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-search-api-openapi.yml
- filename: parallel-tasks-api-openapi.yml
  format: yaml
  label: Parallel Tasks API
  slug: parallel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-tasks-api-openapi.yml
- filename: parallel-responses-api-openapi.yml
  format: yaml
  label: Parallel Responses API
  slug: parallel-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-responses-api-openapi.yml
- filename: parallel-memory-api-openapi.yml
  format: yaml
  label: Parallel Memory API
  slug: parallel-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-memory-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Parallel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parallel secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Parallel
provider_slug: parallel
scheme_count: 2
schemes:
- applies_to: https://api.parallel.ai REST API (all operations)
  env_var: PARALLEL_API_KEY
  in: header
  key_management: https://platform.parallel.ai (default key generated at signup; manage under Settings)
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/_original/parallel-openapi-original.json
  type: apiKey
- applies_to:
  - https://task-mcp.parallel.ai/mcp
  - https://search.parallel.ai/mcp-oauth
  - https://api.parallel.ai/a2a
  - parallel-cli login
  dynamic_client_registration: true
  flows:
  - authorization_url: https://platform.parallel.ai/getKeys/authorize
    pkce: S256
    scopes:
    - key:read
    token_url: https://platform.parallel.ai/getKeys/token
    type: authorizationCode
  - device_authorization_endpoint: https://platform.parallel.ai/getKeys/device/code
    scopes:
    - key:read
    type: deviceCode
  name: parallel_oauth
  registration_endpoint: https://platform.parallel.ai/getKeys/register
  sources:
  - well-known/parallel-oauth-authorization-server.json
  - well-known/parallel-task-mcp-oauth-protected-resource.json
  - a2a/parallel-agent-card.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: parallel-authentication
source_filename: parallel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  openapi/_original/parallel-openapi-original.json +\n  https://docs.parallel.ai/resources/faqs +\n  https://platform.parallel.ai/.well-known/oauth-authorization-server (probed 200)\nnotes: >-\n  Two distinct authentication regimes. The REST API is API-key only. The AGENT\n  surfaces (Task MCP, A2A Deep Research agent, CLI login) additionally accept\n  OAuth 2.0 against an authorization server at platform.parallel.ai whose\n  metadata is publicly published — it supports dynamic client registration, PKCE\n  (S256), authorization_code and device_code, and a single scope `key:read`. The\n  OAuth exchange returns a Parallel API key used as a bearer token.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applies_to: https://api.parallel.ai REST API (all operations)\n  key_management: https://platform.parallel.ai (default\
  \ key generated at signup; manage under Settings)\n  env_var: PARALLEL_API_KEY\n  sources:\n  - openapi/_original/parallel-openapi-original.json\n- name: parallel_oauth\n  type: oauth2\n  flows:\n  - type: authorizationCode\n    authorization_url: https://platform.parallel.ai/getKeys/authorize\n    token_url: https://platform.parallel.ai/getKeys/token\n    pkce: S256\n    scopes: [key:read]\n  - type: deviceCode\n    device_authorization_endpoint: https://platform.parallel.ai/getKeys/device/code\n    scopes: [key:read]\n  registration_endpoint: https://platform.parallel.ai/getKeys/register\n  dynamic_client_registration: true\n  token_endpoint_auth_methods_supported: [none]\n  applies_to:\n  - https://task-mcp.parallel.ai/mcp\n  - https://search.parallel.ai/mcp-oauth\n  - https://api.parallel.ai/a2a\n  - parallel-cli login\n  sources:\n  - well-known/parallel-oauth-authorization-server.json\n  - well-known/parallel-task-mcp-oauth-protected-resource.json\n  - a2a/parallel-agent-card.json\n\
  bearer:\n  supported: true\n  note: >-\n    A Parallel API key may also be presented as `Authorization: Bearer <key>` on\n    the MCP endpoints (documented for raising Search MCP rate limits).\nanonymous:\n  supported: true\n  surfaces:\n  - https://search.parallel.ai/mcp\n  note: The free Search MCP requires no account and no key; session_id is used for free-tier rate limiting.\nwebhook_auth:\n  standard: Standard Webhooks\n  algorithm: HMAC-SHA256\n  secret_prefix: whsec_\n  see: asyncapi/parallel-webhooks.yml\nscopes: scopes/parallel-scopes.yml\ndocs: https://docs.parallel.ai/getting-started/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/authentication/parallel-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Web Search
- Agents
- Deep Research
- Web Extraction
- Data Enrichment
- Web Monitoring
- LLM Tools
---
