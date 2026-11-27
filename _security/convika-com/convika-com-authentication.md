---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Convika Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convika declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Convika
provider_slug: convika-com
scheme_count: 1
schemes:
- applies_to: https://mcp.convika.com/mcp
  bearer_methods:
  - header
  dynamic_client_registration: https://mcp.convika.com/register
  evidence: https://mcp.convika.com/.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.convika.com/authorize
      scopes:
        mcp:connect: Connect an MCP client to Convika
        offline_access: Refresh tokens
      tokenUrl: https://mcp.convika.com/token
  jwks_uri: https://mcp.convika.com/jwks
  name: convika-oauth
  pkce: S256
  revocation_endpoint: https://mcp.convika.com/revoke
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: convika-com-authentication
source_filename: convika-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://convika.com/docs/\ndocs: https://convika.com/docs/\nsummary: The Convika MCP server (https://mcp.convika.com/mcp, Streamable HTTP) uses OAuth 2.1 sign-in; the docs state \"Convika uses OAuth sign-in and does not require an API key.\" Authorization server metadata (GET https://mcp.convika.com/.well-known/oauth-authorization-server, HTTP 200) advertises authorization_code + refresh_token grants, PKCE S256, dynamic client registration and token revocation.\nschemes:\n- name: convika-oauth\n  type: oauth2\n  applies_to: https://mcp.convika.com/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.convika.com/authorize\n      tokenUrl: https://mcp.convika.com/token\n      scopes:\n        mcp:connect: Connect an MCP client to Convika\n        offline_access: Refresh tokens\n  pkce: S256\n  dynamic_client_registration: https://mcp.convika.com/register\n  revocation_endpoint: https://mcp.convika.com/revoke\n\
  \  jwks_uri: https://mcp.convika.com/jwks\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  bearer_methods: [header]\n  evidence: https://mcp.convika.com/.well-known/oauth-authorization-server\napi_keys: none (stated in docs)\n"
source_yaml_url: https://artifacts.apis.io/convika-com/authentication/convika-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Web Hosting
- HTML Publishing
- Landing Pages
- MCP
- Artificial Intelligence
- Forms
- Analytics
---
