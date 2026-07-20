---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Gamma Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Gamma secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Gamma
provider_slug: gamma
scheme_count: 2
schemes:
- applies_to: https://public-api.gamma.app/v1.0
  description: REST API authentication. Generate a key from Account Settings > API Keys. Requires a Pro, Ultra, Teams, or Business plan. The header name is case-sensitive.
  in: header
  key_prefix: sk-gamma-
  name: X-API-KEY
  parameter_name: X-API-KEY
  type: apiKey
- applies_to: https://mcp.gamma.app/mcp
  authorization_endpoint: https://auth.gamma.app/oauth/authorize
  authorization_server: https://auth.gamma.app
  code_challenge_methods:
  - S256
  description: Used by the official remote MCP server (https://mcp.gamma.app/mcp). OAuth 2.0 authorization-code flow with PKCE (S256) and Dynamic Client Registration (RFC 7591). Bearer token in the Authorization header.
  grant_types:
  - authorization_code
  - refresh_token
  jwks_uri: https://auth.gamma.app/.well-known/jwks.json
  name: OAuth2
  registration_endpoint: https://auth.gamma.app/oauth/register
  scopes:
  - generate
  - gamma:read
  token_endpoint: https://auth.gamma.app/oauth/token
  type: oauth2
slug: gamma-authentication
source_filename: gamma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.gamma.app/get-started/understanding-the-api-options\ndocs: https://developers.gamma.app/get-started/understanding-the-api-options\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  key_prefix: sk-gamma-\n  description: >-\n    REST API authentication. Generate a key from Account Settings > API Keys.\n    Requires a Pro, Ultra, Teams, or Business plan. The header name is\n    case-sensitive.\n  applies_to: https://public-api.gamma.app/v1.0\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Used by the official remote MCP server (https://mcp.gamma.app/mcp). OAuth 2.0\n    authorization-code flow with PKCE (S256) and Dynamic Client Registration\n    (RFC 7591). Bearer token in the Authorization header.\n  authorization_server: https://auth.gamma.app\n  authorization_endpoint:\
  \ https://auth.gamma.app/oauth/authorize\n  token_endpoint: https://auth.gamma.app/oauth/token\n  registration_endpoint: https://auth.gamma.app/oauth/register\n  jwks_uri: https://auth.gamma.app/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n  scopes: [generate, gamma:read]\n  applies_to: https://mcp.gamma.app/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamma/refs/heads/main/authentication/gamma-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Productivity
- Presentations
- Documents
- Websites
- Artificial Intelligence
- Generative AI
- Content Generation
- Design
---
