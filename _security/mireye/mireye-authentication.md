---
api_key_in: []
api_specs:
- filename: mireye-ask-api-openapi.yml
  format: yaml
  label: Mireye Ask API
  slug: mireye-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-ask-api-openapi.yml
- filename: mireye-ask-site-api-openapi.yml
  format: yaml
  label: Mireye Ask Site API
  slug: mireye-ask-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-ask-site-api-openapi.yml
- filename: mireye-auth-api-openapi.yml
  format: yaml
  label: Mireye Auth API
  slug: mireye-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-auth-api-openapi.yml
- filename: mireye-authorize-api-openapi.yml
  format: yaml
  label: Mireye Authorize API
  slug: mireye-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-authorize-api-openapi.yml
- filename: mireye-feature-requests-api-openapi.yml
  format: yaml
  label: Mireye Feature Requests API
  slug: mireye-feature-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-feature-requests-api-openapi.yml
- filename: mireye-fetch-api-openapi.yml
  format: yaml
  label: Mireye Fetch API
  slug: mireye-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-fetch-api-openapi.yml
- filename: mireye-healthz-api-openapi.yml
  format: yaml
  label: Mireye Healthz API
  slug: mireye-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-healthz-api-openapi.yml
- filename: mireye-mcp-api-openapi.yml
  format: yaml
  label: Mireye Mcp API
  slug: mireye-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-mcp-api-openapi.yml
- filename: mireye-meta-api-openapi.yml
  format: yaml
  label: Mireye Meta API
  slug: mireye-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-meta-api-openapi.yml
- filename: mireye-oauth-api-openapi.yml
  format: yaml
  label: Mireye Oauth API
  slug: mireye-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-oauth-api-openapi.yml
- filename: mireye-readyz-api-openapi.yml
  format: yaml
  label: Mireye Readyz API
  slug: mireye-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-readyz-api-openapi.yml
- filename: mireye-register-api-openapi.yml
  format: yaml
  label: Mireye Register API
  slug: mireye-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-register-api-openapi.yml
- filename: mireye-revoke-api-openapi.yml
  format: yaml
  label: Mireye Revoke API
  slug: mireye-revoke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-revoke-api-openapi.yml
- filename: mireye-sites-api-openapi.yml
  format: yaml
  label: Mireye Sites API
  slug: mireye-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-sites-api-openapi.yml
- filename: mireye-token-api-openapi.yml
  format: yaml
  label: Mireye Token API
  slug: mireye-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-token-api-openapi.yml
- filename: mireye-users-api-openapi.yml
  format: yaml
  label: Mireye Users API
  slug: mireye-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-users-api-openapi.yml
- filename: mireye-well-known-api-openapi.yml
  format: yaml
  label: Mireye .well Known API
  slug: mireye-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-well-known-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mireye Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mireye secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mireye
provider_slug: mireye
scheme_count: 3
schemes:
- applies_to:
  - POST /v1/ask
  - POST /v1/ask/stream
  - POST /v1/fetch
  - /v1/users/me/*
  bearer_format: JWT
  description: 'Dashboard-minted API token (JWT, 90-day default lifetime) sent as `Authorization: Bearer <token>` on all /v1/ask, /v1/fetch, and /v1/users/me/* requests. No API-key query params or custom headers.'
  name: bearerAuth
  scheme: bearer
  type: http
- description: OAuth 2.1 + PKCE for the hosted MCP endpoint (/mcp). MCP clients discover the authorization server via /.well-known/oauth-authorization-server and complete a browser flow automatically. Tokens are scoped to MCP tool calls and are NOT accepted as general /v1/* API tokens.
  flows:
  - authorizationUrl: https://api.mireye.com/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.mireye.com/register
    revocationUrl: https://api.mireye.com/revoke
    scopes:
      mcp:tools: Call Mireye MCP tools (mireye_ask, mireye_fetch)
    tokenUrl: https://api.mireye.com/token
  name: mcpOAuth
  type: oauth2
- description: 'Device-authorization flow used by the local stdio adapter (`mireye-mcp login`): POST /v1/mcp/device/start -> browser approval -> POST /v1/mcp/device/poll, storing an API token in ~/.config/mireye-mcp/credentials.json bound to MIREYE_BASE_URL.'
  name: deviceFlow
  type: oauth2-device
slug: mireye-authentication
source_filename: mireye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mireye.ai/authentication\ndocs: https://docs.mireye.ai/authentication\nnote: >-\n  The published OpenAPI (openapi/mireye-openapi-original.json) declares no\n  components.securitySchemes, so this profile is captured from the docs auth page rather\n  than derived from the spec.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Dashboard-minted API token (JWT, 90-day default lifetime) sent as\n    `Authorization: Bearer <token>` on all /v1/ask, /v1/fetch, and /v1/users/me/* requests.\n    No API-key query params or custom headers.\n  applies_to: [POST /v1/ask, POST /v1/ask/stream, POST /v1/fetch, /v1/users/me/*]\n- name: mcpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.1 + PKCE for the hosted MCP endpoint (/mcp). MCP clients discover the\n    authorization\
  \ server via /.well-known/oauth-authorization-server and complete a browser\n    flow automatically. Tokens are scoped to MCP tool calls and are NOT accepted as general\n    /v1/* API tokens.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mireye.com/authorize\n    tokenUrl: https://api.mireye.com/token\n    registrationUrl: https://api.mireye.com/register\n    revocationUrl: https://api.mireye.com/revoke\n    pkce: S256\n    scopes:\n      mcp:tools: Call Mireye MCP tools (mireye_ask, mireye_fetch)\n- name: deviceFlow\n  type: oauth2-device\n  description: >-\n    Device-authorization flow used by the local stdio adapter (`mireye-mcp login`):\n    POST /v1/mcp/device/start -> browser approval -> POST /v1/mcp/device/poll, storing an\n    API token in ~/.config/mireye-mcp/credentials.json bound to MIREYE_BASE_URL.\npublic_endpoints:\n- GET /healthz\n- GET /readyz\n- GET /v1/meta/fields\n- GET /v1/openapi.json\n- GET /v1/docs\nidentity_provider: Firebase (Google\
  \ or email/password with verified address)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/authentication/mireye-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Geospatial
- Geographic Information System
- Location
- AI Agents
- MCP
- Government Data
- Risk
- Insurance
- Data
---
