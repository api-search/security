---
anonymous_access: false
api_key_in: []
api_specs:
- filename: competitortracker-io-openapi-generated.yml
  format: yaml
  label: Competitor Tracker & Co. API
  slug: competitortracker-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/competitortracker-io/openapi/_ae-authored/competitortracker-io-openapi-generated.yml
auth_types: []
description: 'Every call to /v1/* on https://api.competitortracker.io needs a credential. Two kinds are accepted: an OAuth 2.0 bearer token (PKCE + OpenID Connect, for apps that sign a person in) on the Authorization header, or an organization API key (prefix ctk_) on the X-API-Key header. "If both headers arrive the API key wins." The MCP server at mcp.competitortracker.io accepts the same credentials and mints none of its own.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Competitor Tracker & Co. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Competitor Tracker & Co. declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Competitor Tracker & Co.
provider_slug: competitortracker-io
scheme_count: 2
schemes:
- authorization_server: https://auth.competitortracker.io
  authorization_url: https://auth.competitortracker.io/oauth/authorize
  discovery:
  - https://api.competitortracker.io/.well-known/oauth-protected-resource
  - https://auth.competitortracker.io/.well-known/oauth-authorization-server
  - https://auth.competitortracker.io/.well-known/openid-configuration
  - https://auth.competitortracker.io/oauth/jwks.json
  dynamic_client_registration: RFC 7591
  flows:
  - authorizationCode
  header: 'Authorization: Bearer <access_token>'
  login_methods:
  - emailed 6-character code
  - magic link
  - Continue with Google
  name: oauth2
  pkce: S256 only
  refresh: on 401, call /oauth/token with grant_type=refresh_token and retry once; refresh rotation is mandatory
  registration_url: https://auth.competitortracker.io/oauth/register
  revocation_url: https://auth.competitortracker.io/oauth/revoke
  token_format: ES256-signed JWT access tokens (15 min) plus opaque refresh tokens (30 days, rotated on use)
  token_url: https://auth.competitortracker.io/oauth/token
  type: oauth2
- audit: GET /v1/api-keys/{id}/usage per-key usage log
  expiry: optional expiresAt; keys without it never expire
  header: X-API-Key
  in: header
  issued_via: POST /v1/api-keys (any member) or the app's API keys page
  name: apiKey
  prefix: ctk_
  revocation: DELETE /v1/api-keys/{id} (immediate, no grace window, no undo)
  rotation: POST /v1/api-keys/{id}/regenerate (old secret stops working at once)
  shown_once: true
  type: apiKey
slug: competitortracker-io-authentication
source_filename: competitortracker-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://competitortracker.io/docs/authentication/\ndocs: https://competitortracker.io/docs/authentication/\nsee_also:\n- https://competitortracker.io/docs/api-keys/\n- https://competitortracker.io/docs/scopes-and-permissions/\ndescription: >-\n  Every call to /v1/* on https://api.competitortracker.io needs a credential. Two kinds are accepted:\n  an OAuth 2.0 bearer token (PKCE + OpenID Connect, for apps that sign a person in) on the\n  Authorization header, or an organization API key (prefix ctk_) on the X-API-Key header. \"If both\n  headers arrive the API key wins.\" The MCP server at mcp.competitortracker.io accepts the same\n  credentials and mints none of its own.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows: [authorizationCode]\n  pkce: S256 only\n  authorization_server: https://auth.competitortracker.io\n  authorization_url: https://auth.competitortracker.io/oauth/authorize\n  token_url: https://auth.competitortracker.io/oauth/token\n\
  \  registration_url: https://auth.competitortracker.io/oauth/register\n  revocation_url: https://auth.competitortracker.io/oauth/revoke\n  dynamic_client_registration: RFC 7591\n  discovery:\n  - https://api.competitortracker.io/.well-known/oauth-protected-resource\n  - https://auth.competitortracker.io/.well-known/oauth-authorization-server\n  - https://auth.competitortracker.io/.well-known/openid-configuration\n  - https://auth.competitortracker.io/oauth/jwks.json\n  token_format: ES256-signed JWT access tokens (15 min) plus opaque refresh tokens (30 days, rotated on use)\n  refresh: on 401, call /oauth/token with grant_type=refresh_token and retry once; refresh rotation is mandatory\n  login_methods: [emailed 6-character code, magic link, Continue with Google]\n  header: 'Authorization: Bearer <access_token>'\n- name: apiKey\n  type: apiKey\n  in: header\n  header: X-API-Key\n  prefix: ctk_\n  issued_via: POST /v1/api-keys (any member) or the app's API keys page\n  shown_once: true\n\
  \  expiry: optional expiresAt; keys without it never expire\n  rotation: POST /v1/api-keys/{id}/regenerate (old secret stops working at once)\n  revocation: DELETE /v1/api-keys/{id} (immediate, no grace window, no undo)\n  audit: GET /v1/api-keys/{id}/usage per-key usage log\nauthorization:\n  model: scope on the credential AND organization role (member < admin < owner); both must pass\n  scopes: scopes/competitortracker-io-scopes.yml\nnote: Endpoints documented here were read from the docs only; no authentication endpoint was called.\n"
source_yaml_url: https://artifacts.apis.io/competitortracker-io/authentication/competitortracker-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Competitive Intelligence
- Competitor Tracking
- Website Change Monitoring
- Price Monitoring
- Market Intelligence
- MCP
- AI Agents
---
