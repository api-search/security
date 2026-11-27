---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ctxstore-ai-account-api-openapi.yml
  format: yaml
  label: ctxstore.ai Account API
  slug: ctxstore-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-account-api-openapi.yml
- filename: ctxstore-ai-admin-api-openapi.yml
  format: yaml
  label: ctxstore.ai Admin API
  slug: ctxstore-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-admin-api-openapi.yml
- filename: ctxstore-ai-context-api-openapi.yml
  format: yaml
  label: ctxstore.ai Context API
  slug: ctxstore-ai-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-context-api-openapi.yml
- filename: ctxstore-ai-events-api-openapi.yml
  format: yaml
  label: ctxstore.ai Events API
  slug: ctxstore-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-events-api-openapi.yml
- filename: ctxstore-ai-facts-api-openapi.yml
  format: yaml
  label: ctxstore.ai Facts API
  slug: ctxstore-ai-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-facts-api-openapi.yml
- filename: ctxstore-ai-openapi-json-api-openapi.yml
  format: yaml
  label: ctxstore.ai Openapi.json API
  slug: ctxstore-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-openapi-json-api-openapi.yml
- filename: ctxstore-ai-search-api-openapi.yml
  format: yaml
  label: ctxstore.ai Search API
  slug: ctxstore-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-search-api-openapi.yml
- filename: ctxstore-ai-stats-api-openapi.yml
  format: yaml
  label: ctxstore.ai Stats API
  slug: ctxstore-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-stats-api-openapi.yml
- filename: ctxstore-ai-users-api-openapi.yml
  format: yaml
  label: ctxstore.ai Users API
  slug: ctxstore-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ctxstore.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ctxstore.ai secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ctxstore.ai
provider_slug: ctxstore-ai
scheme_count: 3
schemes:
- applies_to:
  - REST API https://ctxstore.ai/api/v1
  - MCP server https://mcp.ctxstore.ai/mcp
  description: 'API key from ctxstore.ai dashboard. Format: Bearer emk_...'
  docs_quote: Persistent API keys ( emk_… ) for everything else, activated by a one-time email code.
  key_prefix: emk_
  name: BearerAuth
  rotation: Keys can be rotated from your account page without losing any stored memory.
  scheme: bearer
  sources:
  - openapi/ctxstore-ai-openapi.yml
  - https://ctxstore.ai/security
  type: http
- applies_to:
  - MCP server https://mcp.ctxstore.ai/mcp
  authorization_server_metadata: https://ctxstore.ai/.well-known/oauth-authorization-server
  client_type: public
  description: OAuth 2.1 (dynamic client registration + PKCE S256) is also live, for clients that authorize in a browser instead of holding a key. An unauthenticated tools/call on a session answers 401 with WWW-Authenticate Bearer resource_metadata; initialize, tools/list and setup_account stay open.
  dynamic_client_registration: true
  flows:
  - authorizationCode
  name: OAuth 2.1 (MCP)
  note: Documented only; not declared in the OpenAPI securitySchemes. Discovery URLs recorded from the docs, not called by this module.
  pkce: S256
  protected_resource_metadata: https://mcp.ctxstore.ai/.well-known/oauth-protected-resource
  scopes:
  - mcp:read
  - mcp:write
  sources:
  - https://ctxstore.ai/llms-full.txt
  token_endpoint_auth_method: none
  type: oauth2
- description: Connecting an assistant to https://mcp.ctxstore.ai/try creates a trial account on the first request. No email, no key. The trial URL is the key; keep it to reconnect.
  name: Trial URL
  sources:
  - https://ctxstore.ai/pricing
  type: url-capability
slug: ctxstore-ai-authentication
source_filename: ctxstore-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://ctxstore.ai/llms-full.txt\ndocs: https://ctxstore.ai/docs\ndocs_urls:\n- https://ctxstore.ai/llms-full.txt\n- https://ctxstore.ai/docs\n- https://ctxstore.ai/security\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from ctxstore.ai dashboard. Format: Bearer emk_...'\n  key_prefix: emk_\n  applies_to: [REST API https://ctxstore.ai/api/v1, MCP server https://mcp.ctxstore.ai/mcp]\n  docs_quote: Persistent API keys ( emk_… ) for everything else, activated by a one-time email code.\n  rotation: Keys can be rotated from your account page without losing any stored memory.\n  sources:\n  - openapi/ctxstore-ai-openapi.yml\n  - https://ctxstore.ai/security\n- name: OAuth 2.1 (MCP)\n  type: oauth2\n  flows: [authorizationCode]\n  pkce: S256\n  dynamic_client_registration: true\n  client_type: public\n  token_endpoint_auth_method: none\n  scopes: ['mcp:read',\
  \ 'mcp:write']\n  applies_to: [MCP server https://mcp.ctxstore.ai/mcp]\n  protected_resource_metadata: https://mcp.ctxstore.ai/.well-known/oauth-protected-resource\n  authorization_server_metadata: https://ctxstore.ai/.well-known/oauth-authorization-server\n  description: OAuth 2.1 (dynamic client registration + PKCE S256) is also live, for clients that authorize in a browser instead of holding a key. An unauthenticated tools/call on a session answers 401 with WWW-Authenticate Bearer resource_metadata; initialize, tools/list and setup_account stay open.\n  note: Documented only; not declared in the OpenAPI securitySchemes. Discovery URLs recorded from the docs, not called by this module.\n  sources:\n  - https://ctxstore.ai/llms-full.txt\n- name: Trial URL\n  type: url-capability\n  description: Connecting an assistant to https://mcp.ctxstore.ai/try creates a trial account on the first request. No email, no key. The trial URL is the key; keep it to reconnect.\n  sources:\n  - https://ctxstore.ai/pricing\n\
  notes:\n- 'Calling /mcp or /api/v1 directly? Send a real User-Agent header; default python-urllib is blocked at the edge.'\n"
source_yaml_url: https://artifacts.apis.io/ctxstore-ai/authentication/ctxstore-ai-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- AI Agents
- Memory
- MCP
- Context Management
- Developer Tools
---
