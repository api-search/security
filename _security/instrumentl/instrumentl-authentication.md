---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Instrumentl Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instrumentl secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instrumentl
provider_slug: instrumentl
scheme_count: 2
schemes:
- dynamic_client_registration: https://www.instrumentl.com/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://www.instrumentl.com/oauth/authorize
      refreshUrl: https://www.instrumentl.com/oauth/token
      scopes:
        mcp:read: Read access via the MCP server
        mcp:write: Write access via the MCP server
      tokenUrl: https://www.instrumentl.com/oauth/token
  name: OAuth2
  pkce: S256
  sources:
  - https://www.instrumentl.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- description: The remote MCP server also accepts a valid API key as a bearer token (unauthenticated calls return "You must authenticate with a valid API key to proceed"). Bearer credentials are sent in the Authorization header.
  in: header
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - https://mcp.instrumentl.com
  type: http
slug: instrumentl-authentication
source_filename: instrumentl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.instrumentl.com/.well-known/oauth-authorization-server\ndocs: https://mcp.instrumentl.com/.well-known/oauth-protected-resource\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://www.instrumentl.com/oauth/authorize\n        tokenUrl: https://www.instrumentl.com/oauth/token\n        refreshUrl: https://www.instrumentl.com/oauth/token\n        scopes:\n          mcp:read: Read access via the MCP server\n          mcp:write: Write access via the MCP server\n    pkce: S256\n    token_endpoint_auth_methods_supported: [none]      # public client (PKCE)\n    dynamic_client_registration: https://www.instrumentl.com/oauth/register\n    sources: [https://www.instrumentl.com/.well-known/oauth-authorization-server]\n  - name: ApiKeyAuth\n    type: http\n    scheme:\
  \ bearer\n    description: >-\n      The remote MCP server also accepts a valid API key as a bearer token\n      (unauthenticated calls return \"You must authenticate with a valid API key\n      to proceed\"). Bearer credentials are sent in the Authorization header.\n    in: header\n    sources: [https://mcp.instrumentl.com]\nnotes: >-\n  Derived by search of Instrumentl's OAuth discovery documents (no OpenAPI is\n  published). Access to the MCP server is gated by OAuth 2.0 authorization-code\n  + PKCE with dynamic client registration and refresh tokens, or a bearer API\n  key. Security contact: security@instrumentl.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instrumentl/refs/heads/main/authentication/instrumentl-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Grants
- Nonprofit
- Fundraising
- Grant Management
- Foundation Data
- Philanthropy
- MCP
---
