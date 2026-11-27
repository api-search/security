---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ClosedMCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClosedMCP declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ClosedMCP
provider_slug: closedmcp-com
scheme_count: 3
schemes:
- client_registration: dynamic (POST /oauth/register; token_endpoint_auth_method none)
  discovery:
  - https://closedmcp.com/.well-known/oauth-protected-resource
  - https://closedmcp.com/.well-known/oauth-authorization-server
  - https://closedmcp.com/.well-known/openid-configuration
  docs: https://closedmcp.com/docs/api?task=signin
  flows:
    authorizationCode:
      authorizationUrl: https://closedmcp.com/oauth/authorize
      refreshUrl: https://closedmcp.com/oauth/token
      scopes:
        mcp:list: List tools
        mcp:tools: Call tools
      tokenUrl: https://closedmcp.com/oauth/token
  name: closedmcpOAuth
  pkce: S256 required
  token_lifetime: expires_in 2592000 in the documented example
  token_prefixes:
    access_token: cmcp_at_ (example value cmcp_at_example)
    refresh_token: cmcp_rt_ (example value cmcp_rt_example)
  type: oauth2
- description: 'Authorization: Bearer <access_token> on POST /mcp and GET /mcp.'
  docs: https://closedmcp.com/docs/api
  in: header
  name: bearerAccessToken
  scheme: bearer
  type: http
- description: 'A tool identity token is a JWT signed with Ed25519 (alg: EdDSA); aud must match your MCP server URL; expires in 5 minutes at most; claims iss, aud, sub, email, domain, org, client, iat, exp, jti.'
  docs: https://closedmcp.com/docs/api?task=identity
  jwks_uri: https://closedmcp.com/.well-known/jwks.json
  name: toolIdentityToken
  type: jwt
slug: closedmcp-com-authentication
source_filename: closedmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://closedmcp.com/docs/api?task=signin\n- https://closedmcp.com/docs/api\n- https://closedmcp.com/docs/api?task=identity\ndocs: https://closedmcp.com/docs/api\nsummary: 'OAuth 2.0 authorization code with PKCE (S256) for public clients (no client secret), dynamic client registration\n  at POST /oauth/register, and Google sign-in in the browser. Access tokens are sent as Authorization: Bearer on /mcp. Connected\n  MCP servers receive a separate short-lived Ed25519-signed tool identity JWT verified against /.well-known/jwks.json. No\n  OpenAPI is published; profile read from the API reference.'\nschemes:\n- name: closedmcpOAuth\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://closedmcp.com/oauth/authorize\n      tokenUrl: https://closedmcp.com/oauth/token\n      refreshUrl: https://closedmcp.com/oauth/token\n      scopes:\n        mcp:tools: Call tools\n        mcp:list: List tools\n  pkce:\
  \ S256 required\n  client_registration: dynamic (POST /oauth/register; token_endpoint_auth_method none)\n  discovery:\n  - https://closedmcp.com/.well-known/oauth-protected-resource\n  - https://closedmcp.com/.well-known/oauth-authorization-server\n  - https://closedmcp.com/.well-known/openid-configuration\n  token_lifetime: expires_in 2592000 in the documented example\n  token_prefixes:\n    access_token: cmcp_at_ (example value cmcp_at_example)\n    refresh_token: cmcp_rt_ (example value cmcp_rt_example)\n  docs: https://closedmcp.com/docs/api?task=signin\n- name: bearerAccessToken\n  type: http\n  scheme: bearer\n  in: header\n  description: 'Authorization: Bearer <access_token> on POST /mcp and GET /mcp.'\n  docs: https://closedmcp.com/docs/api\n- name: toolIdentityToken\n  type: jwt\n  description: 'A tool identity token is a JWT signed with Ed25519 (alg: EdDSA); aud must match your MCP server URL; expires\n    in 5 minutes at most; claims iss, aud, sub, email, domain, org, client,\
  \ iat, exp, jti.'\n  jwks_uri: https://closedmcp.com/.well-known/jwks.json\n  docs: https://closedmcp.com/docs/api?task=identity\n"
source_yaml_url: https://artifacts.apis.io/closedmcp-com/authentication/closedmcp-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- MCP
- AI Agents
- Gateways
- Access Control
- Serverless
- Developer Tools
---
