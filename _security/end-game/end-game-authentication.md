---
api_key_in:
- header
api_specs:
- filename: end-game-threads-api-openapi.yml
  format: yaml
  label: Endgame Threads API
  slug: end-game-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-threads-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: End Game Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
overview: Endgame secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and deviceCode flow(s).
provider_name: Endgame
provider_slug: end-game
scheme_count: 2
schemes:
- applies_to: REST API (/api/v1/*)
  description: 'One of: an Endgame API key prefixed `eak_` (created from Settings → API Keys with a Personal or Org-wide scope), or a WorkOS access token from an Endgame-provisioned M2M application (created from Settings → Applications and exchanged via the `client_credentials` grant).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/end-game-threads-api-openapi.yml
  - https://docs.endgame.io/api-reference/authentication
  type: http
- applies_to: MCP endpoint (https://app.endgame.io/api/v1/mcp), Endgame CLI, M2M applications
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://login.endgame.io/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://login.endgame.io/oauth2/token
  - deviceAuthorizationUrl: https://login.endgame.io/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://login.endgame.io/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://login.endgame.io/oauth2/token
  introspection_endpoint: https://login.endgame.io/oauth2/introspection
  issuer: https://app.endgame.io
  jwks_uri: https://login.endgame.io/oauth2/jwks
  name: WorkOS OAuth 2.0
  registration_endpoint: https://login.endgame.io/oauth2/register
  scopes_ref: scopes/end-game-scopes.yml
  sources:
  - https://app.endgame.io/.well-known/oauth-authorization-server
  - https://docs.endgame.io/api-reference/authentication
  type: oauth2
slug: end-game-authentication
source_filename: end-game-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/end-game-threads-api-openapi.yml\ndocs:\n- https://docs.endgame.io/api-reference/authentication\n- https://app.endgame.io/.well-known/oauth-authorization-server\n- https://app.endgame.io/.well-known/oauth-protected-resource\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  note: >-\n    Two authentication surfaces. The REST API takes a single Bearer credential —\n    either a static Endgame API key (eak_ prefix) or a WorkOS-issued JWT — and the\n    OpenAPI declares only that one http/bearer scheme. The MCP endpoint and the CLI\n    use full OAuth 2.0 against the authorization server advertised at\n    app.endgame.io, whose endpoints are delegated to WorkOS at login.endgame.io.\n    Authorization is expressed as PRINCIPAL, not scope: see scopes/end-game-scopes.yml.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme:\
  \ bearer\n  applies_to: REST API (/api/v1/*)\n  description: 'One of: an Endgame API key prefixed `eak_` (created from Settings → API Keys\n    with a Personal or Org-wide scope), or a WorkOS access token from an Endgame-provisioned\n    M2M application (created from Settings → Applications and exchanged via the `client_credentials`\n    grant).'\n  sources:\n  - openapi/end-game-threads-api-openapi.yml\n  - https://docs.endgame.io/api-reference/authentication\n- name: WorkOS OAuth 2.0\n  type: oauth2\n  applies_to: MCP endpoint (https://app.endgame.io/api/v1/mcp), Endgame CLI, M2M applications\n  issuer: https://app.endgame.io\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.endgame.io/oauth2/authorize\n    tokenUrl: https://login.endgame.io/oauth2/token\n    pkce: S256\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.endgame.io/oauth2/device_authorization\n    tokenUrl: https://login.endgame.io/oauth2/token\n  - flow: clientCredentials\n   \
  \ tokenUrl: https://login.endgame.io/oauth2/token\n  jwks_uri: https://login.endgame.io/oauth2/jwks\n  introspection_endpoint: https://login.endgame.io/oauth2/introspection\n  registration_endpoint: https://login.endgame.io/oauth2/register\n  dynamic_client_registration: true\n  scopes_ref: scopes/end-game-scopes.yml\n  sources:\n  - https://app.endgame.io/.well-known/oauth-authorization-server\n  - https://docs.endgame.io/api-reference/authentication\ncredentials:\n- kind: api-key\n  prefix: eak_\n  scope_toggle: [Personal, Org-wide]\n  provisioning: https://app.endgame.io/settings/api-keys\n  admin_only: true\n  shown_once: true\n  scope_immutable: true\n  revocation: >-\n    Revoked from the API Keys settings page; immediate. Personal keys are revoked\n    automatically when the owning user leaves the organization.\n- kind: m2m-application\n  provisioning: https://app.endgame.io/settings/applications\n  admin_only: true\n  grant: client_credentials\n  token_endpoint: https://login.endgame.io/oauth2/token\n\
  \  token_format: JWT\n  note: >-\n    Endgame provisions a WorkOS OAuth client and returns a client id and secret; the\n    secret is shown once and can be rotated. Deleting the application revokes all\n    tokens issued under it. Endgame's own docs prefer M2M over org-wide API keys for\n    read-only service integrations because short-lived tokens are easier to contain.\nauthorization:\n  model: principal-based\n  principals:\n  - {principal: user, credentials: [personal API key, user OAuth token], writes: true, reads: 'own threads + every org-published thread'}\n  - {principal: org-wide service identity, credentials: [org-wide API key, M2M application token], writes: false, reads: 'every org-published thread'}\n  mutation_rule: >-\n    Writes require a user identity. Org-wide credentials return 403 FORBIDDEN on\n    create, rename and delete. Only a thread's creator may rename or delete it, even\n    when the thread is published to the organization. Cross-organization access is\n   \
  \ always denied.\n  gap: >-\n    Endgame's own documentation states org-wide write scope is on the roadmap; today\n    a write-capable automation must use a personal API key issued under a dedicated\n    service-account user.\nfailure_modes:\n- {status: 401, code: UNAUTHORIZED, cause: missing, malformed or revoked credential}\n- {status: 403, code: FORBIDDEN, cause: valid credential without permission to mutate this thread}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/authentication/end-game-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Sales
- Revenue Intelligence
- Go-To-Market
- Artificial Intelligence
- Agents
- MCP
- Knowledge Graph
- CRM
- Conversation Intelligence
---
