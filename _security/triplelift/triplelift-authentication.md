---
api_key_in: []
auth_types: []
description: TripleLift runs three distinct authentication regimes across its API surface. The Reporting API uses a paired static API key plus a monthly-rotating JWT, both sent as headers on every request. The TripleLift platform (app.triplelift.com and the federated GraphQL gateway) uses an Auth0 OpenID Connect tenant with authorization_code + PKCE and a large scope catalog. The TLX exchange endpoint is not authenticated with a credential at all — a supplier is identified by a supplier_id query parameter issued during onboarding and by IP/host allowlisting.
kind: authentication
layout: security
method: searched
name: Triplelift Authentication
name_suffix: Authentication
oauth_flows: []
overview: TripleLift declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: TripleLift
provider_slug: triplelift
scheme_count: 5
schemes:
- api: TripleLift Reporting API
  description: Static API key unique to the TripleLift member account. Does not expire, but is invalidated whenever a new key is generated — and generating a new key rotates it for EVERY user and program querying on behalf of that member account, so key rotation is an account-wide breaking event with no per-client isolation.
  id: reporting-api-key
  in: header
  name: X-API-Key
  obtain:
  - method: console
    steps: Reporting menu -> Reporting API -> "Current API Key" -> copy, or Generate New Key.
    url: https://console.triplelift.com
  - body: '{"id": "<member id>", "overwriteExistingKey": true}'
    endpoint: POST https://reporting-api.triplelift.net/generate-api-key
    headers:
    - 'X-API-Key: <current key>'
    - 'Authorization: Bearer <jwt>'
    method: api
    note: Requires the existing key and a valid JWT — there is no unauthenticated bootstrap.
  required: true
  type: apiKey
- api: TripleLift Reporting API
  bearerFormat: JWT
  description: JSON Web Token that expires after one month and must be refreshed. Sent alongside — not instead of — the X-API-Key header; both are required on every request.
  id: reporting-jwt
  in: header
  lifetime: 1 month
  name: Authorization
  obtain:
  - method: console
    steps: Reporting menu -> Reporting API -> "Current Token".
    url: https://console.triplelift.com
  - body: '{"username": "<username>", "password": "<password>"}'
    endpoint: POST https://api.triplelift.com/login
    method: api
    note: Resource-owner password credentials over a plain JSON POST. There is no client_credentials or service-account flow published for the Reporting API, so an automated integration must store a human user's password to refresh its token every month.
    response_field: reporting_api_token
  refresh: none published — re-POST /login
  required: true
  scheme: bearer
  type: http
- api: TripleLift Platform (app.triplelift.com, federated-api.prod.triplelift.net)
  audience: https://federated-api.prod.triplelift.net
  description: Discovered by probing, not from documentation — TripleLift publishes no developer documentation for the platform API. app.triplelift.com 302s to the Auth0 authorize endpoint and the redirect exposes the client_id, the audience and the complete scope catalog.
  documented: false
  dpop_signing_alg_values_supported:
  - ES256
  flows:
    authorizationCode:
      authorizationUrl: https://auth.triplelift.net/authorize
      pkce: S256
      refreshUrl: https://auth.triplelift.net/oauth/token
      tokenUrl: https://auth.triplelift.net/oauth/token
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: platform-oidc
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.triplelift.net/
  jwks_uri: https://auth.triplelift.net/.well-known/jwks.json
  openIdConnectUrl: https://auth.triplelift.net/.well-known/openid-configuration
  provider: Auth0
  registration_endpoint: https://auth.triplelift.net/oidc/register
  revocation_endpoint: https://auth.triplelift.net/oauth/revoke
  scopes: see scopes/triplelift-scopes.yml
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- api: TripleLift WordPress MCP server
  description: A second, entirely separate OAuth authorization server on the marketing domain, serving only the WordPress MCP endpoint. Unrelated to the platform Auth0 tenant.
  dynamic_client_registration: client_id_metadata_document
  flows:
    authorizationCode:
      authorizationUrl: https://triplelift.com/oauth/authorize
      pkce: S256
      refreshUrl: https://triplelift.com/oauth/token
      tokenUrl: https://triplelift.com/oauth/token
  id: mcp-oauth-wordpress
  issuer: https://triplelift.com
  metadata: https://triplelift.com/.well-known/oauth-authorization-server
  protected_resource: https://triplelift.com/wp-json/mcp/mcp-oauth-server
  scopes:
    mcp: Access the MCP server exposed by the triplelift.com WordPress site.
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- api: TripleLift Exchange (TLX)
  description: The server-to-server OpenRTB endpoint carries no Authorization header. A supply partner is identified by the supplier_id query parameter TripleLift issues at onboarding — https://tlx.3lift.com/s2s/auction?supplier_id=123 — with access otherwise controlled out of band by the partner agreement and allowlisting. User-sync endpoints on eb2.3lift.com use a mid + dongle parameter pair for the same purpose.
  docs: https://docs.triplelift.com/docs/supply-partners
  documented: true
  id: tlx-supplier-id
  type: none
