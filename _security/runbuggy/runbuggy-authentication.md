---
api_key_in:
- header
api_specs:
- filename: runbuggy-companies-api-openapi.yml
  format: yaml
  label: RunBuggy Companies API
  slug: runbuggy-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-companies-api-openapi.yml
- filename: runbuggy-orders-api-openapi.yml
  format: yaml
  label: RunBuggy Orders API
  slug: runbuggy-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-orders-api-openapi.yml
- filename: runbuggy-token-api-openapi.yml
  format: yaml
  label: RunBuggy Token API
  slug: runbuggy-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-token-api-openapi.yml
- filename: runbuggy-vehicle-transfer-orders-api-openapi.yml
  format: yaml
  label: RunBuggy Vehicle Transfer Orders API
  slug: runbuggy-vehicle-transfer-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-vehicle-transfer-orders-api-openapi.yml
- filename: runbuggy-webhooks-api-openapi.yml
  format: yaml
  label: RunBuggy Webhooks API
  slug: runbuggy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: 'RunBuggy runs three distinct authentication models across its estate, and only the first is described in a specification: an opaque bearer token for the REST Shippers API, a short-lived scope=openid JWT for the embeddable order-status iframe, and full OAuth 2.1 with dynamic client registration and PKCE for the mcp-datascience MCP server.'
