---
api_key_in:
- header
api_specs:
- filename: unblocked-public-api-openapi-original.json
  format: json
  label: Unblocked Public API
  slug: unblocked-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unblocked/refs/heads/main/openapi/unblocked-public-api-openapi-original.json
auth_types:
- http-bearer
- oauth2
description: Authentication profile for the Unblocked Public API and tooling surface, captured from the API quickstart, the published OpenAPI securitySchemes, the CLI auth docs, and the OAuth authorization-server metadata published at /.well-known/oauth-authorization-server on getunblocked.com.
kind: authentication
layout: security
method: searched
name: Unblocked Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Unblocked secures its APIs with http-bearer and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Unblocked
provider_slug: unblocked
scheme_count: 2
schemes:
- bearerFormat: Unblocked API Key
  description: 'API token sent as `Authorization: Bearer <token>` on every request. Obtainable from the web dashboard under Settings -> API Tokens.'
  name: ApiKeyBearerAuth
  scheme: bearer
  sources:
  - openapi/unblocked-public-api-openapi-original.json
  type: http
- code_challenge_methods:
  - S256
  description: OAuth 2.0 authorization server published via RFC 8414 metadata at https://getunblocked.com/.well-known/oauth-authorization-server (used by the remote MCP integration). Authorization-code + refresh-token grants, PKCE S256 required option, dynamic client registration with no auth.
  flows:
  - authorizationUrl: https://getunblocked.com/dashboard/login/oauth
    flow: authorizationCode
    tokenUrl: https://getunblocked.com/api/auth/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  jwks_uri: https://getunblocked.com/api/auth/oauth/jwks
  name: oauth-authorization-server
  registration_endpoint: https://getunblocked.com/api/auth/oauth/register
  revocation_endpoint: https://getunblocked.com/api/auth/oauth/revoke
  sources:
  - well-known/unblocked-oauth-authorization-server.json
  type: oauth2
slug: unblocked-authentication
source_filename: unblocked-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.getunblocked.com/api-reference/quickstart\ndocs: https://docs.getunblocked.com/api-reference/quickstart\ndescription: >-\n  Authentication profile for the Unblocked Public API and tooling surface,\n  captured from the API quickstart, the published OpenAPI securitySchemes, the\n  CLI auth docs, and the OAuth authorization-server metadata published at\n  /.well-known/oauth-authorization-server on getunblocked.com.\nsummary:\n  types: [http-bearer, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: ApiKeyBearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: Unblocked API Key\n    description: >-\n      API token sent as `Authorization: Bearer <token>` on every request.\n      Obtainable from the web dashboard under Settings -> API Tokens.\n    sources: [openapi/unblocked-public-api-openapi-original.json]\n  - name: oauth-authorization-server\n    type: oauth2\n  \
  \  description: >-\n      OAuth 2.0 authorization server published via RFC 8414 metadata at\n      https://getunblocked.com/.well-known/oauth-authorization-server (used by\n      the remote MCP integration). Authorization-code + refresh-token grants,\n      PKCE S256 required option, dynamic client registration with no auth.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://getunblocked.com/dashboard/login/oauth\n        tokenUrl: https://getunblocked.com/api/auth/oauth/token\n    registration_endpoint: https://getunblocked.com/api/auth/oauth/register\n    revocation_endpoint: https://getunblocked.com/api/auth/oauth/revoke\n    jwks_uri: https://getunblocked.com/api/auth/oauth/jwks\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    sources: [well-known/unblocked-oauth-authorization-server.json]\ntoken_types:\n  - name: Personal Access Token\n    scope: Individual user account; user-level isolation on the Answers\
  \ API (only that user's questions are returned).\n    limits: 1,000 API calls per day\n    data_source_scoping: Token can be limited to specific data sources at creation time.\n  - name: Team Access Token\n    scope: Organization-wide; grants access to all documents in the team's data sources.\n    guidance: Rotate regularly; use carefully.\n    data_source_scoping: Token can be limited to specific data sources at creation time.\ncli_and_ci: >-\n  The CLI authenticates interactively via `unblocked auth` (browser flow) or\n  headlessly via the UNBLOCKED_API_TOKEN environment variable using the same\n  personal/team tokens.\nsso: >-\n  End-user sign-in supports SAML 2.0 SSO (Okta, Microsoft Entra ID, Google\n  Workspace, AWS Identity Center, PingOne, and other SAML providers) plus SCIM\n  provisioning; documented under team-settings/sso in the provider docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unblocked/refs/heads/main/authentication/unblocked-authentication.yml
summary_line: http-bearer/oauth2 · 2 schemes
tags:
- Company
- Developer Tools
- AI
- Developer Experience
- Knowledge Management
- Code Review
- MCP
- AI Agents
- Context Engineering
- Search
---
