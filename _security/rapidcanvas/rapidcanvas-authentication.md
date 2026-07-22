---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rapidcanvas Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RapidCanvas secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RapidCanvas
provider_slug: rapidcanvas
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://app.rapidcanvas.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://app.rapidcanvas.ai/oauth/register
    scopes:
    - mcp
    - openid
    - profile
    - email
    tokenUrl: https://app.rapidcanvas.ai/oauth/token
  name: OAuth2
  source: well-known/rapidcanvas-oauth-authorization-server.json
  type: oauth2
- description: Platform REST API calls to https://app.rapidcanvas.ai/api/ carry a bearer token. The RC CLI obtains it via `rc login` (browser SSO or --token) and stores it per host x workspace in ~/.rc/credentials.
  name: bearerAuth
  scheme: bearer
  source: https://docs.rapidcanvas.ai/advanced/rc-cli/03-authentication.md
  type: http
slug: rapidcanvas-authentication
source_filename: rapidcanvas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.rapidcanvas.ai/.well-known/oauth-authorization-server\ndocs: https://docs.rapidcanvas.ai/advanced/rc-cli/03-authentication.md\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  api_base: https://app.rapidcanvas.ai/api/\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.rapidcanvas.ai/oauth/authorize\n        tokenUrl: https://app.rapidcanvas.ai/oauth/token\n        registrationUrl: https://app.rapidcanvas.ai/oauth/register\n        pkce: S256\n        scopes: [mcp, openid, profile, email]\n    source: well-known/rapidcanvas-oauth-authorization-server.json\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Platform REST API calls to https://app.rapidcanvas.ai/api/ carry a bearer\n      token. The RC CLI obtains it via `rc login` (browser\
  \ SSO or --token) and\n      stores it per host x workspace in ~/.rc/credentials.\n    source: https://docs.rapidcanvas.ai/advanced/rc-cli/03-authentication.md\nnotes: >-\n  End-user access to the platform is via email/password or SSO sign-in at\n  app.rapidcanvas.ai (sign-up is invitation-based). Programmatic access uses a\n  bearer token scoped to a workspace (tenant). The RFC 8414 metadata advertises\n  authorization_code + refresh_token grants with PKCE for the MCP/OAuth surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidcanvas/refs/heads/main/authentication/rapidcanvas-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Agentic AI
- Data Science
- MLOps
- Enterprise AI
- AI Governance
- Low Code
- Developer Tools
---
