---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Docketai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
overview: Docket secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Docket
provider_slug: docketai
scheme_count: 1
schemes:
- applies_to: https://demand-mcp.app.docketai.com/mcp
  endpoints:
    introspection: https://angelic-precision-36.authkit.app/oauth2/introspection
    jwks: https://angelic-precision-36.authkit.app/oauth2/jwks
    registration: https://angelic-precision-36.authkit.app/oauth2/register
  flows:
  - authorizationUrl: https://angelic-precision-36.authkit.app/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://angelic-precision-36.authkit.app/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token
  - flow: refreshToken
    tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token
  identity_provider: WorkOS AuthKit
  issuer: https://angelic-precision-36.authkit.app
  name: DocketDemandMCPOAuth
  response_modes:
  - query
  response_types:
  - code
  sources:
  - well-known/docketai-oauth-authorization-server.json
  - well-known/docketai-oauth-protected-resource.json
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: docketai-authentication
source_filename: docketai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://demand-mcp.app.docketai.com/.well-known/oauth-authorization-server\ndocs: https://help.docket.io/articles/8225942528-connect-docket-demand-mcp\n\n# Docket ships no OpenAPI, so this profile was not derived from securitySchemes. It was\n# read from the RFC 8414 authorization-server metadata and RFC 9728 protected-resource\n# metadata that the Docket Demand MCP host actually serves, plus the help centre.\n\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken]\n  bearer_methods: [header]\n  dynamic_client_registration: true\n  pkce_methods: [S256]\n\nschemes:\n  - name: DocketDemandMCPOAuth\n    type: oauth2\n    applies_to: https://demand-mcp.app.docketai.com/mcp\n    identity_provider: WorkOS AuthKit\n    issuer: https://angelic-precision-36.authkit.app\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://angelic-precision-36.authkit.app/oauth2/authorize\n\
  \        tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token\n        pkce: S256\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://angelic-precision-36.authkit.app/oauth2/device_authorization\n        tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token\n    endpoints:\n      registration: https://angelic-precision-36.authkit.app/oauth2/register\n      introspection: https://angelic-precision-36.authkit.app/oauth2/introspection\n      jwks: https://angelic-precision-36.authkit.app/oauth2/jwks\n    token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n    response_types: [code]\n    response_modes: [query]\n    sources:\n      - well-known/docketai-oauth-authorization-server.json\n      - well-known/docketai-oauth-protected-resource.json\n\nprotected_resource:\n  resource: https://demand-mcp.app.docketai.com/mcp\n  authorization_servers:\n\
  \    - https://angelic-precision-36.authkit.app/\n  bearer_methods_supported: [header]\n  scopes_supported: []\n  spec: RFC 9728\n  source: well-known/docketai-oauth-protected-resource.json\n\nauthorization_model:\n  principal: the Docket user who authorizes the connector\n  inherits: that user's Docket workspace and permissions\n  privilege: read-only (the MCP server cannot create, change or delete data)\n  admin_gate: >-\n    Some MCP clients (Claude Team/Enterprise, ChatGPT workspaces) require an\n    organization owner to add the custom connector before individual users may connect.\n  source: https://help.docket.io/articles/8225942528-connect-docket-demand-mcp\n\napplication_sign_in:\n  url: https://app.docketai.com/\n  sso: 'SSO / SAML supported on the Enterprise plan only'\n  source: https://www.docket.io/pricing\n\nnot_present:\n  - api_key: no API key, secret key or token-issuance surface is documented anywhere\n  - basic_auth: not offered\n  - mutual_tls: not offered\n  - public_rest_api:\
  \ 'Docket publishes no public REST API, so there is no REST auth model'\n\nx-evidence:\n  - url: https://demand-mcp.app.docketai.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://demand-mcp.app.docketai.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n  - url: https://demand-mcp.app.docketai.com/mcp\n    http_status: 401\n    note: 'unauthenticated JSON-RPC tools/list returned {\"error\":\"invalid_token\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docketai/refs/heads/main/authentication/docketai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- AI Agents
- Agentic Marketing
- Sales Enablement
- Demand Generation
- Marketing Automation
- Conversational AI
- Lead Qualification
- Go-To-Market
- MCP
---
