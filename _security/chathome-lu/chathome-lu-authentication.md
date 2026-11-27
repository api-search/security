---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: chathome-lu-agent-api-openapi.yml
  format: yaml
  label: ChatHome Protected Agent API
  slug: protected-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-agent-api-openapi.yml
- filename: chathome-lu-agents-api-openapi.yml
  format: yaml
  label: ChatHome Agents API
  slug: chathome-lu-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-agents-api-openapi.yml
- filename: chathome-lu-listings-api-openapi.yml
  format: yaml
  label: ChatHome Listings API
  slug: chathome-lu-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-listings-api-openapi.yml
- filename: chathome-lu-market-data-api-openapi.yml
  format: yaml
  label: ChatHome Market data API
  slug: chathome-lu-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-market-data-api-openapi.yml
- filename: chathome-lu-search-api-openapi.yml
  format: yaml
  label: ChatHome Search API
  slug: chathome-lu-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-search-api-openapi.yml
auth_types:
- none
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ChatHome Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChatHome secures its APIs with none, apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ChatHome
provider_slug: chathome-lu
scheme_count: 3
schemes:
- description: 'llms.txt: "Generate a key at: https://chathome.lu/dashboard/agent-access / Pass as header: X-API-Key: cht_<key>". The developer portal shows a key format beginning ch_ ("ch_a1b2c3d4...") and states "Keys are shown once at creation".'
  in: header
  key_prefixes_documented:
  - cht_ (llms.txt)
  - ch_ (developer portal example)
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/chathome-lu-agent-api-openapi.yml
  - https://chathome.lu/llms.txt
  - https://chathome.lu/en/developers
  type: apiKey
- description: Use the ChatHome MCP OAuth token, bound to /api/mcp, with market:read scope.
  name: bearer
  scheme: bearer
  sources:
  - openapi/chathome-lu-agent-api-openapi.yml
  type: http
- description: 'llms.txt: "OAuth 2.1 with PKCE (recommended). This server uses PUBLIC OAuth clients — no client secret is required." Documented client IDs: claude-desktop, cursor, chatgpt. "OAuth tokens expire after 1 hour (clients auto-refresh)".'
  flow: authorization_code
  metadata_url: https://chathome.lu/.well-known/oauth-authorization-server
  name: oauth2-pkce
  pkce: S256
  public_clients: true
  scopes:
  - listings:read
  - market:read
  - inquiries:write
  - inquiries:read
  - documents:write
  sources:
  - https://chathome.lu/llms.txt
  - https://chathome.lu/.well-known/oauth-authorization-server (GET 200, grant_types_supported [authorization_code], code_challenge_methods_supported [S256])
  token_lifetime: 1 hour
  type: oauth2
slug: chathome-lu-authentication
source_filename: chathome-lu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chathome.lu/llms.txt\ndocs: https://chathome.lu/en/developers\nsummary:\n  types:\n  - none\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  anonymous_surface: The public read API (openapi/chathome-lu-openapi.yml) declares no security; its description states \"Every endpoint in this document answers WITHOUT an account, an API key, or an OAuth\n    token.\" Anonymous MCP discovery and public discovery tools are also callable without credentials.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'llms.txt: \"Generate a key at: https://chathome.lu/dashboard/agent-access / Pass as header: X-API-Key: cht_<key>\". The developer portal shows a key format beginning ch_ (\"ch_a1b2c3d4...\")\n    and states \"Keys are shown once at creation\".'\n  key_prefixes_documented:\n  - cht_ (llms.txt)\n  - ch_ (developer portal example)\n  sources:\n  - openapi/chathome-lu-agent-api-openapi.yml\n\
  \  - https://chathome.lu/llms.txt\n  - https://chathome.lu/en/developers\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Use the ChatHome MCP OAuth token, bound to /api/mcp, with market:read scope.\n  sources:\n  - openapi/chathome-lu-agent-api-openapi.yml\n- name: oauth2-pkce\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  public_clients: true\n  description: 'llms.txt: \"OAuth 2.1 with PKCE (recommended). This server uses PUBLIC OAuth clients — no client secret is required.\" Documented client IDs: claude-desktop, cursor, chatgpt. \"OAuth tokens\n    expire after 1 hour (clients auto-refresh)\".'\n  metadata_url: https://chathome.lu/.well-known/oauth-authorization-server\n  scopes:\n  - listings:read\n  - market:read\n  - inquiries:write\n  - inquiries:read\n  - documents:write\n  token_lifetime: 1 hour\n  sources:\n  - https://chathome.lu/llms.txt\n  - https://chathome.lu/.well-known/oauth-authorization-server (GET 200, grant_types_supported [authorization_code],\
  \ code_challenge_methods_supported [S256])\nunauthenticated_response: Protected MCP tool calls \"answer 401 with a WWW-Authenticate header pointing at the OAuth metadata\" (llms.txt).\nrelated_docs:\n- https://chathome.lu/llms.txt\n- https://chathome.lu/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/chathome-lu/authentication/chathome-lu-authentication.yml
summary_line: none/apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Real Estate
- Property Search
- Luxembourg
- Housing
- Property Valuation
- AI Agents
- MCP
- A2A
---
