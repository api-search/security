---
api_key_in: []
api_specs:
- filename: flint-agent-tasks-openapi.yml
  format: yaml
  label: Flint Agent Tasks API
  slug: flint-agent-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flint/refs/heads/main/openapi/flint-agent-tasks-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Flint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Flint secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Flint
provider_slug: flint
scheme_count: 2
schemes:
- format: Bearer [example key]
  header: Authorization
  name: bearerApiKey
  provisioning: API keys are created in Flint team settings and require at least member role permissions.
  scheme: bearer
  sources:
  - openapi/flint-agent-tasks-openapi.yml
  - https://www.flint.com/docs/api
  surface: rest-api
  type: http
- authorization_endpoint: https://clerk.tryflint.com/oauth/authorize
  authorization_server: https://clerk.tryflint.com
  dynamic_client_registration: true
  flows:
  - authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: mcpOAuth
  pkce: S256
  registration_endpoint: https://clerk.tryflint.com/oauth/register
  sources:
  - https://mcp.tryflint.com/.well-known/oauth-protected-resource
  - https://clerk.tryflint.com/.well-known/oauth-authorization-server
  surface: mcp
  token_endpoint: https://clerk.tryflint.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: flint-authentication
source_filename: flint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.flint.com/docs/api\ndocs: https://www.flint.com/docs/api\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  api_key_prefix: \"ak_\"\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The REST Agent Tasks API uses a bearer API key. The hosted MCP server uses\n    OAuth 2.0 (authorization code + PKCE) via Clerk as the authorization server.\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    surface: rest-api\n    header: Authorization\n    format: \"Bearer [example key]\"\n    provisioning: >-\n      API keys are created in Flint team settings and require at least member\n      role permissions.\n    sources: [openapi/flint-agent-tasks-openapi.yml, https://www.flint.com/docs/api]\n  - name: mcpOAuth\n    type: oauth2\n    surface: mcp\n    authorization_server: https://clerk.tryflint.com\n    authorization_endpoint: https://clerk.tryflint.com/oauth/authorize\n    token_endpoint:\
  \ https://clerk.tryflint.com/oauth/token\n    registration_endpoint: https://clerk.tryflint.com/oauth/register\n    flows: [authorizationCode]\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    dynamic_client_registration: true\n    sources:\n      - https://mcp.tryflint.com/.well-known/oauth-protected-resource\n      - https://clerk.tryflint.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flint/refs/heads/main/authentication/flint-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- AI
- Marketing
- Landing Pages
- Agents
- MCP
- Web
- Advertising
---
