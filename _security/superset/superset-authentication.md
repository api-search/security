---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Superset Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Superset secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Superset
provider_slug: superset
scheme_count: 3
schemes:
- authorizationUrl: https://api.superset.sh/api/auth/oauth2/authorize
  description: OAuth 2.1 with dynamic client registration; supports authorization_code, client_credentials, refresh_token.
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  issuer: https://api.superset.sh
  name: OAuth2.1
  registrationUrl: https://api.superset.sh/api/auth/oauth2/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - https://docs.superset.sh/mcp
  - https://api.superset.sh/.well-known/oauth-authorization-server
  tokenUrl: https://api.superset.sh/api/auth/oauth2/token
  type: oauth2
- description: OIDC discovery published at api.superset.sh.
  name: OpenIDConnect
  openIdConnectUrl: https://api.superset.sh/.well-known/openid-configuration
  sources:
  - https://api.superset.sh/.well-known/openid-configuration
  type: openIdConnect
- description: Live API keys for headless/CI environments.
  in: header
  key_prefix: sk_live_
  name: ApiKey
  sources:
  - https://docs.superset.sh/mcp
  type: apiKey
slug: superset-authentication
source_filename: superset-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.superset.sh/mcp\ndocs: https://docs.superset.sh/cli/cli-reference\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  notes: >-\n    Superset's hosted Agent API (api.superset.sh) authenticates with OAuth 2.1\n    (browser-based authorization code, used for interactive/CLI cross-device\n    login) or API keys for headless/CI use. The CLI signs in via\n    `superset auth login` (OAuth or API key) and stores credentials locally.\n    api.superset.sh publishes RFC 8414 authorization-server metadata and OIDC\n    discovery (see well-known/superset-well-known.yml).\nschemes:\n  - name: OAuth2.1\n    type: oauth2\n    flows: [authorizationCode, clientCredentials, refreshToken]\n    issuer: https://api.superset.sh\n    authorizationUrl: https://api.superset.sh/api/auth/oauth2/authorize\n    tokenUrl: https://api.superset.sh/api/auth/oauth2/token\n\
  \    registrationUrl: https://api.superset.sh/api/auth/oauth2/register\n    description: OAuth 2.1 with dynamic client registration; supports authorization_code, client_credentials, refresh_token.\n    scopes: [openid, profile, email, offline_access]\n    sources: [https://docs.superset.sh/mcp, https://api.superset.sh/.well-known/oauth-authorization-server]\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://api.superset.sh/.well-known/openid-configuration\n    description: OIDC discovery published at api.superset.sh.\n    sources: [https://api.superset.sh/.well-known/openid-configuration]\n  - name: ApiKey\n    type: apiKey\n    in: header\n    key_prefix: sk_live_\n    description: Live API keys for headless/CI environments.\n    sources: [https://docs.superset.sh/mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superset/refs/heads/main/authentication/superset-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Developer Tools
- AI Agents
- Code Editor
- IDE
- Coding Agents
- MCP
- CLI
- SDK
- Git Worktrees
- Automation
- Y Combinator
---
