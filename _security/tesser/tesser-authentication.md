---
api_key_in: []
api_specs:
- filename: tesser-openapi-original.json
  format: json
  label: Tesser API
  slug: tesser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-openapi-original.json
auth_types:
- oauth2
- http
description: Every request to the Tesser API must carry a JWT access token. Tokens are minted via the OAuth 2.0 client-credentials grant against Tesser's Auth0 tenant. Each workspace has a Client ID + Client Secret pair (Dashboard -> Settings > API Keys). The token is presented as an HTTP bearer token. The OpenAPI declares a single `bearer` (http/bearer, JWT) security scheme applied globally.
kind: authentication
layout: security
method: searched
name: Tesser Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tesser secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tesser
provider_slug: tesser
scheme_count: 1
schemes:
- applied: global
  bearer_format: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/tesser-openapi-original.json
  type: http
slug: tesser-authentication
source_filename: tesser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tesser.xyz/overviews/authentication\ndocs: https://docs.tesser.xyz/overviews/authentication\nsummary:\n  types: [oauth2, http]\n  scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials]\n  identity_provider: Auth0\ndescription: >-\n  Every request to the Tesser API must carry a JWT access token. Tokens are\n  minted via the OAuth 2.0 client-credentials grant against Tesser's Auth0\n  tenant. Each workspace has a Client ID + Client Secret pair (Dashboard ->\n  Settings > API Keys). The token is presented as an HTTP bearer token. The\n  OpenAPI declares a single `bearer` (http/bearer, JWT) security scheme applied\n  globally.\nschemes:\n  - name: bearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applied: global\n    sources: [openapi/tesser-openapi-original.json]\ntoken_endpoints:\n  - environment: production\n    url: https://auth.tesser.xyz/oauth/token\n    audience: https://api.tesser.xyz\n\
  \    grant_type: client_credentials\n    authorization_server: https://tesser-payments.us.auth0.com\n    token_lifetime_seconds: 86400\n  - environment: sandbox\n    audience: https://sandbox.tesserx.co\n    grant_type: client_credentials\n    authorization_server: https://dev-awqy75wdabpsnsvu.us.auth0.com\ntoken_request_body:\n  client_id: YOUR_CLIENT_ID\n  client_secret: YOUR_CLIENT_SECRET\n  audience: https://api.tesser.xyz\n  grant_type: client_credentials\ntoken_response_fields:\n  - {field: access_token, description: JWT to include in the Authorization header}\n  - {field: token_type, description: Always \"Bearer\"}\n  - {field: expires_in, description: Token lifetime in seconds (default 86400 = 24h)}\nusage:\n  header: Authorization\n  format: 'Bearer <access_token>'\ncredentials_location: https://app.tesser.xyz (Settings > API Keys)\nnotes: >-\n  OAuth Protected Resource metadata (RFC 9728) is served at\n  /.well-known/oauth-protected-resource on both api.tesser.xyz and\n  sandbox.tesserx.co,\
  \ advertising the Auth0 authorization server so MCP/OAuth\n  clients can auto-discover the auth flow. No fine-grained OAuth scopes are\n  documented; access is audience-scoped per environment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/authentication/tesser-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Company
- Payments
- Stablecoins
- Cross-Border Payments
- Fintech
- Treasury
- Banking
- Blockchain
- Compliance
- MCP
- Developer Platform
---
