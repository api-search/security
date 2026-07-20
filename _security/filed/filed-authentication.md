---
api_key_in: []
auth_types: []
description: 'Filed GraphQL API authentication profile. A two-step token model: a long-lived, workspace-scoped API key created in the Filed web app is exchanged at request time for a short-lived (~30 min) access token sent as a Bearer credential. MCP clients use OAuth instead of an API key.'
kind: authentication
layout: security
method: searched
name: Filed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filed declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Filed
provider_slug: filed
scheme_count: 3
schemes:
- description: Short-lived access token (~30 minutes) minted by exchanging an API key. workspaceToken is used for workspace-scoped calls; userToken is account-wide. Sent on every operation except @public ones (health, the token exchange).
  format: JWT (workspaceToken or userToken)
  id: bearer_access_token
  location: Authorization header
  scheme: bearer
  type: http
- access_levels:
  - description: Queries only; all mutations rejected.
    value: read_only
  - description: Queries plus mutations (upload documents, trigger runs, modify data).
    value: read_write
  default_expiry_days: 90
  description: Long-lived credential created per workspace in the Filed web app under Plugins -> Filed API. Shown once; store in a secret manager. Exchanged via exchangeSurfaceRefreshTokenForAccessTokens (passed as refreshToken). Personal — authenticates as the creating user, scoped to one workspace.
  expiry_options_days:
  - 30
  - 60
  - 90
  - 365
  id: api_key
  type: apiKey
- description: MCP clients connect to https://mcp.apps.filed.com/mcp with OAuth, no API key. The client performs DCR and redirects the user to sign in and approve the connection for one workspace. See mcp/filed-mcp.yml.
  flow: Dynamic Client Registration (RFC 7591) + browser consent
  id: mcp_oauth
  type: oauth2
slug: filed-authentication
source_filename: filed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://docs.apps.filed.com/guides/authentication and\n  https://docs.apps.filed.com/guides/connect-mcp\ndescription: >-\n  Filed GraphQL API authentication profile. A two-step token model: a long-lived,\n  workspace-scoped API key created in the Filed web app is exchanged at request\n  time for a short-lived (~30 min) access token sent as a Bearer credential.\n  MCP clients use OAuth instead of an API key.\nendpoint: https://router.apps.filed.com/graphql\nschemes:\n  - id: bearer_access_token\n    type: http\n    scheme: bearer\n    format: JWT (workspaceToken or userToken)\n    location: Authorization header\n    description: >-\n      Short-lived access token (~30 minutes) minted by exchanging an API key.\n      workspaceToken is used for workspace-scoped calls; userToken is account-wide.\n      Sent on every operation except @public ones (health, the token exchange).\n  - id: api_key\n    type: apiKey\n    description:\
  \ >-\n      Long-lived credential created per workspace in the Filed web app under\n      Plugins -> Filed API. Shown once; store in a secret manager. Exchanged via\n      exchangeSurfaceRefreshTokenForAccessTokens (passed as refreshToken).\n      Personal — authenticates as the creating user, scoped to one workspace.\n    expiry_options_days: [30, 60, 90, 365]\n    default_expiry_days: 90\n    access_levels:\n      - value: read_only\n        description: Queries only; all mutations rejected.\n      - value: read_write\n        description: Queries plus mutations (upload documents, trigger runs, modify data).\n  - id: mcp_oauth\n    type: oauth2\n    flow: Dynamic Client Registration (RFC 7591) + browser consent\n    description: >-\n      MCP clients connect to https://mcp.apps.filed.com/mcp with OAuth, no API key.\n      The client performs DCR and redirects the user to sign in and approve the\n      connection for one workspace. See mcp/filed-mcp.yml.\ntoken_exchange:\n  mutation:\
  \ exchangeSurfaceRefreshTokenForAccessTokens\n  public: true\n  input: refreshToken (the API key)\n  returns: [userToken, workspaceToken]\n  token_lifetime: ~30 minutes; re-exchange the same API key on expiry/401\ndefault_security: bearer_access_token (workspaceToken)\nnotes:\n  - New API keys are deliberately workspace-scoped (unlike legacy partner keys that spanned all partner workspaces).\n  - Verify a token with the `me` query (resolves to WorkspaceUser for a workspaceToken).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filed/refs/heads/main/authentication/filed-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Tax
- Accounting
- Artificial Intelligence
- Document Processing
- GraphQL
- Compliance
- Enterprise
---
