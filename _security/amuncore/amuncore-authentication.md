---
api_key_in:
- header
api_specs:
- filename: amuncore-dynamic-api-api-openapi.yml
  format: yaml
  label: AmunCore Dynamic API
  slug: amuncore-dynamic-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/openapi/amuncore-dynamic-api-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: AmunCore authenticates three channels differently, and the provider is explicit about the separation. The generated REST API takes a per-application API key in an X-Api-Key header. The MCP endpoint takes a distinct secret (MCP-Token header) or an OAuth 2.0 bearer token with the "mcp" scope, deliberately not the same credential as the REST keys. Dashboard sign-in is separate again, with optional TOTP two-factor.
kind: authentication
layout: security
method: searched
name: Amuncore Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AmunCore secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AmunCore
provider_slug: amuncore
scheme_count: 3
schemes:
- applies_to: REST API (/api/v1/{appId}/{endpointName})
  description: The application's API key, sent on every request. A missing or invalid key returns 401 with {"success":false,"message":"Application '<appId>' not found or API key does not match."} — the same message for an unknown application and a wrong key, so the API does not leak whether an appId exists.
  header: X-Api-Key
  id: ApiKeyAuth
  in: header
  key_properties:
    ip_allowlist: Optional IP allowlisting per application.
    rotation: Rotatable from the dashboard and via the regenerate_api_key MCP tool.
    scoping: Per application, and issuable read-only or read-write per consumer.
    storage: Keys are hashed; the raw value is shown once at issue time.
  name: ApiKeyAuth
  source: https://amuncore.com/openapi.json
  type: apiKey
- applies_to: MCP endpoint (https://amuncore.com/mcp)
  description: 'A secret distinct from the REST API keys, scoped to a single company and disableable per company. Confirmed live: an unauthenticated JSON-RPC POST returns -32001 "Unauthorized: missing MCP-Token header".'
  header: MCP-Token
  id: mcp-token
  in: header
  name: MCP-Token
  source: https://amuncore.com/mcp
  type: apiKey
- applies_to: MCP endpoint (https://amuncore.com/mcp)
  detail: scopes/amuncore-scopes.yml
  flows:
  - authorizationUrl: https://amuncore.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
      mcp: Access the AmunCore MCP endpoint.
    tokenUrl: https://amuncore.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  id: mcp-oauth
  name: OAuth 2.0 (MCP)
  registration_endpoint: https://amuncore.com/oauth/register
  source: https://amuncore.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
slug: amuncore-authentication
source_filename: amuncore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nstatus: published\nsource: >-\n  https://amuncore.com/openapi.json, https://amuncore.com/llms.txt,\n  https://amuncore.com/security.html, https://amuncore.com/.well-known/oauth-authorization-server\ndocs: https://amuncore.com/llms.txt\ndescription: >-\n  AmunCore authenticates three channels differently, and the provider is explicit\n  about the separation. The generated REST API takes a per-application API key in\n  an X-Api-Key header. The MCP endpoint takes a distinct secret (MCP-Token\n  header) or an OAuth 2.0 bearer token with the \"mcp\" scope, deliberately not the\n  same credential as the REST keys. Dashboard sign-in is separate again, with\n  optional TOTP two-factor.\nverified: '2026-08-10'\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_names: [X-Api-Key, MCP-Token]\n  oauth2_flows: [authorizationCode]\n  oauth2_applies_to: [mcp]\nschemes:\n- id: ApiKeyAuth\n  name: ApiKeyAuth\n  type: apiKey\n \
  \ in: header\n  header: X-Api-Key\n  applies_to: REST API (/api/v1/{appId}/{endpointName})\n  source: https://amuncore.com/openapi.json\n  description: >-\n    The application's API key, sent on every request. A missing or invalid key\n    returns 401 with {\"success\":false,\"message\":\"Application '<appId>' not found\n    or API key does not match.\"} — the same message for an unknown application and\n    a wrong key, so the API does not leak whether an appId exists.\n  key_properties:\n    scoping: Per application, and issuable read-only or read-write per consumer.\n    storage: Keys are hashed; the raw value is shown once at issue time.\n    rotation: Rotatable from the dashboard and via the regenerate_api_key MCP tool.\n    ip_allowlist: Optional IP allowlisting per application.\n- id: mcp-token\n  name: MCP-Token\n  type: apiKey\n  in: header\n  header: MCP-Token\n  applies_to: MCP endpoint (https://amuncore.com/mcp)\n  source: https://amuncore.com/mcp\n  description: >-\n    A\
  \ secret distinct from the REST API keys, scoped to a single company and\n    disableable per company. Confirmed live: an unauthenticated JSON-RPC POST\n    returns -32001 \"Unauthorized: missing MCP-Token header\".\n- id: mcp-oauth\n  name: OAuth 2.0 (MCP)\n  type: oauth2\n  applies_to: MCP endpoint (https://amuncore.com/mcp)\n  source: https://amuncore.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://amuncore.com/oauth/authorize\n    tokenUrl: https://amuncore.com/oauth/token\n    scopes:\n      mcp: Access the AmunCore MCP endpoint.\n    pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  registration_endpoint: https://amuncore.com/oauth/register\n  token_endpoint_auth_methods: [none, client_secret_post]\n  detail: scopes/amuncore-scopes.yml\naccount_security:\n  two_factor: Optional TOTP 2FA on dashboard sign-in, with one-time recovery codes and administrator reset.\n  password_storage: BCrypt hashes.\n \
  \ secret_storage: Database connection strings and 2FA secrets encrypted at rest with AES-256.\n  roles: [SuperAdmin, Admin, Developer, Viewer]\n  tenant_isolation: Strict per-company separation enforced on every request.\n  source: https://amuncore.com/security.html\nsignup:\n  url: https://amuncore.com/Register\n  login: https://amuncore.com/Auth/Login\n  free_plan: true\n  note: '\"Free plan forever\" per the homepage pricing table; no card required to begin.'\ngaps:\n- No OpenID Connect. /.well-known/openid-configuration returns 404, so the OAuth\n  layer carries no identity token for the acting agent.\n- No SSO. The provider's own security page lists OAuth2/SAML single sign-on as\n  roadmap, not shipped.\n- The X-Api-Key parameter is declared on each operation with required omitted, so\n  a strict reader of the spec cannot tell the key is mandatory from the parameter\n  alone — only the securitySchemes block and the prose say so.\nevidence:\n- url: https://amuncore.com/openapi.json\n\
  \  status: 200\n- url: https://amuncore.com/api/v1/demo/customers\n  status: 404\n  method: GET\n  note: Unauthenticated call returned the real JSON auth-failure envelope, not HTML.\n- url: https://amuncore.com/mcp\n  status: 401\n  method: POST\n- url: https://amuncore.com/.well-known/oauth-authorization-server\n  status: 200\n- url: https://amuncore.com/security.html\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/authentication/amuncore-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Database
- API Management
- Backend
- No-Code
- SQL
- PostgreSQL
- MySQL
- Oracle
- MCP
- Agents
- Data
- SQL Server
- Webhook
- OpenAPI
- Low-Code
- Egypt
---
