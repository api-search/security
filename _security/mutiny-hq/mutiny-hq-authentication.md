---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mutiny Hq Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mutiny HQ secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mutiny HQ
provider_slug: mutiny-hq
scheme_count: 1
schemes:
- authorizationUrl: https://mcp.mutinyhq.com/oauth/authorize
  code_challenge_methods:
  - S256
  name: OAuth2
  registrationUrl: https://mcp.mutinyhq.com/oauth/register
  scheme: authorizationCode
  scopes:
  - read_asset_groups
  - create_asset_groups
  - publish_asset_groups
  - read_library_content
  - manage_library_content
  sources:
  - well-known/mutiny-hq-oauth-authorization-server.json
  tokenUrl: https://mcp.mutinyhq.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: mutiny-hq-authentication
source_filename: mutiny-hq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.mutinyhq.com/.well-known/oauth-authorization-server\ndocs: https://help.mutinyhq.com/articles/5947474042-setting-up-the-mutiny-mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  scheme: authorizationCode\n  authorizationUrl: https://mcp.mutinyhq.com/oauth/authorize\n  tokenUrl: https://mcp.mutinyhq.com/oauth/token\n  registrationUrl: https://mcp.mutinyhq.com/oauth/register\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_post, none]\n  scopes:\n  - read_asset_groups\n  - create_asset_groups\n  - publish_asset_groups\n  - read_library_content\n  - manage_library_content\n  sources: [well-known/mutiny-hq-oauth-authorization-server.json]\nnotes: >-\n  Mutiny's public programmatic surface is its hosted MCP server, protected by\n  OAuth 2.0 authorization-code flow with PKCE\
  \ (S256) and RFC 7591 dynamic client\n  registration. Product/CRM integrations (Segment, Salesforce, HubSpot, Marketo)\n  are configured with per-account API keys inside the Mutiny dashboard; Mutiny\n  does not publish a general-purpose REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutiny-hq/refs/heads/main/authentication/mutiny-hq-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- GTM
- Sales Enablement
- Marketing
- Website Personalization
- AI
- Agents
- MCP
- ABM
- Content Generation
---
