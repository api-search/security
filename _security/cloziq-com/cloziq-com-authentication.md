---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloziq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloziq declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloziq
provider_slug: cloziq-com
scheme_count: 1
schemes:
- applies_to: https://mcp.cloziq.com/mcp
  description: Every connection uses OAuth. Your client acts as you and can only reach your own workspace. The consent screen spells out exactly what you're granting, including write, publish, and delete.
  discovery:
  - http_status: 200
    url: https://mcp.cloziq.com/.well-known/oauth-protected-resource
  - http_status: 200
    url: https://mcp.cloziq.com/.well-known/oauth-authorization-server
  dynamic_client_registration: https://mcp.cloziq.com/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.cloziq.com/oauth/authorize
      pkce: S256
      tokenUrl: https://mcp.cloziq.com/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://clerk.app.cloziq.com/oauth/device_authorization
      tokenUrl: https://mcp.cloziq.com/oauth/token
  identity_provider: Clerk (clerk.app.cloziq.com hosts the JWKS, revocation and device endpoints)
  name: Cloziq MCP OAuth
  refresh_token: true
  revocation_endpoint: https://clerk.app.cloziq.com/oauth/token/revoke
  revoke_guidance: Disconnect the connector in your AI client, or contact support to revoke a session server-side.
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  - client_secret_post
  type: oauth2
slug: cloziq-com-authentication
source_filename: cloziq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cloziq.com/mcp\ndocs: https://cloziq.com/mcp\nname: Cloziq authentication\nnote: Cloziq publishes no REST API; its only programmable surface is the remote MCP server. Authentication was read from the MCP docs page and from the server's own OAuth discovery documents (GET only; no token, registration or authorization endpoint was called).\nschemes:\n- name: Cloziq MCP OAuth\n  type: oauth2\n  applies_to: https://mcp.cloziq.com/mcp\n  description: \"Every connection uses OAuth. Your client acts as you and can only reach your own workspace. The consent screen spells out exactly what you're granting, including write, publish, and delete.\"\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.cloziq.com/oauth/authorize\n      tokenUrl: https://mcp.cloziq.com/oauth/token\n      pkce: S256\n    deviceCode:\n      deviceAuthorizationUrl: https://clerk.app.cloziq.com/oauth/device_authorization\n      tokenUrl:\
  \ https://mcp.cloziq.com/oauth/token\n  refresh_token: true\n  dynamic_client_registration: https://mcp.cloziq.com/oauth/register\n  token_endpoint_auth_methods: [client_secret_basic, none, client_secret_post]\n  revocation_endpoint: https://clerk.app.cloziq.com/oauth/token/revoke\n  identity_provider: Clerk (clerk.app.cloziq.com hosts the JWKS, revocation and device endpoints)\n  discovery:\n  - url: https://mcp.cloziq.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://mcp.cloziq.com/.well-known/oauth-authorization-server\n    http_status: 200\n  revoke_guidance: \"Disconnect the connector in your AI client, or contact support to revoke a session server-side.\"\n"
source_yaml_url: https://artifacts.apis.io/cloziq-com/authentication/cloziq-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Sales Agent
- Instagram
- Facebook Messenger
- Direct Messaging
- Appointment-Setting
- Sales Automation
- MCP
---