kind: authentication
layout: security
method: searched
name: Runbuggy Authentication
name_suffix: Authentication
oauth_flows: []
overview: RunBuggy secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RunBuggy
provider_slug: runbuggy
scheme_count: 3
schemes:
- acquisition:
    documented_path: Contact your RunBuggy representative to retrieve a Bearer token.
    operationId: login
    programmatic: POST /login on the Authentication API (base https://ng-staging.runbuggy.com/staging/api/auth) returns a login-response carrying the token.
    self_service: false
  applied_to: all 28 published operations, uniformly
  description: See the [Authentication Guide](/docs/shipping/b6b6c2d4906e9-authentication).
  expiry: not documented
  format: Bearer {token}
  in: header
  name: Authorization
  note: Declared as `apiKey` rather than Swagger 2.0's http/bearer style, so generated clients treat the whole "Bearer {token}" string as the key value. Callers must include the literal "Bearer " prefix themselves.
  parameter: Authorization
  rotation: not documented
  sources:
  - openapi/runbuggy-companies.json
  - openapi/runbuggy-orders.json
  surface: REST Shippers API (Orders, Companies)
  type: apiKey
- documented_expiry_seconds: 60
  flow: token exchange — an authenticated API bearer token is POSTed to the platform oauth2/token endpoint with body {"scope":"openid"} to mint a JWT
  name: order-status-jwt
  note: Not present in any published specification — the endpoint is documented only in prose. The documented pattern moves a bearer credential through a URL query string.
  passed_in: URL query parameter `token` on the iframe src
  source: https://docs.runbuggy.com/docs/shipping/d483faef38c3b-embedding-i-frame-order-status
  surface: embeddable order-status iframe
  token_type: JWT
  type: oauth2
- authorization_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/authorize
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://apps.runbuggy.com/runbuggy/mcp-datascience
  metadata_file: well-known/runbuggy-oauth-authorization-server.json
  name: mcp-oauth
  note: The most modern auth in the estate, and the one RunBuggy documents least — it appears nowhere on runbuggy.com or docs.runbuggy.com.
  registration_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/register
  revocation_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/revoke
  scopes_supported: null
  spec: OAuth 2.1 authorization code with PKCE (S256) and RFC 7591 dynamic client registration
  surface: RunBuggy Data Science MCP server
  token_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: runbuggy-authentication
source_filename: runbuggy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://docs.runbuggy.com/docs/shipping/b6b6c2d4906e9-authentication, openapi/runbuggy-orders.json,\n  openapi/runbuggy-authentication.json, well-known/runbuggy-oauth-authorization-server.json\ndocs: https://docs.runbuggy.com/docs/shipping/b6b6c2d4906e9-authentication\ndescription: 'RunBuggy runs three distinct authentication models across its estate, and\n  only the first is described in a specification: an opaque bearer token for the REST\n  Shippers API, a short-lived scope=openid JWT for the embeddable order-status iframe,\n  and full OAuth 2.1 with dynamic client registration and PKCE for the mcp-datascience\n  MCP server.'\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  surface: REST Shippers API (Orders, Companies)\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Bearer {token}\n  description: See the [Authentication Guide](/docs/shipping/b6b6c2d4906e9-authentication).\n\
  \  sources:\n  - openapi/runbuggy-companies.json\n  - openapi/runbuggy-orders.json\n  acquisition:\n    self_service: false\n    documented_path: Contact your RunBuggy representative to retrieve a Bearer token.\n    programmatic: POST /login on the Authentication API (base https://ng-staging.runbuggy.com/staging/api/auth)\n      returns a login-response carrying the token.\n    operationId: login\n  applied_to: all 28 published operations, uniformly\n  rotation: not documented\n  expiry: not documented\n  note: Declared as `apiKey` rather than Swagger 2.0's http/bearer style, so generated\n    clients treat the whole \"Bearer {token}\" string as the key value. Callers must\n    include the literal \"Bearer \" prefix themselves.\n- name: order-status-jwt\n  surface: embeddable order-status iframe\n  type: oauth2\n  flow: token exchange — an authenticated API bearer token is POSTed to the platform\n    oauth2/token endpoint with body {\"scope\":\"openid\"} to mint a JWT\n  token_type: JWT\n\
  \  documented_expiry_seconds: 60\n  passed_in: URL query parameter `token` on the iframe src\n  source: https://docs.runbuggy.com/docs/shipping/d483faef38c3b-embedding-i-frame-order-status\n  note: Not present in any published specification — the endpoint is documented only in\n    prose. The documented pattern moves a bearer credential through a URL query string.\n- name: mcp-oauth\n  surface: RunBuggy Data Science MCP server\n  type: oauth2\n  spec: OAuth 2.1 authorization code with PKCE (S256) and RFC 7591 dynamic client\n    registration\n  issuer: https://apps.runbuggy.com/runbuggy/mcp-datascience\n  authorization_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/authorize\n  token_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/token\n  registration_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/register\n  revocation_endpoint: https://apps.runbuggy.com/runbuggy/mcp-datascience/revoke\n  grant_types_supported: [authorization_code, refresh_token]\n\
  \  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  scopes_supported: null\n  metadata_file: well-known/runbuggy-oauth-authorization-server.json\n  note: The most modern auth in the estate, and the one RunBuggy documents least — it\n    appears nowhere on runbuggy.com or docs.runbuggy.com.\nmfa:\n  end_user: RunBuggy's security page describes replacing passwords with immutable\n    credentials backed by device-TPM private keys (a phishing-resistant model) for\n    platform users. This applies to the application, not to API tokens.\n  source: https://runbuggy.com/security/\ngaps:\n- No self-service credential issuance for the REST API — every integration begins with a\n  human at RunBuggy.\n- No documented token lifetime, rotation or revocation for the REST bearer token.\n- No scopes on the REST API; a token is all-or-nothing across order creation,\n  cancellation and webhook management.\n- The iframe token exchange endpoint is undocumented in any specification.\n\
  - The MCP OAuth server publishes no scopes_supported and its protected-resource metadata\n  is unreachable.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://docs.runbuggy.com/docs/shipping/b6b6c2d4906e9-authentication\n    http_status: 200\n  - url: https://apps.runbuggy.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://apps.runbuggy.com/runbuggy/mcp-datascience/mcp\n    http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/authentication/runbuggy-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Automotive
- Logistics
- Transportation
- Vehicle Shipping
- Marketplace
- Supply Chain
- Fleet
- TMS
- Freight
---
