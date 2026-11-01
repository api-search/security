---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: brightedge-auth-api-openapi.yml
  format: yaml
  label: BrightEdge Auth API
  slug: brightedge-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-auth-api-openapi.yml
- filename: brightedge-authorize-api-openapi.yml
  format: yaml
  label: BrightEdge Authorize API
  slug: brightedge-authorize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-authorize-api-openapi.yml
- filename: brightedge-feedback-api-openapi.yml
  format: yaml
  label: BrightEdge Feedback API
  slug: brightedge-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-feedback-api-openapi.yml
- filename: brightedge-oauth-api-openapi.yml
  format: yaml
  label: BrightEdge OAuth API
  slug: brightedge-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-oauth-api-openapi.yml
- filename: brightedge-ping-api-openapi.yml
  format: yaml
  label: BrightEdge Ping API
  slug: brightedge-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-ping-api-openapi.yml
- filename: brightedge-saml-api-openapi.yml
  format: yaml
  label: BrightEdge SAML API
  slug: brightedge-saml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-saml-api-openapi.yml
- filename: brightedge-sso-api-openapi.yml
  format: yaml
  label: BrightEdge SSO API
  slug: brightedge-sso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-sso-api-openapi.yml
- filename: brightedge-token-api-openapi.yml
  format: yaml
  label: BrightEdge Token API
  slug: brightedge-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-token-api-openapi.yml
- filename: brightedge-well-known-api-openapi.yml
  format: yaml
  label: BrightEdge .well Known API
  slug: brightedge-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-well-known-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Brightedge Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BrightEdge secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BrightEdge
provider_slug: brightedge
scheme_count: 7
schemes:
- name: http_basic
  scheme: basic
  sources:
  - openapi/_original/brightedge-platform-openapi-original.json
  surface: rest
  type: http
- in: header
  name: forwarded_http_basic
  parameter: X-Forwarded-Authorization
  sources:
  - openapi/_original/brightedge-platform-openapi-original.json
  surface: rest
  type: apiKey
- in: cookie
  name: session_cookie
  parameter: BRIGHTEDGE
  sources:
  - openapi/_original/brightedge-platform-openapi-original.json
  surface: rest
  type: apiKey
- in: header
  name: session_header
  parameter: X-BRIGHTEDGE-SESSION
  sources:
  - openapi/_original/brightedge-platform-openapi-original.json
  surface: rest
  type: apiKey
- in: header
  name: api_token_header
  parameter: X-Token
  sources:
  - openapi/_original/brightedge-platform-openapi-original.json
  surface: rest
  type: apiKey
- in: header
  name: bearer_token
  parameter: Bearer-Token
  sources:
  - openapi/_original/brightedge-platform-openapi-original.json
  surface: rest
  type: apiKey
- bearer_alternative:
    endpoint: https://mcp2-sse.brightedge.com/sse
    note: The Manus setup guide documents a static Authorization header carrying a bearer BrightEdge token against the SSE endpoint, instead of the interactive OAuth flow.
  flows:
  - authorizationUrl: https://mcp2.brightedge.com/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
    - openid
    - profile
    - email
    tokenUrl: https://mcp2.brightedge.com/token
  identity_provider: Auth0 (mrkt-0365.us.auth0.com)
  name: brightedge-mcp-oauth
  ref: scopes/brightedge-scopes.yml
  sources:
  - https://www.brightedge.com/brightedge-mcp
  - well-known/brightedge-mcp2-oauth-authorization-server.json
  - well-known/brightedge-mcp2-oauth-protected-resource.json
  - well-known/brightedge-mcp2-openid-configuration.json
  surface: mcp
  type: oauth2
slug: brightedge-authentication
source_filename: brightedge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/brightedge-platform-openapi-original.json ; https://www.brightedge.com/brightedge-mcp\n  ; https://mcp2.brightedge.com/.well-known/oauth-authorization-server\ndocs: https://www.brightedge.com/brightedge-mcp\nnote: >-\n  BrightEdge runs two authentication models on two surfaces. The REST Platform API v5.0 uses\n  key/basic/session auth (six securitySchemes in its own OpenAPI, no OAuth). The MCP server uses\n  OAuth 2.0 authorization-code + PKCE fronted by Auth0. The OAuth half was read from the provider's\n  published setup page and from anonymously-fetched RFC 8414 / RFC 9728 / OIDC discovery documents\n  (all HTTP 200), not inferred.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [cookie, header]\n  oauth2_flows: [authorizationCode]\n  surfaces:\n    rest: [http_basic, forwarded_http_basic, session_cookie, session_header, api_token_header, bearer_token]\n    mcp: [brightedge-mcp-oauth]\n  self_serve_credentials:\
  \ false\n  credential_issuance: BrightEdge account credentials with API permission are enabled by a\n    BrightEdge representative; MCP OAuth client credentials are issued by a Customer Success\n    Manager or integrations@brightedge.com.\nschemes:\n- name: http_basic\n  type: http\n  scheme: basic\n  surface: rest\n  sources:\n  - openapi/_original/brightedge-platform-openapi-original.json\n- name: forwarded_http_basic\n  type: apiKey\n  in: header\n  parameter: X-Forwarded-Authorization\n  surface: rest\n  sources:\n  - openapi/_original/brightedge-platform-openapi-original.json\n- name: session_cookie\n  type: apiKey\n  in: cookie\n  parameter: BRIGHTEDGE\n  surface: rest\n  sources:\n  - openapi/_original/brightedge-platform-openapi-original.json\n- name: session_header\n  type: apiKey\n  in: header\n  parameter: X-BRIGHTEDGE-SESSION\n  surface: rest\n  sources:\n  - openapi/_original/brightedge-platform-openapi-original.json\n- name: api_token_header\n  type: apiKey\n  in: header\n\
  \  parameter: X-Token\n  surface: rest\n  sources:\n  - openapi/_original/brightedge-platform-openapi-original.json\n- name: bearer_token\n  type: apiKey\n  in: header\n  parameter: Bearer-Token\n  surface: rest\n  sources:\n  - openapi/_original/brightedge-platform-openapi-original.json\n- name: brightedge-mcp-oauth\n  type: oauth2\n  surface: mcp\n  identity_provider: Auth0 (mrkt-0365.us.auth0.com)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp2.brightedge.com/authorize\n    tokenUrl: https://mcp2.brightedge.com/token\n    pkce: S256\n    scopes: [openid, profile, email]\n  bearer_alternative:\n    note: >-\n      The Manus setup guide documents a static Authorization header carrying a bearer\n      BrightEdge token against the SSE endpoint, instead of the interactive OAuth flow.\n    endpoint: https://mcp2-sse.brightedge.com/sse\n  ref: scopes/brightedge-scopes.yml\n  sources:\n  - https://www.brightedge.com/brightedge-mcp\n  - well-known/brightedge-mcp2-oauth-authorization-server.json\n\
  \  - well-known/brightedge-mcp2-oauth-protected-resource.json\n  - well-known/brightedge-mcp2-openid-configuration.json\ndiscovery:\n- url: https://mcp2.brightedge.com/.well-known/oauth-authorization-server\n  status: 200\n- url: https://mcp2.brightedge.com/.well-known/oauth-protected-resource\n  status: 200\n- url: https://mcp2.brightedge.com/.well-known/openid-configuration\n  status: 200\n- url: https://api.brightedge.com/.well-known/oauth-authorization-server\n  status: 404\n"
source_yaml_url: https://artifacts.apis.io/brightedge/authentication/brightedge-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Company
- SEO
- Search
- Content
- Marketing
- Analytics
- Keywords
- Enterprise
- AI Search
---
