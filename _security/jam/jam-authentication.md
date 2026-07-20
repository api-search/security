---
api_key_in:
- header
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Jam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jam secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jam
provider_slug: jam
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://api.jam.dev/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    introspectionUrl: https://api.jam.dev/oauth/introspect
    pkce: S256
    refreshUrl: https://api.jam.dev/oauth/token
    registrationUrl: https://api.jam.dev/oauth/register
    revocationUrl: https://api.jam.dev/oauth/revoke
    scopes:
    - mcp:read
    - mcp:write
    tokenUrl: https://api.jam.dev/oauth/token
  name: OAuth2
  sources:
  - https://mcp.jam.dev/.well-known/oauth-authorization-server
  type: oauth2
  used_by: MCP server (browser OAuth), CLI (jam auth login)
- bearerFormat: jam_pat_<random>
  description: 'Personal Access Tokens for headless MCP clients and CI. Workspace-scoped, user-tied, mandatory expiration (7/30/90 days or 1 year), scope-selectable, stored server-side only as a hash. Used as an Authorization: Bearer header.'
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - https://jam.dev/docs/personal-access-tokens
  type: http
slug: jam-authentication
source_filename: jam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://jam.dev/docs/jam-mcp, https://jam.dev/docs/personal-access-tokens, https://mcp.jam.dev/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.jam.dev/oauth/authorize\n        tokenUrl: https://api.jam.dev/oauth/token\n        refreshUrl: https://api.jam.dev/oauth/token\n        registrationUrl: https://api.jam.dev/oauth/register\n        introspectionUrl: https://api.jam.dev/oauth/introspect\n        revocationUrl: https://api.jam.dev/oauth/revoke\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\n        scopes: [mcp:read, mcp:write]\n    sources: [https://mcp.jam.dev/.well-known/oauth-authorization-server]\n    used_by: MCP server (browser OAuth), CLI (jam auth login)\n  - name: PersonalAccessToken\n\
  \    type: http\n    scheme: bearer\n    bearerFormat: jam_pat_<random>\n    description: >-\n      Personal Access Tokens for headless MCP clients and CI. Workspace-scoped,\n      user-tied, mandatory expiration (7/30/90 days or 1 year), scope-selectable,\n      stored server-side only as a hash. Used as an Authorization: Bearer header.\n    sources: [https://jam.dev/docs/personal-access-tokens]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jam/refs/heads/main/authentication/jam-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Developer Tools
- Bug Reporting
- Debugging
- Quality Assurance
- Observability
- Screen Recording
- Model Context Protocol
---
