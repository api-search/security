---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: cowork24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: cowork24 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: cowork24
provider_slug: cowork24-ch
scheme_count: 1
schemes:
- applies_to: https://mcp.cowork24.ch/mcp
  dynamic_client_registration: https://mcp.cowork24.ch/register
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.cowork24.ch/authorize
      refreshUrl: https://mcp.cowork24.ch/token
      scopes:
        cowork24: Sole scope advertised in scopes_supported (no description published)
      tokenUrl: https://mcp.cowork24.ch/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.cowork24.ch/
  name: cowork24 MCP OAuth
  pkce:
    code_challenge_methods_supported:
    - S256
  response_types_supported:
  - code
  revocation_endpoint: https://mcp.cowork24.ch/revoke
  revocation_endpoint_auth_methods_supported:
  - client_secret_post
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: oauth2
slug: cowork24-ch-authentication
source_filename: cowork24-ch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.cowork24.ch/.well-known/oauth-authorization-server\ndocs: null\nsummary:\n  types:\n  - oauth2\n  note: >-\n    cowork24 publishes no OpenAPI and no developer documentation. The only authentication surface is the\n    remote MCP server (https://mcp.cowork24.ch/mcp), whose OAuth 2.0 authorization-server metadata\n    (RFC 8414) was fetched with GET (HTTP 200). /.well-known/oauth-protected-resource on the same host\n    returned HTTP 404. Endpoints are recorded as advertised; none was called.\nschemes:\n- name: cowork24 MCP OAuth\n  type: oauth2\n  issuer: https://mcp.cowork24.ch/\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.cowork24.ch/authorize\n      tokenUrl: https://mcp.cowork24.ch/token\n      refreshUrl: https://mcp.cowork24.ch/token\n      scopes:\n        cowork24: Sole scope advertised in scopes_supported (no description published)\n  grant_types_supported: [authorization_code, refresh_token]\n\
  \  response_types_supported: [code]\n  pkce: {code_challenge_methods_supported: [S256]}\n  token_endpoint_auth_methods_supported: [client_secret_post, none]\n  revocation_endpoint: https://mcp.cowork24.ch/revoke\n  revocation_endpoint_auth_methods_supported: [client_secret_post]\n  dynamic_client_registration: https://mcp.cowork24.ch/register\n  applies_to: https://mcp.cowork24.ch/mcp\n"
source_yaml_url: https://artifacts.apis.io/cowork24-ch/authentication/cowork24-ch-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Co-Working
- Workspace Booking
- Meeting Rooms
- Marketplace
- Switzerland
- MCP
---
