---
api_key_in: []
api_specs:
- filename: adapter-openapi.json
  format: json
  label: Adapter Cognition API
  slug: adapter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapter/refs/heads/main/openapi/adapter-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Adapter Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Adapter secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Adapter
provider_slug: adapter
scheme_count: 3
schemes:
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/adapter-openapi.json
  type: http
  usage: Protects the documentation endpoints (/docs, /redoc, /openapi.json).
- bearerFormat: JWT
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/adapter-openapi.json
  type: http
  usage: Primary end-user auth for the Adapter Life API (users/me/*, conversations, assets, oauth-connect).
- flows:
  - authorizationUrl: https://api.adapter.com/v1/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
    - mcp:read
    - offline_access
    tokenUrl: https://api.adapter.com/v1/oauth2/token
  name: OAuth2
  sources:
  - https://api.adapter.com/.well-known/oauth-authorization-server
  type: oauth2
  usage: Adapter is itself an OAuth 2.0 authorization server (RFC 8414 metadata at /.well-known/oauth-authorization-server); external apps and agents obtain tokens via the authorization_code + PKCE flow to reach the hosted MCP surface.
slug: adapter-authentication
source_filename: adapter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/adapter-openapi.json + https://api.adapter.com/.well-known/oauth-authorization-server\ndocs: https://api.adapter.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  usage: Protects the documentation endpoints (/docs, /redoc, /openapi.json).\n  sources:\n  - openapi/adapter-openapi.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  usage: Primary end-user auth for the Adapter Life API (users/me/*, conversations, assets, oauth-connect).\n  sources:\n  - openapi/adapter-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.adapter.com/v1/oauth2/authorize\n    tokenUrl: https://api.adapter.com/v1/oauth2/token\n    pkce: S256\n    scopes: [mcp:read, offline_access]\n  usage: >-\n    Adapter is\
  \ itself an OAuth 2.0 authorization server (RFC 8414 metadata at\n    /.well-known/oauth-authorization-server); external apps and agents obtain\n    tokens via the authorization_code + PKCE flow to reach the hosted MCP surface.\n  sources:\n  - https://api.adapter.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapter/refs/heads/main/authentication/adapter-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Ai
- Cognition
- Knowledge Graph
- Memory
- Agents
- MCP
- LLM
---
