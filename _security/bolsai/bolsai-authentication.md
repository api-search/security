---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: openapi.json
  format: json
  label: Bolsai Financial Data API
  slug: bolsai-financial-data-api
  spec_type: OpenAPI
  url: https://usebolsai.com/openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Bolsai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bolsai secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bolsai
provider_slug: bolsai
scheme_count: 4
schemes:
- description: Get your key at POST /api/v1/keys/register
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/bolsai-openapi.json
  type: apiKey
- description: Documented alternative to the header in llms.txt ("?api_key=...").
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - https://usebolsai.com/llms.txt
  type: apiKey
- description: 'Documented alternative in llms.txt ("Authorization: Bearer ..."); also the token style for the hosted MCP endpoint.'
  name: BearerToken
  scheme: bearer
  sources:
  - https://usebolsai.com/llms.txt
  type: http
- authorization_url: https://usebolsai.com/api/v1/oauth/authorize
  description: OAuth 2.0 authorization server (RFC 8414 metadata live at /.well-known/oauth-authorization-server) protecting the hosted MCP endpoint https://usebolsai.com/api/mcp (RFC 9728) and used by the ChatGPT GPT-Actions integration. Public clients with PKCE; no scopes are published.
  flow: authorization_code
  name: McpOAuth
  pkce: S256
  registration_url: https://usebolsai.com/api/v1/oauth/register
  scopes: {}
  sources:
  - https://usebolsai.com/.well-known/oauth-authorization-server
  - https://usebolsai.com/mcp
  token_url: https://usebolsai.com/api/v1/oauth/token
  type: oauth2
slug: bolsai-authentication
source_filename: bolsai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/bolsai-openapi.json\ndocs: https://usebolsai.com/docs\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Get your key at POST /api/v1/keys/register\n  sources:\n  - openapi/bolsai-openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Documented alternative to the header in llms.txt (\"?api_key=...\").\n  sources:\n  - https://usebolsai.com/llms.txt\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: 'Documented alternative in llms.txt (\"Authorization: Bearer ...\"); also the token style for the hosted MCP endpoint.'\n  sources:\n  - https://usebolsai.com/llms.txt\n- name: McpOAuth\n  type: oauth2\n  flow: authorization_code\n  authorization_url: https://usebolsai.com/api/v1/oauth/authorize\n  token_url: https://usebolsai.com/api/v1/oauth/token\n\
  \  registration_url: https://usebolsai.com/api/v1/oauth/register\n  pkce: S256\n  scopes: {}\n  description: >-\n    OAuth 2.0 authorization server (RFC 8414 metadata live at\n    /.well-known/oauth-authorization-server) protecting the hosted MCP endpoint\n    https://usebolsai.com/api/mcp (RFC 9728) and used by the ChatGPT GPT-Actions\n    integration. Public clients with PKCE; no scopes are published.\n  sources:\n  - https://usebolsai.com/.well-known/oauth-authorization-server\n  - https://usebolsai.com/mcp\nkey_management:\n  signup: Google login at https://usebolsai.com (free, no card)\n  active_key_limits: {Free: 5, Pro: 20}\n  operations:\n    create: create_key_api_v1_keys_post\n    rotate: rotate_key_api_v1_keys__key_id__rotate_post\n    delete: delete_key_api_v1_keys__key_id__delete\n    usage: get_usage_api_v1_keys_usage_get\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/authentication/bolsai-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Finance
- Financial Data
- Market Data
- Stocks/equities
- Real Estate Funds
- Dividends
- Fundamentals
- Macroeconomic Data
- Brazil
- Developer Tools
- MCP
- AI Agents
---
