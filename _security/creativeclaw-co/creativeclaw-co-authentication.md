---
anonymous_access: false
api_key_in: []
api_specs:
- filename: creativeclaw-co-health-api-openapi.yml
  format: yaml
  label: CreativeClaw Health API
  slug: creativeclaw-co-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativeclaw-co/openapi/creativeclaw-co-health-api-openapi.yml
- filename: creativeclaw-co-mcp-api-openapi.yml
  format: yaml
  label: CreativeClaw MCP API
  slug: creativeclaw-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativeclaw-co/openapi/creativeclaw-co-mcp-api-openapi.yml
- filename: creativeclaw-co-oauth-api-openapi.yml
  format: yaml
  label: CreativeClaw OAuth API
  slug: creativeclaw-co-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativeclaw-co/openapi/creativeclaw-co-oauth-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CreativeClaw Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CreativeClaw secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CreativeClaw
provider_slug: creativeclaw-co
scheme_count: 2
schemes:
- description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration is supported. Request only `profile` and `email`.
  flows:
  - authorizationUrl: https://clerk.creativeclaw.co/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://clerk.creativeclaw.co/oauth/token
  name: oauth2
  sources:
  - openapi/creativeclaw-co-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: 'Access token from the Clerk token endpoint, sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/creativeclaw-co-openapi.yml
  type: http
slug: creativeclaw-co-authentication
source_filename: creativeclaw-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://creativeclaw.co/auth.md\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.creativeclaw.co/oauth/authorize\n    tokenUrl: https://clerk.creativeclaw.co/oauth/token\n    scopes: 2\n  description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration is supported. Request only `profile`\n    and `email`.\n  sources:\n  - openapi/creativeclaw-co-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Access token from the Clerk token endpoint, sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/creativeclaw-co-openapi.yml\nderived_from: openapi/creativeclaw-co-openapi.yml\ndocs: https://creativeclaw.co/auth.md\ndocumented:\n  discovery: Unauthenticated tools/call on POST /mcp returns HTTP 401 with\
  \ a WWW-Authenticate Bearer challenge whose resource_metadata\n    points at https://app.creativeclaw.co/.well-known/oauth-protected-resource/mcp (RFC 9728); authorization server metadata\n    (RFC 8414) at https://app.creativeclaw.co/.well-known/oauth-authorization-server.\n  pkce: S256 (required)\n  dynamic_client_registration: https://clerk.creativeclaw.co/oauth/register (RFC 7591), public client\n  authorization_endpoint: https://clerk.creativeclaw.co/oauth/authorize\n  token_endpoint: https://clerk.creativeclaw.co/oauth/token\n  revocation_endpoint: https://clerk.creativeclaw.co/oauth/token/revoke\n  jwks: https://clerk.creativeclaw.co/.well-known/jwks.json\n  identity_provider: Clerk (users typically sign in with Gmail)\n  unauthenticated_methods:\n  - initialize\n  - notifications/initialized\n  - ping\n  not_offered:\n  - agent_auth\n  - identity_assertion\n  - service_auth\n  - id-jag\n  - provider API keys\n  note: Docs say \"Never request `openid`\" — Clerk rejects that scope\
  \ for dynamically registered MCP clients.\n"
source_yaml_url: https://artifacts.apis.io/creativeclaw-co/authentication/creativeclaw-co-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Audio
- MCP
- Marketing
---
