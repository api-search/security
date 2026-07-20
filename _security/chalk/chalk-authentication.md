---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Chalk Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Chalk secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Chalk
provider_slug: chalk
scheme_count: 3
schemes:
- description: 'Primary programmatic auth. Exchange client_id + client_secret (grant_type=client_credentials) for a short-lived Bearer access_token, then send Authorization: Bearer <token>. Credentials are minted in the dashboard (Personal = full account access; Service = scoped to a project + environment). `chalk token` returns a ready-to-use access token.'
  flow: clientCredentials
  name: OAuth2ClientCredentials
  token_auth_methods:
  - client_secret_post
  - client_secret_basic
  token_url: https://api.chalk.ai/v1/oauth/token
  type: oauth2
- authorization_url: https://api.chalk.ai/v1/oauth/authorize
  description: Authorization-code + PKCE flow with dynamic client registration, advertised in the RFC 8414 oauth-authorization-server metadata with mcp:read/mcp:write scopes for MCP clients.
  flow: authorizationCode
  name: OAuth2AuthorizationCode
  pkce: S256
  scopes:
  - mcp:read
  - mcp:write
  token_url: https://api.chalk.ai/v1/oauth/token
  type: oauth2
- bearer_format: JWT
  description: RS256-signed JWT access tokens (claims include team_id, environment_id, project_id, kind).
  name: BearerToken
  scheme: bearer
  type: http
slug: chalk-authentication
source_filename: chalk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chalk.ai/docs/online-authentication\ndocs: https://docs.chalk.ai/docs/online-authentication\ndiscovery: https://api.chalk.ai/.well-known/openid-configuration\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  token_endpoint: https://api.chalk.ai/v1/oauth/token\n  authorization_endpoint: https://api.chalk.ai/v1/oauth/authorize\n  registration_endpoint: https://api.chalk.ai/v1/oauth/register\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.chalk.ai/v1/oauth/token\n  token_auth_methods: [client_secret_post, client_secret_basic]\n  description: >-\n    Primary programmatic auth. Exchange client_id + client_secret (grant_type=client_credentials)\n    for a short-lived Bearer access_token, then send Authorization: Bearer <token>.\n    Credentials are minted in the dashboard (Personal = full\
  \ account access; Service =\n    scoped to a project + environment). `chalk token` returns a ready-to-use access token.\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://api.chalk.ai/v1/oauth/authorize\n  token_url: https://api.chalk.ai/v1/oauth/token\n  pkce: S256\n  scopes: [mcp:read, mcp:write]\n  description: >-\n    Authorization-code + PKCE flow with dynamic client registration, advertised in the\n    RFC 8414 oauth-authorization-server metadata with mcp:read/mcp:write scopes for MCP clients.\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: RS256-signed JWT access tokens (claims include team_id, environment_id, project_id, kind).\nrbac:\n  note: >-\n    Service tokens support feature-level RBAC via tags mapped to four levels —\n    Deny, AllowInternal, Allow, AllowDownstream — controlling whether a feature can be\n    computed, returned, or declassified in downstream queries.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chalk/refs/heads/main/authentication/chalk-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Machine Learning
- Feature Store
- Artificial Intelligence
- Data Platform
- MLOps
- Real-Time Data
- LLM
- Agents
- Feature Engineering
---
