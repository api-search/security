---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hockeystack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HockeyStack secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HockeyStack
provider_slug: hockeystack
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization-code flow (PKCE / S256) protecting the HockeyStack Omni MCP server. Supports refresh tokens and RFC 7591 dynamic client registration. Access tokens are presented as Bearer tokens in the Authorization header against the protected resource https://hockeystack.com/api/mcp/omni.
  flows:
  - authorizationUrl: https://hockeystack.com/api/mcp/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://hockeystack.com/api/mcp/oauth/token
    scopes:
      omni:tools: Access to HockeyStack Omni agent tools
    tokenUrl: https://hockeystack.com/api/mcp/oauth/token
  name: OmniOAuth2
  registration_endpoint: https://hockeystack.com/api/mcp/oauth/register
  revocation_endpoint: https://hockeystack.com/api/mcp/oauth/revoke
  sources:
  - well-known/hockeystack-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: hockeystack-authentication
source_filename: hockeystack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://app.hockeystack.com/.well-known/oauth-authorization-server\ndocs: https://docs.hockeystack.com/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  dynamic_client_registration: true\n  bearer_methods:\n  - header\nschemes:\n- name: OmniOAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code flow (PKCE / S256) protecting the HockeyStack\n    Omni MCP server. Supports refresh tokens and RFC 7591 dynamic client\n    registration. Access tokens are presented as Bearer tokens in the\n    Authorization header against the protected resource\n    https://hockeystack.com/api/mcp/omni.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hockeystack.com/api/mcp/oauth/authorize\n    tokenUrl: https://hockeystack.com/api/mcp/oauth/token\n    refreshUrl: https://hockeystack.com/api/mcp/oauth/token\n    scopes:\n      omni:tools: Access to HockeyStack Omni\
  \ agent tools\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  registration_endpoint: https://hockeystack.com/api/mcp/oauth/register\n  revocation_endpoint: https://hockeystack.com/api/mcp/oauth/revoke\n  sources:\n  - well-known/hockeystack-oauth-authorization-server.json\nnotes: >-\n  HockeyStack does not publish a general-purpose REST API with an OpenAPI spec;\n  its programmatic surface is the hosted Omni MCP server, authenticated via this\n  OAuth 2.0 authorization server. Product data integrations are otherwise\n  configured through prebuilt connectors (Salesforce, HubSpot, ad platforms,\n  Snowflake, BigQuery, Segment) inside the app rather than a public API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hockeystack/refs/heads/main/authentication/hockeystack-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Data
- Marketing Analytics
- Attribution
- Revenue Intelligence
- B2B
- Account Intelligence
- MCP
- AI Agents
---
