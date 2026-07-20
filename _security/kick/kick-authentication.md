---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kick Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kick secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kick
provider_slug: kick
scheme_count: 2
schemes:
- access_token_lifetime_seconds: 3600
  authorizationUrl: https://use.kick.co/mcp/oauth/authorize
  dynamic_client_registration: true
  flow: authorizationCode
  name: OAuth2
  pkce: S256
  registrationUrl: https://use.kick.co/mcp/oauth/register
  revocationUrl: https://use.kick.co/mcp/oauth/revoke
  scopes:
  - mcp:read
  - mcp:write
  sources:
  - https://use.kick.co/.well-known/oauth-authorization-server
  tokenUrl: https://use.kick.co/mcp/oauth/token
  type: oauth2
- header: 'Authorization: Bearer [example key]'
  name: PersonalAccessToken
  notes: Prefer read-only PATs; bind to the narrowest workspace; use short expirations for CI/scripts/agents; revoke when no longer needed.
  scheme: bearer
  sources:
  - https://docs.kick.co/ai/permissions-and-security.md
  token_prefix: kick_pat_
  type: http
  used_by:
  - cli
  - mcp
slug: kick-authentication
source_filename: kick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kick.co/ai/permissions-and-security.md\ndocs: https://docs.kick.co/ai/developer-tools/mcp/mcp-reference.md\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Programmatic access (MCP server + CLI) authenticates with either OAuth 2.1 or a\n    Personal Access Token bearer credential. There is no public OpenAPI, so schemes\n    are captured from the OAuth well-known metadata and the published auth docs.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://use.kick.co/mcp/oauth/authorize\n  tokenUrl: https://use.kick.co/mcp/oauth/token\n  registrationUrl: https://use.kick.co/mcp/oauth/register\n  revocationUrl: https://use.kick.co/mcp/oauth/revoke\n  pkce: S256\n  dynamic_client_registration: true\n  scopes: [mcp:read, mcp:write]\n  access_token_lifetime_seconds: 3600\n  sources: [https://use.kick.co/.well-known/oauth-authorization-server]\n\
  - name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  token_prefix: kick_pat_\n  header: \"Authorization: Bearer [example key]\"\n  used_by: [cli, mcp]\n  notes: >-\n    Prefer read-only PATs; bind to the narrowest workspace; use short expirations\n    for CI/scripts/agents; revoke when no longer needed.\n  sources: [https://docs.kick.co/ai/permissions-and-security.md]\nauthorization_model: >-\n  MCP and CLI requests go through Kick's normal backend authorization path — token\n  scope, workspace scope, route policy, and controller-level permission checks —\n  before any read or write. Tool annotations shown to clients are hints, not the\n  source of authorization; the server decides what a credential can do.\nexternal:\n- provider: Plaid\n  purpose: Bank/financial-institution connection; Kick never sees or stores end-user bank login credentials.\n  source: https://docs.kick.co/reference/security.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kick/refs/heads/main/authentication/kick-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Bookkeeping
- Accounting
- Finance
- FinTech
- MCP
- AI Agents
- Small Business
---
