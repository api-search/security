---
api_key_in: []
api_specs:
- filename: ok-capsule-core-api-v2-openapi.yaml
  format: yaml
  label: OK Capsule Core API V2
  slug: ok-capsule-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ok-capsule/refs/heads/main/openapi/ok-capsule-core-api-v2-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ok Capsule Authentication
name_suffix: Authentication
oauth_flows: []
overview: OK Capsule secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OK Capsule
provider_slug: ok-capsule
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ok-capsule-core-api-v2-openapi.yaml
  type: http
- flow: authorizationCode
  name: mcp-oauth2
  sources:
  - https://storefront.okcapsule.app/.well-known/oauth-authorization-server
  type: oauth2
slug: ok-capsule-authentication
source_filename: ok-capsule-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.okcapsule.app/docs/getting-started
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.okcapsule.app/docs/getting-started\nsources:\n- https://docs.okcapsule.app/docs/getting-started\n- https://docs.okcapsule.app/docs/recipes/troubleshooting\n- https://okcapsule.com/mcp/developers\n- https://storefront.okcapsule.app/.well-known/oauth-authorization-server\n- openapi/ok-capsule-core-api-v2-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  note: >-\n    OK Capsule runs two independent auth models on two surfaces. The REST Core API V2 uses a\n    username/password token exchange returning a bearer JWT. The MCP server uses OAuth 2.1\n    authorization-code with PKCE and dynamic client registration. They do not share credentials.\nsurfaces:\n- surface: REST Core API V2\n  base_url: https://na1-prod.okcapsule.app\n  scheme: bearerAuth\n  type: http\n  http_scheme: bearer\n  bearer_format: JWT\n  token_endpoint: POST /v2/authentication/token\n  token_request: '{\"username\": \"<email>\", \"password\"\
  : \"<password>\"}'\n  token_response_fields: [access_token, refresh_token, expires_in]\n  access_token_ttl: 24 hours (expires_in 86400)\n  refresh: 'POST /v2/authentication/refresh-token with {\"refresh_token\": \"...\"}'\n  header: 'Authorization: Bearer <access_token>'\n  credential_issuance: >-\n    Not self-serve. Account and brand (Product Line) setup must be complete, then credentials are\n    obtained from an OK Capsule representative.\n  other_auth_operations:\n  - POST /v2/authentication/forgot-password\n  - POST /v2/authentication/reset-password\n  - GET /v2/authentication/user\n  permissions: >-\n    Role-based, managed in the client portal. A 403 means the signed-in user's role lacks the required\n    permission; there are no OAuth scopes on this surface.\n  environment_isolation: >-\n    Users and data are environment-specific. Stage credentials do not work in Production.\n  documented_token_hygiene:\n  - Store tokens in secure encrypted storage; server-side only, never client-side.\n\
  \  - Never commit or log tokens.\n  - Refresh proactively at roughly 80% of TTL; the docs ship a TokenManager example that refreshes with 5 minutes remaining.\n  - Invalidate tokens on logout or credential change.\n  - Never share tokens between stage and production.\n- surface: MCP server\n  base_url: https://storefront.okcapsule.app/mcp\n  type: oauth2\n  model: OAuth 2.1 authorization_code + PKCE\n  pkce: S256 mandatory\n  client_type: public - no client secrets are issued\n  dynamic_client_registration: true\n  grant_types: [authorization_code, refresh_token]\n  machine_to_machine: false\n  login: staff email one-time code - no passwords, no API keys, no anonymous access\n  access_token: RS256 JWT, 1 hour\n  access_token_claims: [sub, role, email, tenant_id, tenant_slug, scope, iss, aud, jti, iat, exp]\n  refresh_token: 30 days, single-use, rotating — always persist the newest\n  revocation: POST /oauth/revoke, immediate\n  redirect_uri_policy: 'https, with the usual localhost loopback\
  \ exception'\n  tenancy: 'one token is bound to exactly one workspace; no token crosses workspaces'\n  scopes: scopes/ok-capsule-scopes.yml\n  discovery:\n  - https://storefront.okcapsule.app/.well-known/oauth-authorization-server\n  - https://storefront.okcapsule.app/.well-known/oauth-protected-resource\n  challenge: >-\n    An unauthenticated request returns HTTP 401 with a WWW-Authenticate Bearer challenge carrying\n    resource_metadata, per RFC 9728, which a conformant MCP client follows automatically into dynamic\n    registration and browser sign-in.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ok-capsule-core-api-v2-openapi.yaml\n- name: mcp-oauth2\n  type: oauth2\n  flow: authorizationCode\n  sources:\n  - https://storefront.okcapsule.app/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ok-capsule/refs/heads/main/authentication/ok-capsule-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Supplements
- Nutrition
- Health
- Manufacturing
- Fulfillment
- Ecommerce
- Personalization
- Orders
- Shipping
- Agents
- MCP
- Telehealth
---