slug: triplelift-authentication
source_filename: triplelift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: TripleLift Authentication\ndescription: >-\n  TripleLift runs three distinct authentication regimes across its API surface.\n  The Reporting API uses a paired static API key plus a monthly-rotating JWT, both\n  sent as headers on every request. The TripleLift platform (app.triplelift.com and\n  the federated GraphQL gateway) uses an Auth0 OpenID Connect tenant with\n  authorization_code + PKCE and a large scope catalog. The TLX exchange endpoint\n  is not authenticated with a credential at all — a supplier is identified by a\n  supplier_id query parameter issued during onboarding and by IP/host allowlisting.\ngenerated: '2026-08-12'\nmethod: searched\nsource: https://supply-docs.triplelift.com/reference/authorization\nschemes:\n  - id: reporting-api-key\n    api: TripleLift Reporting API\n    type: apiKey\n    in: header\n    name: X-API-Key\n    required: true\n    description: >-\n      Static API key unique to the TripleLift member account. Does not expire, but\n \
  \     is invalidated whenever a new key is generated — and generating a new key\n      rotates it for EVERY user and program querying on behalf of that member\n      account, so key rotation is an account-wide breaking event with no per-client\n      isolation.\n    obtain:\n      - method: console\n        url: https://console.triplelift.com\n        steps: Reporting menu -> Reporting API -> \"Current API Key\" -> copy, or Generate New Key.\n      - method: api\n        endpoint: POST https://reporting-api.triplelift.net/generate-api-key\n        headers:\n          - 'X-API-Key: <current key>'\n          - 'Authorization: Bearer <jwt>'\n        body: '{\"id\": \"<member id>\", \"overwriteExistingKey\": true}'\n        note: Requires the existing key and a valid JWT — there is no unauthenticated bootstrap.\n  - id: reporting-jwt\n    api: TripleLift Reporting API\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    name: Authorization\n    required: true\n \
  \   description: >-\n      JSON Web Token that expires after one month and must be refreshed. Sent\n      alongside — not instead of — the X-API-Key header; both are required on\n      every request.\n    obtain:\n      - method: console\n        url: https://console.triplelift.com\n        steps: Reporting menu -> Reporting API -> \"Current Token\".\n      - method: api\n        endpoint: POST https://api.triplelift.com/login\n        body: '{\"username\": \"<username>\", \"password\": \"<password>\"}'\n        response_field: reporting_api_token\n        note: >-\n          Resource-owner password credentials over a plain JSON POST. There is no\n          client_credentials or service-account flow published for the Reporting\n          API, so an automated integration must store a human user's password to\n          refresh its token every month.\n    lifetime: 1 month\n    refresh: none published — re-POST /login\n  - id: platform-oidc\n    api: TripleLift Platform (app.triplelift.com,\
  \ federated-api.prod.triplelift.net)\n    type: openIdConnect\n    openIdConnectUrl: https://auth.triplelift.net/.well-known/openid-configuration\n    issuer: https://auth.triplelift.net/\n    provider: Auth0\n    flows:\n      authorizationCode:\n        authorizationUrl: https://auth.triplelift.net/authorize\n        tokenUrl: https://auth.triplelift.net/oauth/token\n        refreshUrl: https://auth.triplelift.net/oauth/token\n        pkce: S256\n    audience: https://federated-api.prod.triplelift.net\n    grant_types_supported:\n      - client_credentials\n      - authorization_code\n      - refresh_token\n      - password\n      - implicit\n      - 'urn:ietf:params:oauth:grant-type:device_code'\n      - 'urn:ietf:params:oauth:grant-type:token-exchange'\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - none\n    id_token_signing_alg_values_supported:\n\
  \      - HS256\n      - RS256\n      - PS256\n    jwks_uri: https://auth.triplelift.net/.well-known/jwks.json\n    dpop_signing_alg_values_supported:\n      - ES256\n    revocation_endpoint: https://auth.triplelift.net/oauth/revoke\n    registration_endpoint: https://auth.triplelift.net/oidc/register\n    scopes: see scopes/triplelift-scopes.yml\n    description: >-\n      Discovered by probing, not from documentation — TripleLift publishes no\n      developer documentation for the platform API. app.triplelift.com 302s to the\n      Auth0 authorize endpoint and the redirect exposes the client_id, the audience\n      and the complete scope catalog.\n    documented: false\n  - id: mcp-oauth-wordpress\n    api: TripleLift WordPress MCP server\n    type: oauth2\n    issuer: https://triplelift.com\n    metadata: https://triplelift.com/.well-known/oauth-authorization-server\n    protected_resource: https://triplelift.com/wp-json/mcp/mcp-oauth-server\n    flows:\n      authorizationCode:\n  \
  \      authorizationUrl: https://triplelift.com/oauth/authorize\n        tokenUrl: https://triplelift.com/oauth/token\n        refreshUrl: https://triplelift.com/oauth/token\n        pkce: S256\n    scopes:\n      mcp: Access the MCP server exposed by the triplelift.com WordPress site.\n    token_endpoint_auth_methods_supported:\n      - none\n    dynamic_client_registration: client_id_metadata_document\n    description: >-\n      A second, entirely separate OAuth authorization server on the marketing\n      domain, serving only the WordPress MCP endpoint. Unrelated to the platform\n      Auth0 tenant.\n  - id: tlx-supplier-id\n    api: TripleLift Exchange (TLX)\n    type: none\n    description: >-\n      The server-to-server OpenRTB endpoint carries no Authorization header. A\n      supply partner is identified by the supplier_id query parameter TripleLift\n      issues at onboarding — https://tlx.3lift.com/s2s/auction?supplier_id=123 —\n      with access otherwise controlled out of band\
  \ by the partner agreement and\n      allowlisting. User-sync endpoints on eb2.3lift.com use a mid + dongle\n      parameter pair for the same purpose.\n    documented: true\n    docs: https://docs.triplelift.com/docs/supply-partners\nobservations:\n  - No API surface at TripleLift uses a single credential. Every authenticated\n    surface requires either two headers (Reporting) or a full OIDC round trip\n    (platform).\n  - The Reporting API's account-wide key rotation and its password-grant JWT\n    refresh are the two weakest points in the auth design for automated agents.\n  - There is no published machine-readable security scheme document (no OpenAPI,\n    no oauth-protected-resource metadata on the API hosts), so an agent cannot\n    discover any of this without reading the human docs.\nx-evidence:\n  - url: https://supply-docs.triplelift.com/reference/authorization.md\n    http_status: 200\n    fetched: '2026-08-12'\n  - url: https://auth.triplelift.net/.well-known/openid-configuration\n\
  \    http_status: 200\n    fetched: '2026-08-12'\n  - url: https://triplelift.com/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-12'\n  - url: https://app.triplelift.com/\n    http_status: 302\n    fetched: '2026-08-12'\n    note: Location header names the Auth0 authorize endpoint, audience and scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triplelift/refs/heads/main/authentication/triplelift-authentication.yml
summary_line: 5 schemes
tags:
- Programmatic Advertising
- Native Advertising
- Ad Exchange
- OpenRTB
- Header Bidding
- Connected TV
- Supply Side Platform
- Demand Side Platform
- GraphQL
- Ad Tech
- Publisher Reporting
- Real-Time Bidding
---
