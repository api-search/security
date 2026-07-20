---
api_key_in: []
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Era Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Era secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Era
provider_slug: era
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://forge.era.app/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://forge.era.app/oauth/register
    scope_count: 10
    scopes_ref: scopes/era-scopes.yml
    tokenUrl: https://forge.era.app/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://forge.era.app
  name: OAuth2
  source: https://context.era.app/.well-known/oauth-authorization-server
  type: oauth2
- in: header
  name: ApiKey
  notes: Supported for developer tooling; OAuth 2.1 is the default for end-user MCP clients.
  source: developer tools (per help documentation)
  type: apiKey
slug: era-authentication
source_filename: era-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://era.app/help/mcp-server-era-context\ndocs: https://era.app/help/mcp-server-era-context\nsummary:\n  types: [oauth2, apiKey]\n  oauth2_flows: [authorizationCode]\n  oauth2_version: OAuth 2.1\n  pkce: S256\n  dynamic_client_registration: true\n  notes: OAuth 2.1 is the default for MCP clients; API keys are supported in developer\n    tools.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://context.era.app/.well-known/oauth-authorization-server\n  issuer: https://forge.era.app\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://forge.era.app/oauth/authorize\n    tokenUrl: https://forge.era.app/oauth/token\n    registrationUrl: https://forge.era.app/oauth/register\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none]\n    scope_count: 10\n    scopes_ref: scopes/era-scopes.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n\
  \  source: developer tools (per help documentation)\n  notes: Supported for developer tooling; OAuth 2.1 is the default for end-user MCP clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/era/refs/heads/main/authentication/era-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Fintech
- Artificial Intelligence
- Personal Finance
- Wealth Management
- Model Context Protocol
- MCP
- Agent Native
- Open Banking
- OAuth
---
