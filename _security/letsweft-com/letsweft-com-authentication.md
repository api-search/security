---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Weft API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Weft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weft declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Weft
provider_slug: letsweft-com
scheme_count: 2
schemes:
- authorize_url: https://letsweft.com/api/auth/oauth2/authorize
  evidence: Weft exposes a single MCP endpoint, https://letsweft.com/api/mcp , protected by OAuth 2.1 with Dynamic Client Registration.
  flows:
  - authorization_code
  - client_credentials
  - refresh_token
  how_to_obtain: Client registers itself via Dynamic Client Registration, then signs in once in a browser to receive an access token.
  name: OAuth 2.1
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
- evidence: 'It goes in the Authorization header, next to the endpoint: Authorization: Bearer wft_… .'
  header: Authorization
  how_to_obtain: Mint an access token in the Settings → Access tokens page; the token is shown once and must be copied into the Authorization header.
  location: header
  name: Access token
  type: http-bearer
slug: letsweft-com-authentication
source_filename: letsweft-com-authentication.yml
source_heading: Authentication Profile
source_url: https://letsweft.com/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://letsweft.com/.well-known/oauth-protected-resource\nsources:\n- https://letsweft.com/.well-known/oauth-protected-resource\n- https://letsweft.com/.well-known/oauth-authorization-server\n- https://letsweft.com/docs/access-tokens\n- https://letsweft.com/docs/quickstart\ndescription: Authentication methods for Weft API\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Weft exposes a single MCP endpoint, https://letsweft.com/api/mcp , protected by OAuth 2.1 with Dynamic Client Registration.\n  flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  authorize_url: https://letsweft.com/api/auth/oauth2/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  how_to_obtain: Client registers itself via Dynamic Client Registration, then signs in once in a browser to receive an access token.\n- type: http-bearer\n  name: Access token\n\
  \  evidence: 'It goes in the Authorization header, next to the endpoint: Authorization: Bearer wft_… .'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint an access token in the Settings → Access tokens page; the token is shown once and must be copied into the Authorization\n    header.\ndocs: https://letsweft.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/letsweft-com/authentication/letsweft-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Task Management
- Productivity
- Solo Founders
- Small Teams
---
