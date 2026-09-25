---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dokki-one-openapi.yml
  format: yaml
  label: Dokki API
  slug: dokki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dokki-one/refs/heads/main/openapi/dokki-one-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Dokki One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dokki secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dokki
provider_slug: dokki-one
scheme_count: 3
schemes:
- applies_to: REST API (/api/v1) and MCP endpoints
  description: Authorization Bearer header carrying a dk_ API key, a Supabase bearer token, or (MCP) an OAuth access token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dokki-one-openapi.yml
  - https://dokki.one/pub/api/authentication
  type: http
- applies_to: MCP endpoints (https://dokki.one/mcp/v2, https://dokki.one/api/mcp)
  consent: On the consent screen the user selects any combination of Personal, one or more Organizations and specific Workspaces; the grant is the union of that selection and never exceeds the user's own permissions.
  dynamic_client_registration: https://schcrwqbgkcmhdltwgcz.supabase.co/auth/v1/oauth/clients/register
  flows:
    authorizationCode:
      authorizationUrl: https://schcrwqbgkcmhdltwgcz.supabase.co/auth/v1/oauth/authorize
      refreshUrl: https://dokki.one/api/oauth/token
      scopes:
        email: Email claims
        offline_access: Refresh tokens
        openid: OpenID Connect identity
        phone: Phone claims
        profile: Profile claims (name, picture, preferred_username)
      tokenUrl: https://dokki.one/api/oauth/token
  name: DokkiOAuth
  pkce:
  - S256
  - plain
  sources:
  - https://dokki.one/.well-known/oauth-authorization-server
  - https://dokki.one/pub/docs/clients
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- id_token_signing_alg_values_supported:
  - RS256
  - HS256
  - ES256
  issuer: https://dokki.one
  jwks_uri: https://schcrwqbgkcmhdltwgcz.supabase.co/auth/v1/.well-known/jwks.json
  name: DokkiOIDC
  openIdConnectUrl: https://dokki.one/.well-known/openid-configuration
  sources:
  - https://dokki.one/.well-known/openid-configuration
  type: openIdConnect
slug: dokki-one-authentication
source_filename: dokki-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://dokki.one/pub/api/authentication\ndocs: https://dokki.one/pub/api/authentication\nspec: openapi/dokki-one-openapi.yml\ncorroborating_sources:\n- https://dokki.one/pub/api/api-keys-and-scopes\n- https://dokki.one/pub/docs/clients\n- https://dokki.one/pub/docs/workspace-connectors\n- https://dokki.one/.well-known/oauth-authorization-server\n- https://dokki.one/.well-known/oauth-protected-resource\nsummary:\n  types: [http, oauth2, openIdConnect]\n  transport: Authorization header, Bearer scheme, HTTPS only\n  note: >-\n    The REST API (https://dokki.one/api/v1) authenticates with a bearer credential — a Dokki API key\n    (dk_...), a Supabase access token, or the browser session — and authorizes through three gates\n    (token scope, tenant boundary, object permission). The MCP servers add OAuth 2.0 / OIDC with\n    discovery and dynamic client registration (RFC 8414, RFC 9728, RFC 7591) so interactive clients\n    can\
  \ sign in without a key, plus workspace-scoped connector tokens for machines. The generated\n    OpenAPI models the REST side as one http bearer scheme; the OAuth side is documented here and in\n    scopes/dokki-one-scopes.yml because it is not visible from the REST reference.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applies_to: REST API (/api/v1) and MCP endpoints\n  description: Authorization Bearer header carrying a dk_ API key, a Supabase bearer token, or (MCP) an OAuth access token.\n  sources: [openapi/dokki-one-openapi.yml, https://dokki.one/pub/api/authentication]\n- name: DokkiOAuth\n  type: oauth2\n  applies_to: MCP endpoints (https://dokki.one/mcp/v2, https://dokki.one/api/mcp)\n  flows:\n    authorizationCode:\n      authorizationUrl: https://schcrwqbgkcmhdltwgcz.supabase.co/auth/v1/oauth/authorize\n      tokenUrl: https://dokki.one/api/oauth/token\n      refreshUrl: https://dokki.one/api/oauth/token\n      scopes:\n        openid: OpenID Connect identity\n\
  \        profile: Profile claims (name, picture, preferred_username)\n        email: Email claims\n        phone: Phone claims\n        offline_access: Refresh tokens\n  pkce: [S256, plain]\n  dynamic_client_registration: https://schcrwqbgkcmhdltwgcz.supabase.co/auth/v1/oauth/clients/register\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  consent: On the consent screen the user selects any combination of Personal, one or more Organizations and specific Workspaces; the grant is the union of that selection and never exceeds the user's own permissions.\n  sources: [https://dokki.one/.well-known/oauth-authorization-server, https://dokki.one/pub/docs/clients]\n- name: DokkiOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://dokki.one/.well-known/openid-configuration\n  issuer: https://dokki.one\n  id_token_signing_alg_values_supported: [RS256, HS256, ES256]\n  jwks_uri: https://schcrwqbgkcmhdltwgcz.supabase.co/auth/v1/.well-known/jwks.json\n  sources:\
  \ [https://dokki.one/.well-known/openid-configuration]\ncredentials:\n- id: api-key\n  header: 'Authorization: Bearer dk_...'\n  prefix: dk_\n  use: Server-to-server integrations and trusted non-interactive MCP clients\n  issued_by: Dokki account API key manager or POST /api/v1/api-keys (scope api_key:write)\n  tenant: Personal, or exactly one Org (an Org key cannot access a different Org; a Personal key cannot access Org workspaces)\n  scopes: Per-key scope list; new public keys default to read scopes (see scopes/dokki-one-scopes.yml)\n  shown_once: true\n  rotation: Create a replacement key, deploy it, verify GET /api/v1/me, then revoke the old key; record the key id, not the secret.\n- id: supabase-bearer-token\n  header: 'Authorization: Bearer <supabase_access_token>'\n  prefix: null\n  use: First-party clients acting as a signed-in user\n  issued_by: Supabase Auth (Dokki's identity provider)\n- id: browser-session\n  header: cookie session\n  use: The Dokki web app\n- id: oauth-access-token\n\
  \  header: 'Authorization: Bearer <access_token>'\n  use: Interactive MCP clients (Claude, Claude Desktop, Claude Code, Codex, Cursor, ChatGPT) after OAuth discovery + consent\n  issued_by: Dokki token endpoint https://dokki.one/api/oauth/token\n- id: workspace-connector-token\n  header: query parameters in the generated connector URL (workspace id, connector id, one-time token)\n  use: CI jobs, shared automations, dedicated agents locked to ONE workspace (Documents, Publish or Memory flavor)\n  issued_by: Workspace admins under Workspace -> Extensions -> Connectors; raw token shown once, Dokki keeps a hash and visible prefix\n  note: The client must preserve the exact connector URL and query parameters; a different workspace id or connector id is rejected.\nverify_principal:\n  endpoint: GET /api/v1/me\n  returns: [type (authentication mode), user_id, org_id (null for Personal), key_id (API keys), scopes (effective)]\nfailures:\n  '401 unauthorized': missing, invalid, expired or revoked\
  \ credentials\n  '403 insufficient_scope': credential valid but lacks the endpoint scope\n  '403 forbidden': scope valid but tenant or object permission denies access\n  '404': may be returned instead of 403 where revealing existence would leak information\nmcp_challenge:\n  http_status: 401\n  www_authenticate: Bearer resource_metadata=\"https://dokki.one/.well-known/oauth-protected-resource?resource=https%3A%2F%2Fdokki.one%2Fapi%2Fmcp\"\n  body: '{\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Unauthorized\"},\"id\":null}'\nagent_guidance: '\"Do not ask users to paste secrets into a chat. Ask them to create or authorize a key in Dokki, then store it in the host application''s secret manager.\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dokki-one/refs/heads/main/authentication/dokki-one-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Collaboration
- Knowledge Management
- Documents
- Agents
- MCP
- Artificial Intelligence
- Productivity
- Workspace
- Publishing
- Search
- Singapore
---
