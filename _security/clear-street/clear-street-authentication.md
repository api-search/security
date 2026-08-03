---
api_key_in:
- header
api_specs:
- filename: clear-street-trading-api-openapi.yml
  format: yaml
  label: Clear Street Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-trading-api-openapi.yml
- filename: clear-street-studio-openapi.yml
  format: yaml
  label: Clear Street Studio API
  slug: studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-studio-openapi.yml
- filename: clear-street-legacy-api-swagger.yml
  format: yaml
  label: Clear Street API (Trades and Uploads)
  slug: legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-legacy-api-swagger.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Clear Street Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Clear Street secures its APIs with http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Clear Street
provider_slug: clear-street
scheme_count: 5
schemes:
- applied: 'global — security: [{BearerAuth: []}] at the document root'
  bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/clear-street-studio-openapi.yml
  - openapi/clear-street-trading-api-openapi.yml
  type: http
- api: Clear Street Trading API
  docs: https://docs.clearstreet.com/guides/api-fundamentals/
  exchange_note: Used as a raw bearer token — no OAuth exchange.
  exchange_required: false
  header: 'Authorization: Bearer <CLEARSTREET_API_KEY>'
  issuance: Created by the account holder in the API Keys section of the Clear Street app.
  key_shape: <id>.<secret>
  name: Trading API key
  scheme: bearer
  source: https://github.com/clear-street/clearstreet-skills
  type: http
- api: Clear Street Studio API
  docs: https://docs.clearstreet.io/studio/docs/oauth2
  flows:
  - audience: https://api.clearstreet.io
    flow: clientCredentials
    scopes:
    - studio
    tokenUrl: https://auth.clearstreet.io/oauth/token
  issuance: Studio > Settings > Developer > Create OAuth2 API Credentials
  issuer: https://auth.clearstreet.io/
  name: Studio OAuth2
  per_application_credentials: true
  provider: Auth0
  token_lifetime: 24h
  type: oauth2
- api: Clear Street MCP Server
  authorization_server: https://api.clearstreet.com/oauth/mcp
  discovery: well-known/clear-street-mcp-oauth-protected-resource.json
  flows:
  - authorizationUrl: https://api.clearstreet.com/oauth/mcp/authorize
    flow: authorizationCode
    pkce:
    - S256
    scopes:
    - openid
    - offline_access
    tokenUrl: https://auth.clearstreet.io/oauth/token
  name: MCP OAuth
  resource: https://api.clearstreet.com/v1/mcp
  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata
  type: oauth2
- api: Clear Street application login
  discovery: well-known/clear-street-openid-configuration.json
  dpop_supported: true
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - device_code
  - token-exchange
  - implicit
  - password
  issuer: https://auth.clearstreet.io/
  name: Auth0 OIDC
  openIdConnectUrl: https://auth.clearstreet.io/.well-known/openid-configuration
  type: openIdConnect
slug: clear-street-authentication
source_filename: clear-street-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/clear-street-studio-openapi.yml, openapi/clear-street-trading-api-openapi.yml\ndocs:\n- https://docs.clearstreet.com/guides/api-fundamentals/\n- https://docs.clearstreet.io/studio/docs/oauth2\nnote: >\n  Upgraded from the mechanical derive. Both OpenAPI documents declare a single `BearerAuth`\n  (http/bearer/JWT) scheme, which understates the real model: the two APIs mint that bearer\n  token in completely different ways, and a third surface (the MCP server) is protected by a\n  separate OAuth authorization server discovered via RFC 9728.\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  transport: TLS 1.3 on every probed host\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: 'global — security: [{BearerAuth: []}] at the document root'\n  sources:\n  - openapi/clear-street-studio-openapi.yml\n\
  \  - openapi/clear-street-trading-api-openapi.yml\n- name: Trading API key\n  api: Clear Street Trading API\n  type: http\n  scheme: bearer\n  key_shape: '<id>.<secret>'\n  header: 'Authorization: Bearer <CLEARSTREET_API_KEY>'\n  issuance: Created by the account holder in the API Keys section of the Clear Street app.\n  exchange_required: false\n  exchange_note: 'Used as a raw bearer token — no OAuth exchange.'\n  docs: https://docs.clearstreet.com/guides/api-fundamentals/\n  source: https://github.com/clear-street/clearstreet-skills\n- name: Studio OAuth2\n  api: Clear Street Studio API\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.clearstreet.io/oauth/token\n    audience: https://api.clearstreet.io\n    scopes: [studio]\n  issuer: https://auth.clearstreet.io/\n  provider: Auth0\n  token_lifetime: 24h\n  issuance: Studio > Settings > Developer > Create OAuth2 API Credentials\n  per_application_credentials: true\n  docs: https://docs.clearstreet.io/studio/docs/oauth2\n\
  - name: MCP OAuth\n  api: Clear Street MCP Server\n  type: oauth2\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  resource: https://api.clearstreet.com/v1/mcp\n  authorization_server: https://api.clearstreet.com/oauth/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.clearstreet.com/oauth/mcp/authorize\n    tokenUrl: https://auth.clearstreet.io/oauth/token\n    pkce: [S256]\n    scopes: [openid, offline_access]\n  discovery: well-known/clear-street-mcp-oauth-protected-resource.json\n- name: Auth0 OIDC\n  api: Clear Street application login\n  type: openIdConnect\n  openIdConnectUrl: https://auth.clearstreet.io/.well-known/openid-configuration\n  issuer: https://auth.clearstreet.io/\n  grant_types: [authorization_code, client_credentials, refresh_token, device_code,\n    token-exchange, implicit, password]\n  dpop_supported: true\n  discovery: well-known/clear-street-openid-configuration.json\nwebsocket:\n  scheme: oauth2 access token in the subscribe\
  \ message `authorization` field\n  note: See asyncapi/clear-street-studio-events.yml.\nmutual_tls: false\ngaps:\n- The specifications do not model the OAuth2 flows at all — only the resulting bearer token —\n  so tooling generated straight from the spec cannot obtain a Studio credential.\n- No per-resource scopes; see scopes/clear-street-scopes.yml#granularity.\nx-evidence:\n  fetched: '2026-08-02'\n  sources:\n  - {url: 'https://docs.clearstreet.io/studio/docs/oauth2', http_status: 200}\n  - {url: 'https://docs.clearstreet.com/guides/api-fundamentals/index.md', http_status: 200}\n  - {url: 'https://auth.clearstreet.io/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://api.clearstreet.com/v1/mcp', http_status: 401, note: 'RFC 9728 WWW-Authenticate challenge'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/authentication/clear-street-authentication.yml
summary_line: http/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Financial Services
- Capital Markets
- Prime Brokerage
- Trading
- Brokerage
- Clearing
- Market Data
- Fintech
- Investing
---
