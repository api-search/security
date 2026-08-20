---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Stackadapt Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: StackAdapt secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: StackAdapt
provider_slug: stackadapt
scheme_count: 4
schemes:
- applies_to: https://api.stackadapt.com/service/v2
  in: header
  method: searched
  name: RestApiKey
  note: Read-only reporting REST API (v2). Write operations are deprecated in favour of GraphQL.
  parameter_name: X-Authorization
  source: graphql/stackadapt-graphql.md, https://www.stackadapt.com/llms.txt
  type: apiKey
- applies_to: https://api.stackadapt.com/graphql
  method: probed
  name: GraphQLBearer
  note: 'Static GraphQL API key issued by StackAdapt (Account Settings -> API Integration, or via an account manager). Observed behaviour without a token: HTTP 401 with body {"errors":[{"message":"Schema introspection requires authentication.","extensions":{"traceId":"..."}}]} — introspection itself is gated, not only data access.'
  scheme: bearer
  source: live POST to https://api.stackadapt.com/graphql
  type: http
- applies_to: https://mcp.stackadapt.com/
  authorization_server: https://www.stackadapt.com/
  challenge: 'WWW-Authenticate: Bearer error="invalid_token", error_description="Missing Authorization header", resource_metadata="https://mcp.stackadapt.com/.well-known/oauth-protected-resource/"'
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://www.stackadapt.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    refreshUrl: https://www.stackadapt.com/oauth/token
    scopes:
      graphql-public:read: Read access to the GraphQL Public API surface
      graphql-public:write: Write access to the GraphQL Public API surface
    tokenUrl: https://www.stackadapt.com/oauth/token
  - flow: clientCredentials
    scopes:
      graphql-public:read: Read access to the GraphQL Public API surface
      graphql-public:write: Write access to the GraphQL Public API surface
    tokenUrl: https://www.stackadapt.com/oauth/token
  introspection_endpoint: https://www.stackadapt.com/oauth/introspect
  method: probed
  name: MCPOAuth
  registration_endpoint: https://www.stackadapt.com/oauth/register
  resource: https://mcp.stackadapt.com/
  revocation_endpoint: https://www.stackadapt.com/oauth/revoke
  source: https://mcp.stackadapt.com/.well-known/oauth-protected-resource
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- applies_to: https://tags.srv.stackadapt.com/
  in: query
  method: derived
  name: PixelIdentifier
  note: The server-to-server pixel surface is not bearer-authenticated. The caller identifies itself with a StackAdapt-issued pixel identifier passed as a query parameter — sid for retargeting/lookalike endpoints, cid for conversion, uid for the universal pixel.
  parameter_name: sid | cid | uid
  source: https://github.com/StackAdapt/stackadapt-gtm-server-side-pixel (template.tpl)
  type: apiKey
