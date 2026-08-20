---
api_key_in:
- header
api_specs:
- filename: sybilion-operational-api-openapi.yml
  format: yaml
  label: Sybilion Operational API
  slug: sybilion-operational-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-operational-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sybilion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sybilion secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sybilion
provider_slug: sybilion
scheme_count: 3
schemes:
- accepted_credentials:
  - env_var: SYBILION_API_TOKEN
    expiry: not published
    issuance: Developers Portal -> API keys
    kind: api_key
    note: Opaque key, no scopes, no per-key permissions. One key grants the full account surface including billing history and balance.
    prefix: sk_ops_
    retrievable_later: false
    revocable: true
    rotation_policy: not published
    shown_once: true
  - audience: sybilion
    format: JWT access token from the Developers Portal session
    issuer: Auth0
    issuer_host: auth0.sybilion.com
    kind: session_token
    note: accepted on the same Authorization header as the API key
  applies_to: https://api.sybilion.dev
  bearerFormat: null
  failure: 401 with {"error":"missing bearer token","trace_id":"..."}
  header: 'Authorization: Bearer <token>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sybilion-operational-api-openapi.yml
  surface: rest
  type: http
- applies_to: https://mcp.sybilion.dev/mcp
  bearer_methods:
  - header
  challenge: 'WWW-Authenticate: Bearer resource_metadata="https://mcp.sybilion.dev/.well-known/oauth-protected-resource/mcp"'
  discovered_by: probe
  dynamic_client_registration: https://mcp.sybilion.dev/oauth/register
  flows:
  - authorizationUrl: https://mcp.sybilion.dev/oauth/authorize
    flow: authorizationCode
    scopes:
    - openid
    - profile
    - email
    - offline_access
    tokenUrl: https://mcp.sybilion.dev/oauth/token
  jwks_uri: https://sybilion.eu.auth0.com/.well-known/jwks.json
  name: mcp-oauth
  note: No API key is used here. The docs are explicit that an MCP client runs the browser approval flow and that there is nothing to paste into the connector config. The server implements both RFC 8414 and RFC 9728 discovery plus RFC 7591 dynamic client registration, which is a materially better OAuth posture than the REST side's opaque static key.
  pkce:
  - S256
  - plain
  revocation: https://mcp.sybilion.dev/oauth/revoke
  sources:
  - https://mcp.sybilion.dev/.well-known/oauth-authorization-server
  - https://mcp.sybilion.dev/.well-known/oauth-protected-resource
  - https://sybilion.dev/docs/integrations
  surface: mcp
  type: oauth2
- applies_to: https://sybilion.dev
  discovered_by: probe
  name: portal-oidc
  note: Auth0 custom domain backing the Developers Portal login. Not an API credential surface in its own right, but it is the issuer of the session tokens the REST API accepts.
  openIdConnectUrl: https://auth0.sybilion.com/.well-known/openid-configuration
  sources:
  - well-known/sybilion-openid-configuration.json
  surface: portal
  type: openIdConnect
slug: sybilion-authentication
source_filename: sybilion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://sybilion.dev/docs/authentication\nderived_from: openapi/sybilion-operational-api-openapi.yml\ndocs: https://sybilion.dev/docs/authentication\nnote: >-\n  The OpenAPI declares exactly one scheme (http bearer, no bearerFormat) applied to all ten\n  /api/v1/* operations, with /health left unsecured. The docs are richer than the spec: they\n  distinguish THREE credential kinds behind that one header, and they describe a second, entirely\n  separate OAuth surface on the MCP server that the OpenAPI does not mention at all.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  surfaces: 2\n  unauthenticated_operations: ['GET /health']\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: null\n    surface: rest\n    applies_to: https://api.sybilion.dev\n    sources: [openapi/sybilion-operational-api-openapi.yml]\n    header:\
  \ 'Authorization: Bearer <token>'\n    accepted_credentials:\n      - kind: api_key\n        prefix: sk_ops_\n        issuance: Developers Portal -> API keys\n        shown_once: true\n        retrievable_later: false\n        revocable: true\n        rotation_policy: not published\n        expiry: not published\n        env_var: SYBILION_API_TOKEN\n        note: >-\n          Opaque key, no scopes, no per-key permissions. One key grants the full account surface\n          including billing history and balance.\n      - kind: session_token\n        issuer: Auth0\n        issuer_host: auth0.sybilion.com\n        format: JWT access token from the Developers Portal session\n        audience: sybilion\n        note: accepted on the same Authorization header as the API key\n    failure: 401 with {\"error\":\"missing bearer token\",\"trace_id\":\"...\"}\n  - name: mcp-oauth\n    type: oauth2\n    surface: mcp\n    applies_to: https://mcp.sybilion.dev/mcp\n    sources:\n      - https://mcp.sybilion.dev/.well-known/oauth-authorization-server\n\
  \      - https://mcp.sybilion.dev/.well-known/oauth-protected-resource\n      - https://sybilion.dev/docs/integrations\n    discovered_by: probe\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.sybilion.dev/oauth/authorize\n        tokenUrl: https://mcp.sybilion.dev/oauth/token\n        scopes: [openid, profile, email, offline_access]\n    pkce: [S256, plain]\n    dynamic_client_registration: https://mcp.sybilion.dev/oauth/register\n    revocation: https://mcp.sybilion.dev/oauth/revoke\n    jwks_uri: https://sybilion.eu.auth0.com/.well-known/jwks.json\n    bearer_methods: [header]\n    challenge: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.sybilion.dev/.well-known/oauth-protected-resource/mcp\"'\n    note: >-\n      No API key is used here. The docs are explicit that an MCP client runs the browser approval\n      flow and that there is nothing to paste into the connector config. The server implements both\n      RFC 8414 and RFC 9728 discovery\
  \ plus RFC 7591 dynamic client registration, which is a\n      materially better OAuth posture than the REST side's opaque static key.\n  - name: portal-oidc\n    type: openIdConnect\n    surface: portal\n    applies_to: https://sybilion.dev\n    openIdConnectUrl: https://auth0.sybilion.com/.well-known/openid-configuration\n    sources: [well-known/sybilion-openid-configuration.json]\n    discovered_by: probe\n    note: >-\n      Auth0 custom domain backing the Developers Portal login. Not an API credential surface in its\n      own right, but it is the issuer of the session tokens the REST API accepts.\ngaps:\n  - The OpenAPI gives bearerAuth no bearerFormat and no description, so a generated client cannot tell an sk_ops_ key from a JWT.\n  - No scopes, roles or per-key permissions exist on the REST surface; the key is all-or-nothing.\n  - Key rotation, expiry and maximum key count are not documented.\n  - The MCP OAuth surface is absent from the OpenAPI entirely and is only discoverable\
  \ by probing /.well-known/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/authentication/sybilion-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Industrial market intelligence
- Commodity price forecasting
- Economic Forecasting
- Time-series forecasting
- Procurement
- Supply Chain Risk
- Trading analytics
- AI decision support
- MCP
- agent-native
- Causal Inference
- Anomaly Detection
---
