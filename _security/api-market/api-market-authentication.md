---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Api Market Authentication
name_suffix: Authentication
oauth_flows: []
overview: API.market declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: API.market
provider_slug: api-market
scheme_count: 2
schemes:
- applies_to:
  - Subscription Management API
  - Usage API
  - per-product APIs and MCP servers
  - MCP gateway (alternative)
  description: Pass your personal or workspace API key in the custom x-api-market-key request header.
  header: x-api-market-key
  in: header
  key_management: https://api.market/account/apiKeys
  name: apiMarketKey
  type: apiKey
- applies_to:
  - MCP gateway
  authorization_endpoint: https://api.market/api/oauth/authorize
  bearer_methods:
  - header
  flow: authorization_code
  name: mcpOAuth
  pkce:
  - S256
  registration_endpoint: https://api.market/api/oauth/register
  revocation_endpoint: https://api.market/api/oauth/revoke
  scopes:
  - mcp:use
  - offline_access
  token_endpoint: https://api.market/api/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: api-market-authentication
source_filename: api-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: searched\nsource:\n- https://docs.api.market/subscription-management-api-documentation\n- https://docs.api.market/api.market-usage-api-documentation\n- https://api.market/.well-known/oauth-authorization-server\n- https://api.market/.well-known/oauth-protected-resource/api/mcp/gateway\ndocs: https://docs.api.market/api.market-usage-api-documentation\nschemes:\n- name: apiMarketKey\n  type: apiKey\n  in: header\n  header: x-api-market-key\n  applies_to:\n  - Subscription Management API\n  - Usage API\n  - per-product APIs and MCP servers\n  - MCP gateway (alternative)\n  description: Pass your personal or workspace API key in the custom x-api-market-key request header.\n  key_management: https://api.market/account/apiKeys\n- name: mcpOAuth\n  type: oauth2\n  applies_to:\n  - MCP gateway\n  flow: authorization_code\n  pkce:\n  - S256\n  authorization_endpoint: https://api.market/api/oauth/authorize\n  token_endpoint: https://api.market/api/oauth/token\n\
  \  registration_endpoint: https://api.market/api/oauth/register\n  revocation_endpoint: https://api.market/api/oauth/revoke\n  token_endpoint_auth_methods:\n  - none\n  scopes:\n  - mcp:use\n  - offline_access\n  bearer_methods:\n  - header\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/authentication/api-market-authentication.yml
summary_line: 2 schemes
tags:
- API Marketplace
- MCP
- AI Agents
- API Monetization
- Subscription
- Usage Metering
- Authentication
---
