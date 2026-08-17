---
api_key_in:
- header
api_specs:
- filename: equals-memories-openapi.yml
  format: yaml
  label: Equals Memories API
  slug: equals-memories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equals/refs/heads/main/openapi/equals-memories-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Equals Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Equals secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Equals
provider_slug: equals
scheme_count: 2
schemes:
- evidence:
    body: '{"error":"Unauthorized"}'
    checked: '2026-08-14'
    status: 401
    url: https://go.equals.com/api/v1/memories
  header: 'Authorization: Bearer <token>'
  name: bearerAuth
  revocation: Revocable from the same Settings → API tokens page at any time.
  scheme: bearer
  scope_model: Tokens act as the creating user and are scoped to the workspace the token was created in. No granular scopes or permissions are published.
  sources:
  - openapi/equals-memories-openapi.yml
  surface: REST — Memories API
  token_prefix: eq_
  token_source: Settings → API tokens → Create token, inside the Equals app
  token_visibility: shown once at creation
  type: http
- authorization_response_iss_parameter_supported: true
  bearer_methods_supported:
  - header
  dynamic_client_registration: true
  evidence:
    checked: '2026-08-14'
    status: 401
    url: https://go.equals.com/api/mcp
    www_authenticate: Bearer realm="Equals", resource_metadata="https://go.equals.com/.well-known/oauth-protected-resource"
  flows:
  - authorizationUrl: https://go.equals.com/oauth/authorize
    flow: authorizationCode
    note: The authorization-server metadata publishes no scopes_supported; no scope surface is documented.
    pkce:
    - S256
    scopes: {}
    tokenUrl: https://go.equals.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://go.equals.com
  name: mcpOAuth
  protected_resource: https://go.equals.com/api/mcp
  registration_endpoint: https://go.equals.com/oauth/register
  response_types_supported:
  - code
  sources:
  - well-known/equals-oauth-authorization-server.json
  - well-known/equals-oauth-protected-resource.json
  surface: MCP — https://go.equals.com/api/mcp
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: equals-authentication
source_filename: equals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/equals-memories-openapi.yml\ndocs:\n  - https://docs.equals.com/docs/memories-api\n  - https://docs.equals.com/docs/equals-mcp\nnote: >-\n  Equals runs two separate programmatic surfaces with two different auth models: the REST Memories API\n  uses a workspace-scoped bearer API token minted in the product UI, while the hosted MCP server uses a\n  full OAuth 2.1 authorization-code flow with PKCE and dynamic client registration, advertised through\n  RFC 8414 / RFC 9728 discovery documents. Both were probed live.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  api_key_in: [header]\n  anonymous_access: false\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    surface: REST — Memories API\n    sources: [openapi/equals-memories-openapi.yml]\n    token_source: Settings → API tokens → Create token, inside the Equals app\n    token_prefix: eq_\n    token_visibility:\
  \ shown once at creation\n    scope_model: >-\n      Tokens act as the creating user and are scoped to the workspace the token was created in. No\n      granular scopes or permissions are published.\n    revocation: Revocable from the same Settings → API tokens page at any time.\n    header: 'Authorization: Bearer <token>'\n    evidence:\n      url: https://go.equals.com/api/v1/memories\n      status: 401\n      body: '{\"error\":\"Unauthorized\"}'\n      checked: '2026-08-14'\n  - name: mcpOAuth\n    type: oauth2\n    surface: MCP — https://go.equals.com/api/mcp\n    sources: [well-known/equals-oauth-authorization-server.json, well-known/equals-oauth-protected-resource.json]\n    issuer: https://go.equals.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://go.equals.com/oauth/authorize\n        tokenUrl: https://go.equals.com/oauth/token\n        pkce: [S256]\n        scopes: {}\n        note: The authorization-server metadata publishes no scopes_supported;\
  \ no scope surface is documented.\n    registration_endpoint: https://go.equals.com/oauth/register\n    dynamic_client_registration: true\n    grant_types_supported: [authorization_code, refresh_token]\n    token_endpoint_auth_methods_supported: [none]\n    response_types_supported: [code]\n    authorization_response_iss_parameter_supported: true\n    bearer_methods_supported: [header]\n    protected_resource: https://go.equals.com/api/mcp\n    evidence:\n      url: https://go.equals.com/api/mcp\n      status: 401\n      www_authenticate: 'Bearer realm=\"Equals\", resource_metadata=\"https://go.equals.com/.well-known/oauth-protected-resource\"'\n      checked: '2026-08-14'\nsso:\n  enterprise_sso: true\n  providers_named: [Okta, Azure AD]\n  note: End-user SSO on the Enterprise plan only; this is product sign-in, not API authentication.\n  source: https://equals.com/pricing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equals/refs/heads/main/authentication/equals-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Analytics
- Spreadsheets
- Business Intelligence
- Dashboards
- Data
- Revenue Operations
- Reporting
- MCP
---
