---
api_key_in: []
api_specs:
- filename: toksta-public-api-openapi.yml
  format: yaml
  label: Toksta Public API
  slug: toksta-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-public-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Toksta Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: toksta secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: toksta
provider_slug: toksta
scheme_count: 2
schemes:
- applies_to: https://api.toksta.com/v1/
  bearerFormat: API key
  eligibility: Requires an active dedicated API plan (PAYG, Build, Scale, Enterprise) or a SaaS plan (Starter, Pro, Agency, PAYG) with api_access_enabled. Free plans cannot create API keys.
  in: header
  issuance: Self-serve from the app at hub.toksta.com — Account -> API keys (/account#api-keys).
  key_prefix: tk_live_
  key_shape: tk_live_ followed by 48 hex characters
  name: bearerAuth
  negative_facts:
  - No query-string API key auth.
  - No cookie auth.
  - No X-Api-Key header — the docs state Authorization Bearer is the only accepted form.
  parameter_name: Authorization
  rotation: Rotation issues a new secret (shown once) and immediately revokes the previous key. Revoked keys return 401 UNAUTHORIZED.
  scheme: bearer
  scoping: A key may be restricted to a subset of endpoint families at creation. A scoped key calling a disallowed route returns 403 FORBIDDEN. See scopes/toksta-scopes.yml.
  sources:
  - https://help.toksta.com/public-api/authentication
  - openapi/toksta-public-api-openapi.yml
  storage: Toksta stores only a SHA-256 hash of the key; the secret is displayed once at creation and cannot be recovered afterwards.
  type: http
- applies_to: https://mcp.toksta.com/mcp
  description: The hosted Toksta MCP server is an OAuth 2.0 protected resource. Unauthenticated POSTs to /mcp return 401 with a WWW-Authenticate Bearer challenge carrying resource_metadata, and the resource metadata names a Supabase Auth authorization server. Dynamic client registration is advertised.
  flows:
  - authorization_endpoint: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    issuer: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1
    pkce:
    - S256
    - plain
    registration_endpoint: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1/oauth/clients/register
    response_types:
    - code
    scopes_note: The authorization-server metadata document declares no scopes_supported. Entitlement is enforced by plan/credit state rather than by OAuth scope — see mcp/toksta-mcp.yml.
    scopes_supported: null
    token_endpoint: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
  name: mcpOAuth
  sources:
  - well-known/toksta-mcp-oauth-authorization-server.json
  - well-known/toksta-mcp-oauth-protected-resource.json
  type: oauth2
slug: toksta-authentication
source_filename: toksta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.toksta.com/public-api/authentication\ndocs: https://help.toksta.com/public-api/authentication\nalso_sourced_from:\n- https://help.toksta.com/account/managing-api-keys\n- https://help.toksta.com/public-api/getting-started\n- https://mcp.toksta.com/.well-known/oauth-authorization-server\n- https://mcp.toksta.com/.well-known/oauth-protected-resource\n- openapi/toksta-public-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Two distinct surfaces with two distinct auth models. The Public REST API\n    (api.toksta.com) uses HTTP Bearer with a self-serve, one-time-reveal API key.\n    The hosted MCP server (mcp.toksta.com/mcp) uses OAuth 2.0 against a Supabase\n    Auth authorization server, advertised via RFC 8414 + RFC 9728 metadata.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  in:\
  \ header\n  parameter_name: Authorization\n  applies_to: https://api.toksta.com/v1/\n  key_prefix: tk_live_\n  key_shape: 'tk_live_ followed by 48 hex characters'\n  storage: >-\n    Toksta stores only a SHA-256 hash of the key; the secret is displayed once at\n    creation and cannot be recovered afterwards.\n  issuance: Self-serve from the app at hub.toksta.com — Account -> API keys (/account#api-keys).\n  eligibility: >-\n    Requires an active dedicated API plan (PAYG, Build, Scale, Enterprise) or a SaaS\n    plan (Starter, Pro, Agency, PAYG) with api_access_enabled. Free plans cannot\n    create API keys.\n  rotation: >-\n    Rotation issues a new secret (shown once) and immediately revokes the previous\n    key. Revoked keys return 401 UNAUTHORIZED.\n  scoping: >-\n    A key may be restricted to a subset of endpoint families at creation. A scoped\n    key calling a disallowed route returns 403 FORBIDDEN. See scopes/toksta-scopes.yml.\n  negative_facts:\n  - No query-string API key\
  \ auth.\n  - No cookie auth.\n  - No X-Api-Key header — the docs state Authorization Bearer is the only accepted form.\n  sources:\n  - https://help.toksta.com/public-api/authentication\n  - openapi/toksta-public-api-openapi.yml\n- name: mcpOAuth\n  type: oauth2\n  applies_to: https://mcp.toksta.com/mcp\n  description: >-\n    The hosted Toksta MCP server is an OAuth 2.0 protected resource. Unauthenticated\n    POSTs to /mcp return 401 with a WWW-Authenticate Bearer challenge carrying\n    resource_metadata, and the resource metadata names a Supabase Auth authorization\n    server. Dynamic client registration is advertised.\n  flows:\n  - flow: authorizationCode\n    issuer: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1\n    authorization_endpoint: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1/oauth/authorize\n    token_endpoint: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1/oauth/token\n    registration_endpoint: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1/oauth/clients/register\n\
  \    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n    pkce: [S256, plain]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    scopes_supported: null\n    scopes_note: >-\n      The authorization-server metadata document declares no scopes_supported. Entitlement\n      is enforced by plan/credit state rather than by OAuth scope — see mcp/toksta-mcp.yml.\n  sources:\n  - well-known/toksta-mcp-oauth-authorization-server.json\n  - well-known/toksta-mcp-oauth-protected-resource.json\nobserved:\n- probe: 'POST https://api.toksta.com/v1/creators/search (no Authorization header)'\n  http_status: 401\n  body: '{\"success\":false,\"error\":{\"code\":\"UNAUTHORIZED\",\"message\":\"Provide an API key using the Authorization: Bearer header.\"},...}'\n  fetched: '2026-08-13'\n- probe: 'POST https://mcp.toksta.com/mcp (tools/list, no Authorization header)'\n  http_status: 401\n  www_authenticate: 'Bearer error=\"invalid_token\", error_description=\"\
  Missing Authorization header\", resource_metadata=\"https://mcp.toksta.com/.well-known/oauth-protected-resource/mcp\"'\n  fetched: '2026-08-13'\nsecurity_guidance_published:\n- Call the API server-to-server only; never embed keys in browser or mobile clients.\n- Store keys in a secrets manager, not in source control.\n- Use a separate key per integration or service.\n- Rotate on a schedule and after team-member offboarding.\n- Monitor consumption via GET /v1/account/usage.\ncross_links:\n  scopes: scopes/toksta-scopes.yml\n  conventions: conventions/toksta-conventions.yml\n  errors: errors/toksta-problem-types.yml\n  mcp: mcp/toksta-mcp.yml\n  well_known: well-known/toksta-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/authentication/toksta-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Influencer Marketing
- Marketing
- B2B
- Creator Discovery
- AI Agents
- LinkedIn
- YouTube
- Software-as-a-Service
- Creator Data
- MCP
- Brand Monitoring
---
