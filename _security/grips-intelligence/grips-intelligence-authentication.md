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
name: Grips Intelligence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Grips Intelligence secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Grips Intelligence
provider_slug: grips-intelligence
scheme_count: 2
schemes:
- applies_to: REST Data API (https://app.gripsintelligence.com/api/data/v1)
  description: Per-account API key passed in the `grips-api-key` request header. Keys are provisioned per contract; rate limits and quotas apply per contract terms.
  in: header
  name: gripsApiKey
  parameter_name: grips-api-key
  sources:
  - https://gripsintelligence.com/knowledge-base/api
  type: apiKey
- applies_to: Peekd Data MCP server (https://app.gripsintelligence.com/api/mcp)
  authorization_endpoint: https://app.gripsintelligence.com/authorize
  authorization_server: https://app.gripsintelligence.com/
  code_challenge_methods:
  - S256
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: peekdDataMcpOAuth
  registration_endpoint: https://app.gripsintelligence.com/register
  scopes:
  - mcp
  sources:
  - https://app.gripsintelligence.com/.well-known/oauth-authorization-server
  - https://app.gripsintelligence.com/.well-known/oauth-protected-resource/api/mcp
  token_endpoint: https://app.gripsintelligence.com/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: grips-intelligence-authentication
source_filename: grips-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://gripsintelligence.com/knowledge-base/api\ndocs: https://gripsintelligence.com/knowledge-base/api\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: gripsApiKey\n  type: apiKey\n  in: header\n  parameter_name: grips-api-key\n  applies_to: REST Data API (https://app.gripsintelligence.com/api/data/v1)\n  description: >-\n    Per-account API key passed in the `grips-api-key` request header. Keys are\n    provisioned per contract; rate limits and quotas apply per contract terms.\n  sources: [https://gripsintelligence.com/knowledge-base/api]\n- name: peekdDataMcpOAuth\n  type: oauth2\n  flow: authorizationCode        # PKCE S256\n  applies_to: Peekd Data MCP server (https://app.gripsintelligence.com/api/mcp)\n  authorization_server: https://app.gripsintelligence.com/\n  authorization_endpoint: https://app.gripsintelligence.com/authorize\n  token_endpoint: https://app.gripsintelligence.com/token\n\
  \  registration_endpoint: https://app.gripsintelligence.com/register\n  token_endpoint_auth_methods: [client_secret_post, none]\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n  scopes:\n  - mcp\n  sources:\n  - https://app.gripsintelligence.com/.well-known/oauth-authorization-server\n  - https://app.gripsintelligence.com/.well-known/oauth-protected-resource/api/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grips-intelligence/refs/heads/main/authentication/grips-intelligence-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- E-commerce Intelligence
- Competitive Intelligence
- Market Research
- Analytics
- Product Intelligence
- Retail
- Data
---
