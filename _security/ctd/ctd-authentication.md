---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Ctd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Connect The Dots declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Connect The Dots
provider_slug: ctd
scheme_count: 3
schemes:
- applies_to: CTD Paths REST API (https://api.ctd.ai/user/atc-paths-api/public/v1/)
  description: 'REST API authentication. Two headers on every request: ctd-api-key (your API key, obtained from https://app.ctd.ai/) and ctd-client-id (your account email). No OAuth flow and no SDK required.'
  header_names:
  - ctd-api-key
  - ctd-client-id
  id: apiKey
  in: header
  type: apiKey
- applies_to: CTD MCP server (https://app.ctd.ai/mcp)
  authorization_endpoint: https://app.ctd.ai/oauth/authorize
  authorization_server: https://app.ctd.ai/users-api
  description: MCP server authentication. OAuth 2.0 authorization-code with PKCE (S256) and RFC 7591 dynamic client registration; the client obtains a bearer token via the user's browser approval. No manual API keys.
  dynamic_client_registration: true
  flow: authorization_code
  id: oauth2
  pkce: S256
  scopes:
  - read
  - write
  token_endpoint: https://app.ctd.ai/users-api/v2/oauth/token
  type: oauth2
- applies_to: App / organization access
  description: SSO and SCIM provisioning available on the Business tier.
  id: sso
  source: https://ctd.ai/security
  type: enterprise
slug: ctd-authentication
source_filename: ctd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://ctd.ai/integrations-api + https://ctd.ai/integrations-mcp + OAuth well-known metadata\ndocs: https://ctd.ai/integrations-api\nschemes:\n- id: apiKey\n  type: apiKey\n  in: header\n  header_names:\n  - ctd-api-key\n  - ctd-client-id\n  description: >-\n    REST API authentication. Two headers on every request: ctd-api-key (your API\n    key, obtained from https://app.ctd.ai/) and ctd-client-id (your account email).\n    No OAuth flow and no SDK required.\n  applies_to: CTD Paths REST API (https://api.ctd.ai/user/atc-paths-api/public/v1/)\n- id: oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  dynamic_client_registration: true\n  authorization_server: https://app.ctd.ai/users-api\n  authorization_endpoint: https://app.ctd.ai/oauth/authorize\n  token_endpoint: https://app.ctd.ai/users-api/v2/oauth/token\n  scopes:\n  - read\n  - write\n  description: >-\n    MCP server authentication. OAuth 2.0 authorization-code\
  \ with PKCE (S256) and\n    RFC 7591 dynamic client registration; the client obtains a bearer token via the\n    user's browser approval. No manual API keys.\n  applies_to: CTD MCP server (https://app.ctd.ai/mcp)\n- id: sso\n  type: enterprise\n  description: SSO and SCIM provisioning available on the Business tier.\n  applies_to: App / organization access\n  source: https://ctd.ai/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctd/refs/heads/main/authentication/ctd-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Relationship Intelligence
- Sales
- Warm Introductions
- Network Graph
- CRM
- MCP
- Venture Capital
---
