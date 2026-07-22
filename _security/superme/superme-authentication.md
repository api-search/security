---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Superme Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SuperMe secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SuperMe
provider_slug: superme
scheme_count: 1
schemes:
- authorization_endpoint: https://mcp.superme.ai/authorize
  code_challenge_methods_supported:
  - S256
  issuer: https://mcp.superme.ai/
  name: OAuth2
  registration_endpoint: https://mcp.superme.ai/register
  response_types_supported:
  - code
  sources:
  - well-known/superme-oauth-authorization-server.json
  token_endpoint: https://mcp.superme.ai/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: superme-authentication
source_filename: superme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mcp.superme.ai/.well-known/oauth-authorization-server\ndocs: https://superme.ai/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256\n  dynamic_client_registration: true    # RFC 7591 registration_endpoint present\n  bearer_methods: [header]\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://mcp.superme.ai/\n  authorization_endpoint: https://mcp.superme.ai/authorize\n  token_endpoint: https://mcp.superme.ai/token\n  registration_endpoint: https://mcp.superme.ai/register\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  response_types_supported: [code]\n  sources:\n  - well-known/superme-oauth-authorization-server.json\nnotes: >-\n  Auth model derived from SuperMe's live OAuth 2.1 authorization-server metadata,\n  which fronts the hosted MCP server\
  \ (mcp.superme.ai). No public OpenAPI is\n  published for the underlying REST API (api.superme.ai auto-docs disabled), so\n  API-key/other scheme details are not documented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superme/refs/heads/main/authentication/superme-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Professional Network
- Expert Knowledge
- Model Context Protocol
- MCP
---
