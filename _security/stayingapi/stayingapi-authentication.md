---
api_key_in:
- header
api_specs:
- filename: stayingapi-account-api-openapi.yml
  format: yaml
  label: StayingAPI Account API
  slug: stayingapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-account-api-openapi.yml
- filename: stayingapi-data-api-openapi.yml
  format: yaml
  label: StayingAPI Data API
  slug: stayingapi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-data-api-openapi.yml
- filename: stayingapi-jobs-api-openapi.yml
  format: yaml
  label: StayingAPI Jobs API
  slug: stayingapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-jobs-api-openapi.yml
auth_types:
- http
- oauth2
description: StayingAPI runs two distinct auth surfaces. The REST API at api.stayingapi.com/v1 uses a Bearer API key with an environment-encoding prefix (stay_test_ = deterministic sandbox, stay_live_ = live). The hosted MCP server at mcp.stayingapi.com/mcp uses OAuth 2.1 with PKCE (S256) and dynamic client registration, advertised through RFC 8414 authorization server metadata and RFC 9728 protected-resource metadata. Both draw on the same account and the same single credit balance.
kind: authentication
layout: security
method: searched
name: Stayingapi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: StayingAPI secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: StayingAPI
provider_slug: stayingapi
scheme_count: 2
schemes:
- description: 'Bearer API key sent as `Authorization: Bearer <key>`. stay_test_ = deterministic sandbox (0 credits, synchronous); stay_live_ = live.'
  key_prefixes:
  - stay_test_
  - stay_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/stayingapi-openapi-original.json
  - https://stayingapi.com/docs/authentication
  surface: REST
  type: http
- description: OAuth 2.1 authorization code + PKCE (S256) with dynamic client registration for the hosted MCP server. Not declared in the REST OpenAPI; discovered from the live /.well-known metadata on mcp.stayingapi.com.
  flows:
  - authorizationUrl: https://mcp.stayingapi.com/mcp/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    issuer: https://mcp.stayingapi.com/mcp/oauth
    registrationUrl: https://mcp.stayingapi.com/mcp/oauth/register
    scopes:
    - stays.read
    tokenUrl: https://mcp.stayingapi.com/mcp/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_basic
  name: mcpOAuth
  sources:
  - well-known/stayingapi-oauth-authorization-server.json
  - well-known/stayingapi-oauth-protected-resource.json
  - https://stayingapi.com/docs/mcp
  surface: MCP
  type: oauth2
slug: stayingapi-authentication
source_filename: stayingapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/stayingapi-openapi-original.json\ndocs: https://stayingapi.com/docs/authentication\ndescription: >-\n  StayingAPI runs two distinct auth surfaces. The REST API at api.stayingapi.com/v1 uses a\n  Bearer API key with an environment-encoding prefix (stay_test_ = deterministic sandbox,\n  stay_live_ = live). The hosted MCP server at mcp.stayingapi.com/mcp uses OAuth 2.1 with\n  PKCE (S256) and dynamic client registration, advertised through RFC 8414 authorization\n  server metadata and RFC 9728 protected-resource metadata. Both draw on the same account\n  and the same single credit balance.\nsummary:\n  types:\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    surface: REST\n    description: >-\n      Bearer API key sent as `Authorization: Bearer <key>`. stay_test_ = deterministic\n      sandbox (0 credits,\
  \ synchronous); stay_live_ = live.\n    key_prefixes:\n      - stay_test_\n      - stay_live_\n    sources:\n      - openapi/stayingapi-openapi-original.json\n      - https://stayingapi.com/docs/authentication\n  - name: mcpOAuth\n    type: oauth2\n    surface: MCP\n    description: >-\n      OAuth 2.1 authorization code + PKCE (S256) with dynamic client registration for the\n      hosted MCP server. Not declared in the REST OpenAPI; discovered from the live\n      /.well-known metadata on mcp.stayingapi.com.\n    flows:\n      - flow: authorizationCode\n        issuer: https://mcp.stayingapi.com/mcp/oauth\n        authorizationUrl: https://mcp.stayingapi.com/mcp/oauth/authorize\n        tokenUrl: https://mcp.stayingapi.com/mcp/oauth/token\n        registrationUrl: https://mcp.stayingapi.com/mcp/oauth/register\n        code_challenge_methods:\n          - S256\n        token_endpoint_auth_methods:\n          - none\n          - client_secret_basic\n        scopes:\n          - stays.read\n\
  \    sources:\n      - well-known/stayingapi-oauth-authorization-server.json\n      - well-known/stayingapi-oauth-protected-resource.json\n      - https://stayingapi.com/docs/mcp\nkey_management:\n  dashboard: https://stayingapi.com/dashboard/keys\n  rotation: Keys can be created, labelled, rotated and revoked from the dashboard.\n  storage: Secret is displayed once at creation and stored only as a hash.\n  revocation: Revoked keys immediately return 401 revoked_api_key.\n  verification_gate: >-\n    Live credits are unusable until account email is verified; a 403 permission_denied /\n    email_unverified is returned until then. Sandbox keys work throughout.\nx-evidence:\n  - url: https://api.stayingapi.com/openapi.json\n    http_status: 200\n    note: components.securitySchemes.bearerAuth\n  - url: https://mcp.stayingapi.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.stayingapi.com/.well-known/oauth-protected-resource\n    http_status: 200\n  -\
  \ url: https://mcp.stayingapi.com/mcp\n    http_status: 401\n    note: >-\n      WWW-Authenticate: Bearer resource_metadata=\"https://mcp.stayingapi.com/mcp/.well-known/oauth-protected-resource\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/authentication/stayingapi-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- travel
- hospitality
- accommodation-data
- hotel-api
- vacation-rental
- short-term-rental
- airbnb
- booking.com
- vrbo
- google-hotels
- cross-ota-price-comparison
- Availability
- Reviews
- rest
- MCP
- agent-native
- OpenAPI
---
