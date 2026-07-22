---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sesame Labs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sesame Labs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sesame Labs
provider_slug: sesame-labs
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.usenotch.ai/api/v1/mcp-auth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce_methods:
    - S256
    registrationUrl: https://app.usenotch.ai/api/v1/mcp-auth/register
    response_types:
    - code
    revocationUrl: https://app.usenotch.ai/api/v1/mcp-auth/revoke
    scopes: []
    tokenUrl: https://app.usenotch.ai/api/v1/mcp-auth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://app.usenotch.ai
  name: OAuth2
  source: https://app.usenotch.ai/.well-known/oauth-authorization-server
  type: oauth2
slug: sesame-labs-authentication
source_filename: sesame-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://app.usenotch.ai/.well-known/oauth-authorization-server\ndocs: https://app.usenotch.ai/mcp/setup\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_keys: false\n  notes: >-\n    Notch has no API-key surface. Access is exclusively via the hosted MCP\n    server, authenticated with browser-based OAuth 2.0. It is a public client\n    (token_endpoint_auth_methods = none) using PKCE (S256) and RFC 7591 dynamic\n    client registration, so MCP clients self-register with no pre-issued\n    credentials.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://app.usenotch.ai/.well-known/oauth-authorization-server\n  issuer: https://app.usenotch.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.usenotch.ai/api/v1/mcp-auth/authorize\n    tokenUrl: https://app.usenotch.ai/api/v1/mcp-auth/token\n    registrationUrl: https://app.usenotch.ai/api/v1/mcp-auth/register\n    revocationUrl:\
  \ https://app.usenotch.ai/api/v1/mcp-auth/revoke\n    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n    pkce_methods: [S256]\n    token_endpoint_auth_methods: [none]\n    scopes: []\nprotected_resource:\n  resource: https://app.usenotch.ai/mcp\n  authorization_servers: [https://app.usenotch.ai]\n  bearer_methods_supported: [header]\n  scopes_supported: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sesame-labs/refs/heads/main/authentication/sesame-labs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Advertising
- Video
- Marketing
- Generative AI
- MCP
- Agents
---
