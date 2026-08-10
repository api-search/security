---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Spocket Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Spocket secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Spocket
provider_slug: spocket
scheme_count: 2
schemes:
- applies_to: https://www.spocket.dev/api/mcp
  bearer_methods_supported:
  - header
  challenge:
    observed_status: 401
    www_authenticate: Bearer resource_metadata="https://www.spocket.dev/.well-known/oauth-protected-resource"
  consent: The first tool call opens a browser for human consent; the client then holds the token. There is no API key and nothing to paste.
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://www.spocket.dev/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://www.spocket.dev/oauth/register
    revocationUrl: https://www.spocket.dev/oauth/revoke
    scopes:
      spocket: Full access to the connected account's Spocket MCP tool surface
    tokenUrl: https://www.spocket.dev/oauth/token
  name: MCPOAuth21
  response_types_supported:
  - code
  revocation: Every connected tool is listed in account Settings with its last-call time. Revoking one takes effect on the next request and reconnecting requires approval again.
  sources:
  - well-known/spocket-oauth-authorization-server.json
  - well-known/spocket-oauth-protected-resource.json
  surface: Spocket MCP Server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to: https://www.spocket.dev/api/v1
  availability:
    gated: true
    requirement: Paid Fleet plan - the key page unlocks once the account is on Fleet.
  credential_shape:
    client_id_env: SPOCKET_CLIENT_ID
    client_id_prefix: spk_live_
    client_secret_env: SPOCKET_CLIENT_SECRET
    client_secret_prefix: sk_
    storage: Secret is shown once at creation and stored only as a hash.
  flows:
  - flow: clientCredentials
    scopes:
      apps:delete: Delete apps
      apps:read: List apps, read status and logs
      apps:write: Provision, deploy, start, stop, restart
      domains:write: Attach and verify custom domains
    tokenUrl: https://www.spocket.dev/api/v1/token
  name: PlatformClientCredentials
  rotation: Rotating a key keeps the old secret working for 24 hours so it can be rolled out without taking customers offline.
  scope_selection: Scopes are chosen at key creation, so a key that provisions and deploys need not be able to delete.
  sources:
  - https://www.spocket.dev/documentation/platform-api
  surface: Spocket Platform REST API
  token:
    header: authorization
    in: header
    lifetime: 3600
    type: bearer
  type: oauth2
slug: spocket-authentication
source_filename: spocket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://www.spocket.dev/documentation/platform-api\ndocs:\n  - https://www.spocket.dev/documentation/platform-api\n  - https://www.spocket.dev/documentation/quickstart\n  - https://www.spocket.dev/.well-known/oauth-authorization-server\n  - https://www.spocket.dev/.well-known/oauth-protected-resource\nnote: >-\n  Derived by reading the provider's published auth documentation and the two live OAuth\n  discovery documents. No OpenAPI securitySchemes exist to derive from - Spocket publishes\n  no machine-readable spec - so derive-authentication.py has nothing to read.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  api_key_supported: false\n  surfaces: 2\nschemes:\n  - name: MCPOAuth21\n    type: oauth2\n    surface: Spocket MCP Server\n    applies_to: https://www.spocket.dev/api/mcp\n    sources: [well-known/spocket-oauth-authorization-server.json, well-known/spocket-oauth-protected-resource.json]\n\
  \    flows:\n      - flow: authorizationCode\n        pkce: S256\n        authorizationUrl: https://www.spocket.dev/oauth/authorize\n        tokenUrl: https://www.spocket.dev/oauth/token\n        revocationUrl: https://www.spocket.dev/oauth/revoke\n        registrationUrl: https://www.spocket.dev/oauth/register\n        scopes:\n          spocket: Full access to the connected account's Spocket MCP tool surface\n    dynamic_client_registration: true      # RFC 7591\n    token_endpoint_auth_methods_supported: [none]\n    response_types_supported: [code]\n    bearer_methods_supported: [header]\n    consent: >-\n      The first tool call opens a browser for human consent; the client then holds the\n      token. There is no API key and nothing to paste.\n    revocation: >-\n      Every connected tool is listed in account Settings with its last-call time. Revoking\n      one takes effect on the next request and reconnecting requires approval again.\n    challenge:\n      observed_status: 401\n\
  \      www_authenticate: 'Bearer resource_metadata=\"https://www.spocket.dev/.well-known/oauth-protected-resource\"'\n  - name: PlatformClientCredentials\n    type: oauth2\n    surface: Spocket Platform REST API\n    applies_to: https://www.spocket.dev/api/v1\n    sources: ['https://www.spocket.dev/documentation/platform-api']\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://www.spocket.dev/api/v1/token\n        scopes:\n          apps:read: List apps, read status and logs\n          apps:write: Provision, deploy, start, stop, restart\n          apps:delete: Delete apps\n          domains:write: Attach and verify custom domains\n    credential_shape:\n      client_id_env: SPOCKET_CLIENT_ID\n      client_id_prefix: spk_live_\n      client_secret_env: SPOCKET_CLIENT_SECRET\n      client_secret_prefix: sk_\n      storage: Secret is shown once at creation and stored only as a hash.\n    token:\n      type: bearer\n      in: header\n      header: authorization\n     \
  \ lifetime: 3600            # documented as \"tokens last an hour\"\n    rotation: >-\n      Rotating a key keeps the old secret working for 24 hours so it can be rolled out\n      without taking customers offline.\n    availability:\n      gated: true\n      requirement: Paid Fleet plan - the key page unlocks once the account is on Fleet.\n    scope_selection: >-\n      Scopes are chosen at key creation, so a key that provisions and deploys need not be\n      able to delete.\nx-evidence:\n  fetched: '2026-08-09'\n  probed:\n    - url: https://www.spocket.dev/documentation/platform-api\n      status: 200\n    - url: https://www.spocket.dev/.well-known/oauth-authorization-server\n      status: 200\n    - url: https://www.spocket.dev/.well-known/oauth-protected-resource\n      status: 200\n    - url: https://www.spocket.dev/api/mcp\n      status: 401\n    - url: https://www.spocket.dev/.well-known/openid-configuration\n      status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spocket/refs/heads/main/authentication/spocket-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- PaaS
- application-hosting
- bot-hosting
- developer-tools
- agent-infrastructure
- MCP
- deployment
- serverless
- always-on
---
