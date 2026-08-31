---
api_key_in:
- header
- query
api_specs:
- filename: textql-v2-openapi.yml
  format: yaml
  label: TextQL v2 API
  slug: textql-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-v2-openapi.yml
- filename: textql-chat-v1-openapi.yml
  format: yaml
  label: TextQL Platform API (v1)
  slug: textql-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-chat-v1-openapi.yml
- filename: textql-platform-api-openapi.yml
  format: yaml
  label: TextQL Public RPC API
  slug: textql-public-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-platform-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Textql Authentication
name_suffix: Authentication
oauth_flows: []
overview: TextQL secures its APIs with apiKey, http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TextQL
provider_slug: textql
scheme_count: 5
schemes:
- accepts:
  - platform API key
  - JWT
  base: https://app.textql.com/v2
  header: 'Authorization: Bearer <key>'
  method: derived
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/textql-v2-openapi.yml
  surface: TextQL v2 API
  type: http
- base: https://app.textql.com/rpc/public
  in: header
  method: derived
  name: apiKey
  parameter: tql_api_key
  sources:
  - openapi/textql-platform-api-openapi.yml
  surface: TextQL Public RPC API
  type: apiKey
- in: query
  method: searched
  name: authKey
  parameter: authKey
  sources:
  - https://docs.textql.com/core/guides/embedding-ana
  surface: Embedded Ana iframe
  type: apiKey
  url_pattern: https://app.textql.com/embed?authKey=<API_KEY>
  warning: A credential in a URL query string. TextQL's own docs say "never expose a long-lived API key in frontend code" and direct production integrations to mint a short-lived, role-scoped service account key server-side per session.
- authorization_server: https://app.textql.com
  declared_in_openapi: false
  declared_in_openapi_note: Not declared as a securityScheme in ANY published spec, despite governing the MCP endpoint and the CLI. A client reading only the OpenAPI would not know OAuth exists on this platform.
  flow: authorization_code
  metadata: https://app.textql.com/.well-known/oauth-authorization-server
  method: probed
  name: oauth2
  pkce: S256
  sources:
  - https://app.textql.com/.well-known/oauth-authorization-server
  surface: MCP server and the ana CLI
  type: oauth2
- discovery: https://app.textql.com/.well-known/openid-configuration
  id_token_alg: EdDSA
  jwks: https://app.textql.com/.well-known/jwks.json
  method: probed
  name: openIdConnect
  type: openIdConnect
