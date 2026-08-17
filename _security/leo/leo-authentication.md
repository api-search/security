---
api_key_in: []
api_specs:
- filename: leo-prospects-api-openapi.yml
  format: yaml
  label: LeO Public API
  slug: leo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/openapi/leo-prospects-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Leo Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeO secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeO
provider_slug: leo
scheme_count: 2
schemes:
- applies_to: every operation except GET /health
  bearerFormat: JWT
  header: Authorization
  in: header
  name: bearer
  scheme: bearer
  source: openapi/_original/leo-openapi.json
  sources:
  - openapi/leo-account-api-openapi.yml
  - openapi/leo-credits-api-openapi.yml
  - openapi/leo-jobs-api-openapi.yml
  - openapi/leo-prospects-api-openapi.yml
  surface: REST
  type: http
  unauthenticated_response:
    description: Unauthorized (declared on every secured operation in the spec)
    status: 401
- authorization_endpoint: https://insights-app-auth.meetleo.com/oauth2/authorize
  dynamic_client_registration: false
  flow: authorization_code
  header: Authorization
  identity_provider: AWS Cognito (us-east-1_RnOkUWIRc)
  in: header
  issuer: https://mcp.meetleo.com
  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_RnOkUWIRc/.well-known/jwks.json
  name: oauth2-mcp
  pkce: S256
  resource: https://mcp.meetleo.com
  revocation_endpoint: https://insights-app-auth.meetleo.com/oauth2/revoke
  scopes: scopes/leo-scopes.yml
  source: https://mcp.meetleo.com/.well-known/oauth-protected-resource
  surface: MCP
  token_endpoint: https://insights-app-auth.meetleo.com/oauth2/token
  type: oauth2
  unauthenticated_response:
    body: '{"jsonrpc":"2.0","error":{"code":-32001,"message":"Authentication required. Provide a token via the Authorization header."},"id":null}'
    probed: '2026-08-14'
    status: 401
    www_authenticate: Bearer resource_metadata="https://mcp.meetleo.com/.well-known/oauth-protected-resource"
slug: leo-authentication
source_filename: leo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  openapi/_original/leo-openapi.json (https://api.meetleo.com/openapi.json),\n  https://mcp.meetleo.com/.well-known/oauth-protected-resource,\n  https://mcp.meetleo.com/.well-known/oauth-authorization-server,\n  live 401 challenge from https://mcp.meetleo.com/mcp\ndocs: https://api.meetleo.com/docs\nnotes: >-\n  LeO runs two authenticated surfaces with the same identity provider behind them.\n  The REST API at https://api.meetleo.com declares a single HTTP bearer scheme\n  carrying a JWT, applied per-operation to every path except GET /health. The MCP\n  Connector at https://mcp.meetleo.com/mcp is OAuth 2.1-shaped: an unauthenticated\n  JSON-RPC call returns HTTP 401 with a WWW-Authenticate header pointing at RFC\n  9728 protected-resource metadata, which in turn names an AWS Cognito user pool\n  (us-east-1_RnOkUWIRc) fronted by https://insights-app-auth.meetleo.com. No API\n  key, mTLS or basic-auth surface was found. There\
  \ is no public self-service\n  credential issuance: LeO's own MCP page states the connector \"authenticates\n  against your existing tenant and respects your entitlements and credit balance\",\n  and account entitlement flags hasApiAccess / hasMcpAccess gate access per plan.\nsummary:\n  types:\n  - http\n  - oauth2\n  primary: bearer JWT\n  credential_issuance: account-gated (no public self-service key page found)\nschemes:\n- name: bearer\n  surface: REST\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  applies_to: every operation except GET /health\n  source: openapi/_original/leo-openapi.json\n  sources:\n  - openapi/leo-account-api-openapi.yml\n  - openapi/leo-credits-api-openapi.yml\n  - openapi/leo-jobs-api-openapi.yml\n  - openapi/leo-prospects-api-openapi.yml\n  unauthenticated_response:\n    status: 401\n    description: Unauthorized (declared on every secured operation in the spec)\n- name: oauth2-mcp\n  surface: MCP\n  type: oauth2\n\
  \  flow: authorization_code\n  pkce: S256\n  in: header\n  header: Authorization\n  resource: https://mcp.meetleo.com\n  issuer: https://mcp.meetleo.com\n  authorization_endpoint: https://insights-app-auth.meetleo.com/oauth2/authorize\n  token_endpoint: https://insights-app-auth.meetleo.com/oauth2/token\n  revocation_endpoint: https://insights-app-auth.meetleo.com/oauth2/revoke\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_RnOkUWIRc/.well-known/jwks.json\n  identity_provider: AWS Cognito (us-east-1_RnOkUWIRc)\n  dynamic_client_registration: false\n  scopes: scopes/leo-scopes.yml\n  source: https://mcp.meetleo.com/.well-known/oauth-protected-resource\n  unauthenticated_response:\n    status: 401\n    body: >-\n      {\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Authentication required.\n      Provide a token via the Authorization header.\"},\"id\":null}\n    www_authenticate: >-\n      Bearer resource_metadata=\"https://mcp.meetleo.com/.well-known/oauth-protected-resource\"\
  \n    probed: '2026-08-14'\nentitlements:\n- field: plan.hasApiAccess\n  schema: PlanDto\n  description: Whether the authenticated account's plan permits REST API access.\n  source: openapi/leo-account-api-openapi.yml\n- field: plan.hasMcpAccess\n  schema: PlanDto\n  description: Whether the authenticated account's plan permits MCP Connector access.\n  source: openapi/leo-account-api-openapi.yml\ngaps:\n- >-\n  No published developer-portal page documents how to obtain a REST bearer token;\n  the Swagger UI at https://api.meetleo.com/docs presents the scheme but not the\n  issuance flow. Credentials appear to be issued through the application or by\n  sales.\n- >-\n  No RFC 7591 dynamic client registration endpoint (POST /register returns 404),\n  so an MCP client cannot self-register.\n- No /.well-known/security.txt is served on any LeO host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/authentication/leo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Insurance
- Commercial Insurance
- Property and Casualty
- Employee Benefits
- Insurtech
- Artificial Intelligence
- Sales
- Lead Generation
- Prospecting
- Data Enrichment
- Sales Intelligence
- Nonprofits
- Trucking
- MCP
- Agent Native
---