slug: stackadapt-authentication
source_filename: stackadapt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.stackadapt.com/.well-known/oauth-authorization-server (RFC 8414),\n  https://mcp.stackadapt.com/.well-known/oauth-protected-resource (RFC 9728),\n  live 401 challenges from https://api.stackadapt.com/graphql and https://mcp.stackadapt.com/,\n  https://www.stackadapt.com/llms.txt, and graphql/stackadapt-graphql.md in this repo\ndocs: https://docs.stackadapt.com/\nnote: >-\n  Derived without an OpenAPI — StackAdapt publishes no OpenAPI on any host (see x-coverage in\n  apis.yml). Every scheme below is either read from a machine-readable discovery document the\n  provider serves, or observed in a live unauthenticated response.\n\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  key_separation: >-\n    The REST API and the GraphQL API use SEPARATE API keys. StackAdapt's own migration\n    guidance (and every downstream connector that documents\
  \ the change) states the legacy\n    REST key does not work against the GraphQL API.\n\nschemes:\n- name: RestApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-Authorization\n  applies_to: https://api.stackadapt.com/service/v2\n  method: searched\n  source: graphql/stackadapt-graphql.md, https://www.stackadapt.com/llms.txt\n  note: >-\n    Read-only reporting REST API (v2). Write operations are deprecated in favour of GraphQL.\n\n- name: GraphQLBearer\n  type: http\n  scheme: bearer\n  applies_to: https://api.stackadapt.com/graphql\n  method: probed\n  source: live POST to https://api.stackadapt.com/graphql\n  note: >-\n    Static GraphQL API key issued by StackAdapt (Account Settings -> API Integration, or via\n    an account manager). Observed behaviour without a token: HTTP 401 with body\n    {\"errors\":[{\"message\":\"Schema introspection requires authentication.\",\"extensions\":{\"traceId\":\"...\"}}]}\n    — introspection itself is gated, not only data access.\n\n- name:\
  \ MCPOAuth\n  type: oauth2\n  applies_to: https://mcp.stackadapt.com/\n  method: probed\n  source: https://mcp.stackadapt.com/.well-known/oauth-protected-resource\n  resource: https://mcp.stackadapt.com/\n  authorization_server: https://www.stackadapt.com/\n  dynamic_client_registration: true\n  registration_endpoint: https://www.stackadapt.com/oauth/register\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.stackadapt.com/oauth/authorize\n    tokenUrl: https://www.stackadapt.com/oauth/token\n    refreshUrl: https://www.stackadapt.com/oauth/token\n    pkce: [S256, plain]\n    scopes:\n      graphql-public:read: Read access to the GraphQL Public API surface\n      graphql-public:write: Write access to the GraphQL Public API surface\n  - flow: clientCredentials\n    tokenUrl: https://www.stackadapt.com/oauth/token\n    scopes:\n      graphql-public:read: Read access to the GraphQL Public API surface\n      graphql-public:write: Write access to the GraphQL Public API\
  \ surface\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  revocation_endpoint: https://www.stackadapt.com/oauth/revoke\n  introspection_endpoint: https://www.stackadapt.com/oauth/introspect\n  challenge: >-\n    WWW-Authenticate: Bearer error=\"invalid_token\",\n    error_description=\"Missing Authorization header\",\n    resource_metadata=\"https://mcp.stackadapt.com/.well-known/oauth-protected-resource/\"\n\n- name: PixelIdentifier\n  type: apiKey\n  in: query\n  parameter_name: sid | cid | uid\n  applies_to: https://tags.srv.stackadapt.com/\n  method: derived\n  source: https://github.com/StackAdapt/stackadapt-gtm-server-side-pixel (template.tpl)\n  note: >-\n    The server-to-server pixel surface is not bearer-authenticated. The caller identifies\n    itself with a StackAdapt-issued pixel identifier passed as a query parameter — sid for\n    retargeting/lookalike endpoints, cid for conversion, uid for the universal pixel.\n\nenvironments:\n- name: production\n\
  \  issuer: https://api.stackadapt.com\n  authorization_server_metadata: https://api.stackadapt.com/.well-known/oauth-authorization-server\n- name: sandbox\n  issuer: https://sandbox.stackadapt.com\n  authorization_server_metadata: https://sandbox.stackadapt.com/.well-known/oauth-authorization-server\n  note: Sandbox runs its own isolated OAuth issuer; production tokens are not portable to it.\n\ntoken_introspection_in_api:\n  field: Query.tokenInfo\n  source: graphql/stackadapt-schema.graphql\n  note: The GraphQL API exposes a tokenInfo query so a caller can inspect its own token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackadapt/refs/heads/main/authentication/stackadapt-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Programmatic Advertising
- Digital Advertising
- Campaign Management
- AdTech
- DSP
- Demand-Side Platform
- Native Advertising
- Display Advertising
- Video Advertising
- Connected TV
- Audience Targeting
- Real-Time Bidding
- Conversion Tracking
- Performance Reporting
---