slug: textql-authentication
source_filename: textql-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: >-\n  openapi/textql-platform-api-openapi.yml, openapi/textql-v2-openapi.yml (derived baseline), upgraded\n  from https://docs.textql.com/core/admin/api-keys, https://docs.textql.com/core/guides/embedding-ana,\n  https://docs.textql.com/core/admin/cli and https://app.textql.com/.well-known/oauth-authorization-server\ndocs: https://docs.textql.com/core/admin/api-keys\nnote: >-\n  The spec-derived baseline found two schemes. It missed the third and most capable one entirely:\n  TextQL runs a full OAuth 2.1 authorization server, probed live at the discovery endpoint, which no\n  published OpenAPI declares. Three different authentication styles are in production across four\n  surfaces, and a client has to know which surface it is calling to pick one.\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header, query]\n  surfaces: 4\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization:\
  \ Bearer <key>'\n  accepts: [platform API key, JWT]\n  surface: TextQL v2 API\n  base: https://app.textql.com/v2\n  sources: [openapi/textql-v2-openapi.yml]\n  method: derived\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: tql_api_key\n  surface: TextQL Public RPC API\n  base: https://app.textql.com/rpc/public\n  sources: [openapi/textql-platform-api-openapi.yml]\n  method: derived\n- name: authKey\n  type: apiKey\n  in: query\n  parameter: authKey\n  surface: Embedded Ana iframe\n  url_pattern: https://app.textql.com/embed?authKey=<API_KEY>\n  sources: [https://docs.textql.com/core/guides/embedding-ana]\n  method: searched\n  warning: >-\n    A credential in a URL query string. TextQL's own docs say \"never expose a long-lived API key in\n    frontend code\" and direct production integrations to mint a short-lived, role-scoped service\n    account key server-side per session.\n- name: oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  surface: MCP server\
  \ and the ana CLI\n  authorization_server: https://app.textql.com\n  metadata: https://app.textql.com/.well-known/oauth-authorization-server\n  sources: [https://app.textql.com/.well-known/oauth-authorization-server]\n  method: probed\n  declared_in_openapi: false\n  declared_in_openapi_note: >-\n    Not declared as a securityScheme in ANY published spec, despite governing the MCP endpoint and the\n    CLI. A client reading only the OpenAPI would not know OAuth exists on this platform.\n- name: openIdConnect\n  type: openIdConnect\n  discovery: https://app.textql.com/.well-known/openid-configuration\n  jwks: https://app.textql.com/.well-known/jwks.json\n  id_token_alg: EdDSA\n  method: probed\noauth:\n  authorization_endpoint: https://app.textql.com/oauth/authorize\n  token_endpoint: https://app.textql.com/oauth/token\n  revocation_endpoint: https://app.textql.com/oauth/revoke\n  registration_endpoint: https://app.textql.com/oauth/register\n  grant_types: [authorization_code, refresh_token]\n\
  \  response_types: [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_post]\n  dynamic_client_registration: true\n  scope_count: 34\n  scopes: scopes/textql-scopes.yml\n  implicit_grant: false\n  password_grant: false\n  posture_note: >-\n    Authorization-code-with-PKCE only, plus dynamic client registration and a revocation endpoint.\n    No implicit or resource-owner-password grant is offered. This is a current, correct OAuth 2.1\n    posture rather than a legacy OAuth 2.0 one.\napi_keys:\n  issuance_ui: Settings → Developers → API Keys\n  issuance_api: v2.createApiKey (POST /v2/api-keys)\n  admin_required_for_ui_creation: true\n  shown_once: true\n  types:\n  - name: Personal\n    acts_as: the creating member\n    permission_required: none\n  - name: Service Account\n    acts_as: a dedicated non-human member\n    permission_required: 'organization:write'\n    recommended_for: production embeds and automations\n  expiry: supported (e.g. 3600 seconds)\n\
  \  rotation: v2.rotateApiKey — revoke and mint a replacement with the same scope in one call\n  revocation: v2.revokeApiKey\n  metadata: clientId, read per request by TQL row-level security for multi-tenant embedding\n  authorization_model:\n    owner_vs_roles: >-\n      Every key has an OWNER (the member it authenticates as, deciding personal shares, connector\n      grants, creator bypass and audit attribution) and ASSUMED ROLES (deciding permissions). Roles\n      cannot substitute for ownership — a key with the admin role but the wrong owner is still denied\n      a Data App shared with a specific colleague.\n    role_snapshot: >-\n      Assumed roles are a snapshot taken at key creation and NEVER update. The snapshot is intersected\n      with the owner's live roles on every request, so a key can lose access when a role is removed\n      but never gain access when one is added. Legacy keys showing \"All roles\" predate snapshots and\n      do track role changes.\n    resolution: per\
  \ request, not at login\ncustomer_sso:\n  note: TextQL is also a relying party for customer identity, sold at the Enterprise tier.\n  protocols: [SAML 2.0, OIDC]\n  initiation: [IdP-initiated, SP-initiated]\n  provisioning: JIT on first login, SCIM 2.0 for lifecycle, directory sync\n  controls: [domain claim enforcement, MFA enforced at the customer IdP]\n  source: https://textql.com/security\ncross_references:\n  scopes: scopes/textql-scopes.yml\n  conventions: conventions/textql-conventions.yml\n  cli: cli/textql-cli.yml\n  mcp: mcp/textql-mcp.yml\n  well_known: well-known/textql-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/authentication/textql-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Artificial Intelligence
- Analytics
- Business Intelligence
- Data
- Agents
- MCP
- Semantic Layer
- Text-to-SQL
- Data Warehouse
- Enterprise
---
